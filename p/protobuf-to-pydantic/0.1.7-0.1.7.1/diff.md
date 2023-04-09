# Comparing `tmp/protobuf_to_pydantic-0.1.7.tar.gz` & `tmp/protobuf_to_pydantic-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protobuf_to_pydantic-0.1.7.tar", max compression
+gzip compressed data, was "protobuf_to_pydantic-0.1.7.1.tar", max compression
```

## Comparing `protobuf_to_pydantic-0.1.7.tar` & `protobuf_to_pydantic-0.1.7.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 protobuf_to_pydantic-0.1.7/LICENSE
--rw-r--r--   0        0        0    33623 2023-03-23 17:23:44.348493 protobuf_to_pydantic-0.1.7/README.md
--rw-r--r--   0        0        0      157 2023-04-06 10:17:44.904269 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/__init__.py
--rw-r--r--   0        0        0       23 2023-04-06 10:22:05.460616 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/__version__.py
--rw-r--r--   0        0        0        0 2022-06-28 03:26:29.000000 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/contrib/__init__.py
--rw-r--r--   0        0        0    14814 2023-03-19 16:10:34.117082 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/contrib/proto_parser.py
--rw-r--r--   0        0        0     7873 2022-08-19 06:41:43.000000 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/customer_con_type.py
--rw-r--r--   0        0        0    11699 2023-03-19 16:10:34.117082 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/customer_validator.py
--rw-r--r--   0        0        0    23793 2023-04-06 10:17:44.588269 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/gen_code.py
--rw-r--r--   0        0        0    27724 2023-04-02 18:33:55.827477 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/gen_model.py
--rw-r--r--   0        0        0      169 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/__init__.py
--rw-r--r--   0        0        0      134 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pb_option/__init__.py
--rw-r--r--   0        0        0    14497 2023-03-30 12:19:52.880142 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pb_option/base.py
--rw-r--r--   0        0        0      479 2023-02-21 11:07:15.262565 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pb_option/from_p2p.py
--rw-r--r--   0        0        0      356 2023-02-21 11:07:15.326564 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pb_option/from_pgv.py
--rw-r--r--   0        0        0     2074 2022-07-30 20:12:53.000000 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pb_option/types.py
--rw-r--r--   0        0        0     3663 2023-03-31 07:16:34.356473 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_proto_file.py
--rw-r--r--   0        0        0     5626 2023-02-23 06:43:54.137679 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pyi_file.py
--rw-r--r--   0        0        0     1517 2023-03-30 17:36:31.267633 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/grpc_types.py
--rw-r--r--   0        0        0        0 2022-12-04 12:28:50.000000 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/__init__.py
--rw-r--r--   0        0        0       31 2022-12-28 10:00:32.000000 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/__main__.py
--rw-r--r--   0        0        0     3508 2023-04-01 17:20:07.477049 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/code_gen.py
--rw-r--r--   0        0        0     2482 2023-03-30 07:29:18.237163 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/config.py
--rw-r--r--   0        0        0    19530 2023-03-31 10:20:32.030717 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py
--rwxr-xr-x   0        0        0      347 2023-03-30 03:00:46.463995 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/main.py
--rw-r--r--   0        0        0      332 2023-02-22 17:08:00.346785 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/my_types.py
--rw-r--r--   0        0        0   363829 2023-04-06 10:15:51.416121 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0   176974 2023-04-06 10:15:51.416121 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-04-06 10:18:12.628306 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.py
--rw-r--r--   0        0        0      169 2023-04-06 10:15:51.416121 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.pyi
--rw-r--r--   0        0        0   121461 2023-04-06 10:15:51.416121 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-04-06 10:15:51.416121 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-04-06 10:18:12.628306 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-06 10:15:51.416121 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0      270 2023-04-01 17:49:33.439309 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0    32541 2023-04-06 10:16:08.108142 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0   176974 2023-04-06 10:16:08.108142 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-04-06 10:18:12.592306 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.py
--rw-r--r--   0        0        0      169 2023-04-06 10:16:08.108142 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.pyi
--rw-r--r--   0        0        0    13083 2023-04-06 10:16:08.108142 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-04-06 10:16:08.108142 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-04-06 10:18:12.628306 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-06 10:16:08.108142 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0      262 2023-04-01 17:20:07.469049 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/validate_pb2.py
--rw-r--r--   0        0        0     1593 2023-02-22 16:09:35.749710 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/types.py
--rw-r--r--   0        0        0     5755 2023-04-02 18:31:56.063240 protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/util.py
--rw-r--r--   0        0        0     3107 2023-04-06 10:22:05.460616 protobuf_to_pydantic-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    35925 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.1.7/setup.py
--rw-r--r--   0        0        0    34839 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 protobuf_to_pydantic-0.1.7.1/LICENSE
+-rw-r--r--   0        0        0    33623 2023-03-23 17:23:44.348493 protobuf_to_pydantic-0.1.7.1/README.md
+-rw-r--r--   0        0        0      157 2023-04-06 10:17:44.904269 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-09 16:21:35.619100 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/__version__.py
+-rw-r--r--   0        0        0        0 2022-06-28 03:26:29.000000 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/contrib/__init__.py
+-rw-r--r--   0        0        0    14814 2023-03-19 16:10:34.117082 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/contrib/proto_parser.py
+-rw-r--r--   0        0        0     7873 2022-08-19 06:41:43.000000 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/customer_con_type.py
+-rw-r--r--   0        0        0    11699 2023-03-19 16:10:34.117082 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/customer_validator.py
+-rw-r--r--   0        0        0    23793 2023-04-06 10:17:44.588269 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/gen_code.py
+-rw-r--r--   0        0        0    28283 2023-04-09 15:30:54.888047 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/gen_model.py
+-rw-r--r--   0        0        0      169 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/__init__.py
+-rw-r--r--   0        0        0      134 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pb_option/__init__.py
+-rw-r--r--   0        0        0    14497 2023-03-30 12:19:52.880142 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pb_option/base.py
+-rw-r--r--   0        0        0      479 2023-02-21 11:07:15.262565 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pb_option/from_p2p.py
+-rw-r--r--   0        0        0      356 2023-02-21 11:07:15.326564 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pb_option/from_pgv.py
+-rw-r--r--   0        0        0     2074 2022-07-30 20:12:53.000000 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pb_option/types.py
+-rw-r--r--   0        0        0     3663 2023-03-31 07:16:34.356473 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_proto_file.py
+-rw-r--r--   0        0        0     5626 2023-02-23 06:43:54.137679 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pyi_file.py
+-rw-r--r--   0        0        0     1517 2023-03-30 17:36:31.267633 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/grpc_types.py
+-rw-r--r--   0        0        0        0 2022-12-04 12:28:50.000000 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/__init__.py
+-rw-r--r--   0        0        0       31 2022-12-28 10:00:32.000000 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/__main__.py
+-rw-r--r--   0        0        0     3508 2023-04-01 17:20:07.477049 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/code_gen.py
+-rw-r--r--   0        0        0     2482 2023-03-30 07:29:18.237163 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/config.py
+-rw-r--r--   0        0        0    19530 2023-03-31 10:20:32.030717 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py
+-rwxr-xr-x   0        0        0      347 2023-03-30 03:00:46.463995 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/main.py
+-rw-r--r--   0        0        0      332 2023-02-22 17:08:00.346785 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/my_types.py
+-rw-r--r--   0        0        0   383358 2023-04-09 16:16:19.083932 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0   185862 2023-04-09 16:16:19.083932 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-04-09 16:18:53.561574 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.py
+-rw-r--r--   0        0        0      169 2023-04-09 16:16:19.083932 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0   121461 2023-04-09 16:16:19.083932 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-04-09 16:16:19.083932 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-04-09 16:18:53.569574 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-09 16:16:19.083932 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0      270 2023-04-01 17:49:33.439309 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0    34121 2023-04-09 16:16:35.411683 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0   185862 2023-04-09 16:16:35.411683 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-04-09 16:18:53.549574 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.py
+-rw-r--r--   0        0        0      169 2023-04-09 16:16:35.411683 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13083 2023-04-09 16:16:35.411683 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-04-09 16:16:35.411683 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-04-09 16:18:53.557574 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-09 16:16:35.411683 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0      262 2023-04-01 17:20:07.469049 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/validate_pb2.py
+-rw-r--r--   0        0        0     1593 2023-02-22 16:09:35.749710 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/types.py
+-rw-r--r--   0        0        0     5755 2023-04-02 18:31:56.063240 protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/util.py
+-rw-r--r--   0        0        0     3109 2023-04-09 16:21:35.619100 protobuf_to_pydantic-0.1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    35927 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.1.7.1/setup.py
+-rw-r--r--   0        0        0    34841 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.1.7.1/PKG-INFO
```

### Comparing `protobuf_to_pydantic-0.1.7/LICENSE` & `protobuf_to_pydantic-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/README.md` & `protobuf_to_pydantic-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/contrib/proto_parser.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/contrib/proto_parser.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/customer_con_type.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/customer_con_type.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/customer_validator.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/customer_validator.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/gen_code.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/gen_code.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/gen_model.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/gen_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 import json
 from dataclasses import MISSING
 from enum import IntEnum
 from importlib import import_module
 from pathlib import Path
 from types import ModuleType
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Generator, List, Optional, Tuple, Type, Union
 
 from pydantic import BaseModel, Field, root_validator
 from pydantic.fields import FieldInfo, Undefined
 from pydantic.typing import NoArgAnyCallable
 
 from protobuf_to_pydantic.customer_validator import check_one_of
 from protobuf_to_pydantic.get_desc import (
@@ -159,14 +159,31 @@
             # If a nested type is found, use the same treatment
             field_param_dict_handle(sub_field_param_dict, default, default_factory)
             field_param_dict["type_"] = field_type(sub_field_param_dict["type_"], **type_param_dict)
         else:
             field_param_dict["type_"] = field_type(**type_param_dict)
 
 
+class JsonAndDict(dict):
+    @classmethod
+    def __get_validators__(cls) -> Generator[Callable, None, None]:
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, v: Union[str, dict]) -> dict:
+        if isinstance(v, str):
+            try:
+                v = json.loads(v)
+            except json.JSONDecodeError:
+                raise ValueError("JSON string is not valid JSON")
+        elif not isinstance(v, dict):
+            raise ValueError("JSON string is not a dict")
+        return v  # type: ignore[return-value]
+
+
 class MessagePaitModel(BaseModel):
     field: Optional[Type[FieldInfo]] = Field(None)
     enable: bool = Field(True)
     miss_default: bool = Field(False)
     default: Optional[Any] = Field(None)
     default_factory: Optional[Callable] = Field(None)
     example: Any = Field(MISSING)
@@ -182,15 +199,15 @@
     min_length: Optional[int] = Field(None)
     max_length: Optional[int] = Field(None)
     min_items: Optional[int] = Field(None)
     max_items: Optional[int] = Field(None)
     unique_items: Optional[bool] = Field(None)
     multiple_of: Optional[int] = Field(None)
     regex: Optional[str] = Field(None)
-    extra: dict = Field(default_factory=dict)
+    extra: JsonAndDict = Field(default_factory=dict)
     type_: Any = Field(None, alias="type")
     validator: Optional[Dict[str, Any]] = Field(None)
     sub: Optional["MessagePaitModel"] = Field(None)
     map_type: Optional[Dict[str, type]] = Field(None)
 
 
 class DescTemplate(object):
```

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pb_option/base.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pb_option/base.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pb_option/types.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pb_option/types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_proto_file.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_proto_file.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/get_desc/from_pyi_file.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/get_desc/from_pyi_file.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/grpc_types.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/grpc_types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/code_gen.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/code_gen.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/config.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/config.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='protos/p2p_validate.proto',
   package='p2p_validate',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x19protos/p2p_validate.proto\x12\x0cp2p_validate\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x81\x08\n\nFieldRules\x12\x30\n\x07message\x18\x11 \x01(\x0b\x32\x1a.p2p_validate.MessageRulesH\x01\x88\x01\x01\x12)\n\x05\x66loat\x18\x01 \x01(\x0b\x32\x18.p2p_validate.FloatRulesH\x00\x12+\n\x06\x64ouble\x18\x02 \x01(\x0b\x32\x19.p2p_validate.DoubleRulesH\x00\x12)\n\x05int32\x18\x03 \x01(\x0b\x32\x18.p2p_validate.Int32RulesH\x00\x12)\n\x05int64\x18\x04 \x01(\x0b\x32\x18.p2p_validate.Int64RulesH\x00\x12+\n\x06uint32\x18\x05 \x01(\x0b\x32\x19.p2p_validate.UInt32RulesH\x00\x12+\n\x06uint64\x18\x06 \x01(\x0b\x32\x19.p2p_validate.UInt64RulesH\x00\x12+\n\x06sint32\x18\x07 \x01(\x0b\x32\x19.p2p_validate.SInt32RulesH\x00\x12+\n\x06sint64\x18\x08 \x01(\x0b\x32\x19.p2p_validate.SInt64RulesH\x00\x12-\n\x07\x66ixed32\x18\t \x01(\x0b\x32\x1a.p2p_validate.Fixed32RulesH\x00\x12-\n\x07\x66ixed64\x18\n \x01(\x0b\x32\x1a.p2p_validate.Fixed64RulesH\x00\x12/\n\x08sfixed32\x18\x0b \x01(\x0b\x32\x1b.p2p_validate.SFixed32RulesH\x00\x12/\n\x08sfixed64\x18\x0c \x01(\x0b\x32\x1b.p2p_validate.SFixed64RulesH\x00\x12\'\n\x04\x62ool\x18\r \x01(\x0b\x32\x17.p2p_validate.BoolRulesH\x00\x12+\n\x06string\x18\x0e \x01(\x0b\x32\x19.p2p_validate.StringRulesH\x00\x12)\n\x05\x62ytes\x18\x0f \x01(\x0b\x32\x18.p2p_validate.BytesRulesH\x00\x12\'\n\x04\x65num\x18\x10 \x01(\x0b\x32\x17.p2p_validate.EnumRulesH\x00\x12/\n\x08repeated\x18\x12 \x01(\x0b\x32\x1b.p2p_validate.RepeatedRulesH\x00\x12%\n\x03map\x18\x13 \x01(\x0b\x32\x16.p2p_validate.MapRulesH\x00\x12%\n\x03\x61ny\x18\x14 \x01(\x0b\x32\x16.p2p_validate.AnyRulesH\x00\x12/\n\x08\x64uration\x18\x15 \x01(\x0b\x32\x1b.p2p_validate.DurationRulesH\x00\x12\x31\n\ttimestamp\x18\x16 \x01(\x0b\x32\x1c.p2p_validate.TimestampRulesH\x00\x42\x06\n\x04typeB\n\n\x08_message\"\xa8\x04\n\nFloatRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x02H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x02H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x02H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x02H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x02H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x02\x12\x0e\n\x06not_in\x18\x07 \x03(\x02\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0b\x44oubleRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x01H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x01H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x01H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x01H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x01H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x01\x12\x0e\n\x06not_in\x18\x07 \x03(\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa8\x04\n\nInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x05H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x05H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x05H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x05H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x05\x12\x0e\n\x06not_in\x18\x07 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa8\x04\n\nInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x03H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x03H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x03H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x03H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x03H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x03\x12\x0e\n\x06not_in\x18\x07 \x03(\x03\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0bUInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\rH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\rH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\rH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\rH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\rH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\r\x12\x0e\n\x06not_in\x18\x07 \x03(\r\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0bUInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x04H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x04H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x04H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x04\x12\x0e\n\x06not_in\x18\x07 \x03(\x04\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0bSInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x11H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x11H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x11H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x11H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x11H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x11\x12\x0e\n\x06not_in\x18\x07 \x03(\x11\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0bSInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x12H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x12H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x12H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x12H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x12H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x12\x12\x0e\n\x06not_in\x18\x07 \x03(\x12\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xaa\x04\n\x0c\x46ixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x07H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x07H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x07H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x07H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x07H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x07\x12\x0e\n\x06not_in\x18\x07 \x03(\x07\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xaa\x04\n\x0c\x46ixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x06H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x06H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x06H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x06H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x06H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x06\x12\x0e\n\x06not_in\x18\x07 \x03(\x06\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xab\x04\n\rSFixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0fH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x0fH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x0fH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x0fH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x0fH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x0f\x12\x0e\n\x06not_in\x18\x07 \x03(\x0f\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xab\x04\n\rSFixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x10H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x10H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x10H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x10H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x10H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x10\x12\x0e\n\x06not_in\x18\x07 \x03(\x10\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xc8\x02\n\tBoolRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x08H\x01\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x02 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x03 \x01(\x08H\x00\x12\x16\n\x0cmiss_default\x18\x04 \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x04\x88\x01\x01\x12\x14\n\x07\x65xample\x18\x07 \x01(\x08H\x05\x88\x01\x01\x12\x12\n\x05\x66ield\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x11\n\x04type\x18\t \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x08\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\n\n\x08_exampleB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xfa\x06\n\x0bStringRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\tH\x03\x88\x01\x01\x12\x10\n\x03len\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmin_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x17\n\nmax_length\x18\x04 \x01(\x04H\x06\x88\x01\x01\x12\x14\n\x07pattern\x18\x05 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x06prefix\x18\x06 \x01(\tH\x08\x88\x01\x01\x12\x13\n\x06suffix\x18\x07 \x01(\tH\t\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x08 \x01(\tH\n\x88\x01\x01\x12\x19\n\x0cnot_contains\x18\t \x01(\tH\x0b\x88\x01\x01\x12\n\n\x02in\x18\n \x03(\t\x12\x0e\n\x06not_in\x18\x0b \x03(\t\x12\x0f\n\x05\x65mail\x18\x0c \x01(\x08H\x00\x12\x12\n\x08hostname\x18\r \x01(\x08H\x00\x12\x0c\n\x02ip\x18\x0e \x01(\x08H\x00\x12\x0e\n\x04ipv4\x18\x0f \x01(\x08H\x00\x12\x0e\n\x04ipv6\x18\x10 \x01(\x08H\x00\x12\r\n\x03uri\x18\x11 \x01(\x08H\x00\x12\x11\n\x07uri_ref\x18\x12 \x01(\x08H\x00\x12\x11\n\x07\x61\x64\x64ress\x18\x15 \x01(\x08H\x00\x12\x0e\n\x04uuid\x18\x16 \x01(\x08H\x00\x12\x17\n\rpydantic_type\x18\x63 \x01(\tH\x00\x12\x13\n\x06\x65nable\x18\x17 \x01(\x08H\x0c\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x18 \x01(\tH\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x19 \x01(\tH\x01\x12\x16\n\x0cmiss_default\x18\x1a \x01(\x08H\x01\x12\x12\n\x05\x61lias\x18\x1b \x01(\tH\r\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x1c \x01(\tH\x0e\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x1e \x01(\tH\x02\x12\x19\n\x0f\x65xample_factory\x18\x1f \x01(\tH\x02\x12\x12\n\x05\x66ield\x18  \x01(\tH\x0f\x88\x01\x01\x12\x11\n\x04type\x18! \x01(\tH\x10\x88\x01\x01\x12\x12\n\x05title\x18\" \x01(\tH\x11\x88\x01\x01\x42\x0c\n\nwell_knownB\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x06\n\x04_lenB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\n\n\x08_patternB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\x0f\n\r_not_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xb8\x05\n\nBytesRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0cH\x03\x88\x01\x01\x12\x17\n\nmin_length\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmax_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06prefix\x18\x05 \x01(\x0cH\x06\x88\x01\x01\x12\x13\n\x06suffix\x18\x06 \x01(\x0cH\x07\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x07 \x01(\x0cH\x08\x88\x01\x01\x12\n\n\x02in\x18\x08 \x03(\x0c\x12\x0e\n\x06not_in\x18\t \x03(\x0c\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\t\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0cH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\n\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x10 \x01(\x02H\x0c\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x11 \x01(\x0cH\x01\x12\x19\n\x0f\x65xample_factory\x18\x12 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x14 \x01(\tH\x0e\x88\x01\x01\x12\x0c\n\x02ip\x18\x15 \x01(\x08H\x02\x12\x0e\n\x04ipv4\x18\x16 \x01(\x08H\x02\x12\x0e\n\x04ipv6\x18\x17 \x01(\x08H\x02\x12\x12\n\x05title\x18\x18 \x01(\tH\x0f\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\nwell_knownB\x08\n\x06_constB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\x81\x03\n\tEnumRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\n\n\x02in\x18\x03 \x03(\x05\x12\x0e\n\x06not_in\x18\x04 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x05H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x05H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x12 \x01(\tH\x07\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_title\"\xa6\x03\n\x0cMessageRules\x12\x11\n\x04skip\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\x15\n\x08required\x18\x02 \x01(\x08H\x03\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x04\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x05\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x06\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x07\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x08\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\t\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x07\n\x05_skipB\x0b\n\t_requiredB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xe5\x03\n\rRepeatedRules\x12\x16\n\tmin_items\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_items\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x13\n\x06unique\x18\x03 \x01(\x08H\x04\x88\x01\x01\x12,\n\x05items\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_itemsB\x0c\n\n_max_itemsB\t\n\x07_uniqueB\x08\n\x06_itemsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xf8\x03\n\x08MapRules\x12\x16\n\tmin_pairs\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_pairs\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12+\n\x04keys\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x04\x88\x01\x01\x12-\n\x06values\x18\x05 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_pairsB\x0c\n\n_max_pairsB\x07\n\x05_keysB\t\n\x07_valuesB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\x86\x03\n\x08\x41nyRules\x12\x15\n\x08required\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\n\n\x02in\x18\x02 \x03(\t\x12\x0e\n\x06not_in\x18\x03 \x03(\t\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\tH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0e \x01(\tH\x01\x12\x19\n\x0f\x65xample_factory\x18\x0f \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x10 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x11 \x01(\tH\x07\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0b\n\t_requiredB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_title\"\xf4\x05\n\rDurationRules\x12-\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationH\x02\x88\x01\x01\x12*\n\x02lt\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationH\x03\x88\x01\x01\x12*\n\x02le\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationH\x04\x88\x01\x01\x12*\n\x02gt\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationH\x05\x88\x01\x01\x12*\n\x02ge\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationH\x06\x88\x01\x01\x12%\n\x02in\x18\x07 \x03(\x0b\x32\x19.google.protobuf.Duration\x12)\n\x06not_in\x18\x08 \x03(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x06\x65nable\x18\x0e \x01(\x08H\x07\x88\x01\x01\x12,\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12,\n\x07\x65xample\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationH\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\n\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0c\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa5\x06\n\x0eTimestampRules\x12.\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12+\n\x02lt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12+\n\x02le\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x12+\n\x02gt\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12+\n\x02ge\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x13\n\x06lt_now\x18\x07 \x01(\x08H\x07\x88\x01\x01\x12\x13\n\x06gt_now\x18\x08 \x01(\x08H\x08\x88\x01\x01\x12.\n\x06within\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\t\x88\x01\x01\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\n\x88\x01\x01\x12-\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0c\x88\x01\x01\x12-\n\x07\x65xample\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x12\x19\n\x0f\x65xample_factory\x18\x11 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x12 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x13 \x01(\tH\x0e\x88\x01\x01\x12\x12\n\x05title\x18\x14 \x01(\tH\x0f\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_lt_nowB\t\n\x07_gt_nowB\t\n\x07_withinB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title:4\n\x07ignored\x12\x1f.google.protobuf.MessageOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:3\n\x08required\x12\x1d.google.protobuf.OneofOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:J\n\x05rules\x12\x1d.google.protobuf.FieldOptions\x18\xb1\x08 \x01(\x0b\x32\x18.p2p_validate.FieldRules\x88\x01\x01\x62\x06proto3'
+  serialized_pb=b'\n\x19protos/p2p_validate.proto\x12\x0cp2p_validate\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x81\x08\n\nFieldRules\x12\x30\n\x07message\x18\x11 \x01(\x0b\x32\x1a.p2p_validate.MessageRulesH\x01\x88\x01\x01\x12)\n\x05\x66loat\x18\x01 \x01(\x0b\x32\x18.p2p_validate.FloatRulesH\x00\x12+\n\x06\x64ouble\x18\x02 \x01(\x0b\x32\x19.p2p_validate.DoubleRulesH\x00\x12)\n\x05int32\x18\x03 \x01(\x0b\x32\x18.p2p_validate.Int32RulesH\x00\x12)\n\x05int64\x18\x04 \x01(\x0b\x32\x18.p2p_validate.Int64RulesH\x00\x12+\n\x06uint32\x18\x05 \x01(\x0b\x32\x19.p2p_validate.UInt32RulesH\x00\x12+\n\x06uint64\x18\x06 \x01(\x0b\x32\x19.p2p_validate.UInt64RulesH\x00\x12+\n\x06sint32\x18\x07 \x01(\x0b\x32\x19.p2p_validate.SInt32RulesH\x00\x12+\n\x06sint64\x18\x08 \x01(\x0b\x32\x19.p2p_validate.SInt64RulesH\x00\x12-\n\x07\x66ixed32\x18\t \x01(\x0b\x32\x1a.p2p_validate.Fixed32RulesH\x00\x12-\n\x07\x66ixed64\x18\n \x01(\x0b\x32\x1a.p2p_validate.Fixed64RulesH\x00\x12/\n\x08sfixed32\x18\x0b \x01(\x0b\x32\x1b.p2p_validate.SFixed32RulesH\x00\x12/\n\x08sfixed64\x18\x0c \x01(\x0b\x32\x1b.p2p_validate.SFixed64RulesH\x00\x12\'\n\x04\x62ool\x18\r \x01(\x0b\x32\x17.p2p_validate.BoolRulesH\x00\x12+\n\x06string\x18\x0e \x01(\x0b\x32\x19.p2p_validate.StringRulesH\x00\x12)\n\x05\x62ytes\x18\x0f \x01(\x0b\x32\x18.p2p_validate.BytesRulesH\x00\x12\'\n\x04\x65num\x18\x10 \x01(\x0b\x32\x17.p2p_validate.EnumRulesH\x00\x12/\n\x08repeated\x18\x12 \x01(\x0b\x32\x1b.p2p_validate.RepeatedRulesH\x00\x12%\n\x03map\x18\x13 \x01(\x0b\x32\x16.p2p_validate.MapRulesH\x00\x12%\n\x03\x61ny\x18\x14 \x01(\x0b\x32\x16.p2p_validate.AnyRulesH\x00\x12/\n\x08\x64uration\x18\x15 \x01(\x0b\x32\x1b.p2p_validate.DurationRulesH\x00\x12\x31\n\ttimestamp\x18\x16 \x01(\x0b\x32\x1c.p2p_validate.TimestampRulesH\x00\x42\x06\n\x04typeB\n\n\x08_message\"\xc6\x04\n\nFloatRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x02H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x02H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x02H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x02H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x02H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x02\x12\x0e\n\x06not_in\x18\x07 \x03(\x02\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0b\x44oubleRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x01H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x01H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x01H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x01H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x01H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x01\x12\x0e\n\x06not_in\x18\x07 \x03(\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc6\x04\n\nInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x05H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x05H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x05H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x05H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x05\x12\x0e\n\x06not_in\x18\x07 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc6\x04\n\nInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x03H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x03H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x03H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x03H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x03H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x03\x12\x0e\n\x06not_in\x18\x07 \x03(\x03\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0bUInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\rH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\rH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\rH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\rH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\rH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\r\x12\x0e\n\x06not_in\x18\x07 \x03(\r\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0bUInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x04H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x04H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x04H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x04\x12\x0e\n\x06not_in\x18\x07 \x03(\x04\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0bSInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x11H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x11H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x11H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x11H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x11H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x11\x12\x0e\n\x06not_in\x18\x07 \x03(\x11\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0bSInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x12H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x12H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x12H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x12H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x12H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x12\x12\x0e\n\x06not_in\x18\x07 \x03(\x12\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc8\x04\n\x0c\x46ixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x07H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x07H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x07H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x07H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x07H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x07\x12\x0e\n\x06not_in\x18\x07 \x03(\x07\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc8\x04\n\x0c\x46ixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x06H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x06H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x06H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x06H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x06H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x06\x12\x0e\n\x06not_in\x18\x07 \x03(\x06\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc9\x04\n\rSFixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0fH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x0fH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x0fH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x0fH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x0fH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x0f\x12\x0e\n\x06not_in\x18\x07 \x03(\x0f\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc9\x04\n\rSFixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x10H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x10H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x10H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x10H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x10H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x10\x12\x0e\n\x06not_in\x18\x07 \x03(\x10\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xe6\x02\n\tBoolRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x08H\x01\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x02 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x03 \x01(\x08H\x00\x12\x16\n\x0cmiss_default\x18\x04 \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x04\x88\x01\x01\x12\x14\n\x07\x65xample\x18\x07 \x01(\x08H\x05\x88\x01\x01\x12\x12\n\x05\x66ield\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x11\n\x04type\x18\t \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x08\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\t\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\n\n\x08_exampleB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x98\x07\n\x0bStringRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\tH\x03\x88\x01\x01\x12\x10\n\x03len\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmin_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x17\n\nmax_length\x18\x04 \x01(\x04H\x06\x88\x01\x01\x12\x14\n\x07pattern\x18\x05 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x06prefix\x18\x06 \x01(\tH\x08\x88\x01\x01\x12\x13\n\x06suffix\x18\x07 \x01(\tH\t\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x08 \x01(\tH\n\x88\x01\x01\x12\x19\n\x0cnot_contains\x18\t \x01(\tH\x0b\x88\x01\x01\x12\n\n\x02in\x18\n \x03(\t\x12\x0e\n\x06not_in\x18\x0b \x03(\t\x12\x0f\n\x05\x65mail\x18\x0c \x01(\x08H\x00\x12\x12\n\x08hostname\x18\r \x01(\x08H\x00\x12\x0c\n\x02ip\x18\x0e \x01(\x08H\x00\x12\x0e\n\x04ipv4\x18\x0f \x01(\x08H\x00\x12\x0e\n\x04ipv6\x18\x10 \x01(\x08H\x00\x12\r\n\x03uri\x18\x11 \x01(\x08H\x00\x12\x11\n\x07uri_ref\x18\x12 \x01(\x08H\x00\x12\x11\n\x07\x61\x64\x64ress\x18\x15 \x01(\x08H\x00\x12\x0e\n\x04uuid\x18\x16 \x01(\x08H\x00\x12\x17\n\rpydantic_type\x18\x63 \x01(\tH\x00\x12\x13\n\x06\x65nable\x18\x17 \x01(\x08H\x0c\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x18 \x01(\tH\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x19 \x01(\tH\x01\x12\x16\n\x0cmiss_default\x18\x1a \x01(\x08H\x01\x12\x12\n\x05\x61lias\x18\x1b \x01(\tH\r\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x1c \x01(\tH\x0e\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x1e \x01(\tH\x02\x12\x19\n\x0f\x65xample_factory\x18\x1f \x01(\tH\x02\x12\x12\n\x05\x66ield\x18  \x01(\tH\x0f\x88\x01\x01\x12\x11\n\x04type\x18! \x01(\tH\x10\x88\x01\x01\x12\x12\n\x05title\x18\" \x01(\tH\x11\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x12\x88\x01\x01\x42\x0c\n\nwell_knownB\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x06\n\x04_lenB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\n\n\x08_patternB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\x0f\n\r_not_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xd6\x05\n\nBytesRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0cH\x03\x88\x01\x01\x12\x17\n\nmin_length\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmax_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06prefix\x18\x05 \x01(\x0cH\x06\x88\x01\x01\x12\x13\n\x06suffix\x18\x06 \x01(\x0cH\x07\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x07 \x01(\x0cH\x08\x88\x01\x01\x12\n\n\x02in\x18\x08 \x03(\x0c\x12\x0e\n\x06not_in\x18\t \x03(\x0c\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\t\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0cH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\n\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x10 \x01(\x02H\x0c\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x11 \x01(\x0cH\x01\x12\x19\n\x0f\x65xample_factory\x18\x12 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x14 \x01(\tH\x0e\x88\x01\x01\x12\x0c\n\x02ip\x18\x15 \x01(\x08H\x02\x12\x0e\n\x04ipv4\x18\x16 \x01(\x08H\x02\x12\x0e\n\x04ipv6\x18\x17 \x01(\x08H\x02\x12\x12\n\x05title\x18\x18 \x01(\tH\x0f\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x19 \x01(\tH\x10\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\nwell_knownB\x08\n\x06_constB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x9f\x03\n\tEnumRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\n\n\x02in\x18\x03 \x03(\x05\x12\x0e\n\x06not_in\x18\x04 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x05H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x05H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x12 \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x08\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_titleB\x08\n\x06_extra\"\xc4\x03\n\x0cMessageRules\x12\x11\n\x04skip\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\x15\n\x08required\x18\x02 \x01(\x08H\x03\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x04\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x05\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x06\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x07\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x08\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\t\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\n\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x07\n\x05_skipB\x0b\n\t_requiredB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x83\x04\n\rRepeatedRules\x12\x16\n\tmin_items\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_items\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x13\n\x06unique\x18\x03 \x01(\x08H\x04\x88\x01\x01\x12,\n\x05items\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0c\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_itemsB\x0c\n\n_max_itemsB\t\n\x07_uniqueB\x08\n\x06_itemsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x96\x04\n\x08MapRules\x12\x16\n\tmin_pairs\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_pairs\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12+\n\x04keys\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x04\x88\x01\x01\x12-\n\x06values\x18\x05 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0c\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_pairsB\x0c\n\n_max_pairsB\x07\n\x05_keysB\t\n\x07_valuesB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xa4\x03\n\x08\x41nyRules\x12\x15\n\x08required\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\n\n\x02in\x18\x02 \x03(\t\x12\x0e\n\x06not_in\x18\x03 \x03(\t\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\tH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0e \x01(\tH\x01\x12\x19\n\x0f\x65xample_factory\x18\x0f \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x10 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x11 \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x08\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0b\n\t_requiredB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_titleB\x08\n\x06_extra\"\x92\x06\n\rDurationRules\x12-\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationH\x02\x88\x01\x01\x12*\n\x02lt\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationH\x03\x88\x01\x01\x12*\n\x02le\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationH\x04\x88\x01\x01\x12*\n\x02gt\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationH\x05\x88\x01\x01\x12*\n\x02ge\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationH\x06\x88\x01\x01\x12%\n\x02in\x18\x07 \x03(\x0b\x32\x19.google.protobuf.Duration\x12)\n\x06not_in\x18\x08 \x03(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x06\x65nable\x18\x0e \x01(\x08H\x07\x88\x01\x01\x12,\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12,\n\x07\x65xample\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationH\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\n\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc3\x06\n\x0eTimestampRules\x12.\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12+\n\x02lt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12+\n\x02le\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x12+\n\x02gt\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12+\n\x02ge\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x13\n\x06lt_now\x18\x07 \x01(\x08H\x07\x88\x01\x01\x12\x13\n\x06gt_now\x18\x08 \x01(\x08H\x08\x88\x01\x01\x12.\n\x06within\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\t\x88\x01\x01\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\n\x88\x01\x01\x12-\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0c\x88\x01\x01\x12-\n\x07\x65xample\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x12\x19\n\x0f\x65xample_factory\x18\x11 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x12 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x13 \x01(\tH\x0e\x88\x01\x01\x12\x12\n\x05title\x18\x14 \x01(\tH\x0f\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x15 \x01(\tH\x10\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_lt_nowB\t\n\x07_gt_nowB\t\n\x07_withinB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra:4\n\x07ignored\x12\x1f.google.protobuf.MessageOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:3\n\x08required\x12\x1d.google.protobuf.OneofOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:J\n\x05rules\x12\x1d.google.protobuf.FieldOptions\x18\xb1\x08 \x01(\x0b\x32\x18.p2p_validate.FieldRules\x88\x01\x01\x62\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_descriptor__pb2.DESCRIPTOR,google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 
 IGNORED_FIELD_NUMBER = 1073
 ignored = _descriptor.FieldDescriptor(
   name='ignored', full_name='p2p_validate.ignored', index=0,
@@ -379,14 +379,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.FloatRules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.FloatRules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -460,17 +467,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.FloatRules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.FloatRules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
   serialized_start=1171,
-  serialized_end=1723,
+  serialized_end=1753,
 )
 
 
 _DOUBLERULES = _descriptor.Descriptor(
   name='DoubleRules',
   full_name='p2p_validate.DoubleRules',
   filename=None,
@@ -607,14 +619,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.DoubleRules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.DoubleRules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -688,17 +707,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.DoubleRules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.DoubleRules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=1726,
-  serialized_end=2279,
+  serialized_start=1756,
+  serialized_end=2339,
 )
 
 
 _INT32RULES = _descriptor.Descriptor(
   name='Int32Rules',
   full_name='p2p_validate.Int32Rules',
   filename=None,
@@ -835,14 +859,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.Int32Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.Int32Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -916,17 +947,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.Int32Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.Int32Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=2282,
-  serialized_end=2834,
+  serialized_start=2342,
+  serialized_end=2924,
 )
 
 
 _INT64RULES = _descriptor.Descriptor(
   name='Int64Rules',
   full_name='p2p_validate.Int64Rules',
   filename=None,
@@ -1063,14 +1099,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.Int64Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.Int64Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -1144,17 +1187,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.Int64Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.Int64Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=2837,
-  serialized_end=3389,
+  serialized_start=2927,
+  serialized_end=3509,
 )
 
 
 _UINT32RULES = _descriptor.Descriptor(
   name='UInt32Rules',
   full_name='p2p_validate.UInt32Rules',
   filename=None,
@@ -1291,14 +1339,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.UInt32Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.UInt32Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -1372,17 +1427,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.UInt32Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.UInt32Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=3392,
-  serialized_end=3945,
+  serialized_start=3512,
+  serialized_end=4095,
 )
 
 
 _UINT64RULES = _descriptor.Descriptor(
   name='UInt64Rules',
   full_name='p2p_validate.UInt64Rules',
   filename=None,
@@ -1519,14 +1579,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.UInt64Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.UInt64Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -1600,17 +1667,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.UInt64Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.UInt64Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=3948,
-  serialized_end=4501,
+  serialized_start=4098,
+  serialized_end=4681,
 )
 
 
 _SINT32RULES = _descriptor.Descriptor(
   name='SInt32Rules',
   full_name='p2p_validate.SInt32Rules',
   filename=None,
@@ -1747,14 +1819,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.SInt32Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.SInt32Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -1828,17 +1907,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.SInt32Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.SInt32Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=4504,
-  serialized_end=5057,
+  serialized_start=4684,
+  serialized_end=5267,
 )
 
 
 _SINT64RULES = _descriptor.Descriptor(
   name='SInt64Rules',
   full_name='p2p_validate.SInt64Rules',
   filename=None,
@@ -1975,14 +2059,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.SInt64Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.SInt64Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -2056,17 +2147,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.SInt64Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.SInt64Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=5060,
-  serialized_end=5613,
+  serialized_start=5270,
+  serialized_end=5853,
 )
 
 
 _FIXED32RULES = _descriptor.Descriptor(
   name='Fixed32Rules',
   full_name='p2p_validate.Fixed32Rules',
   filename=None,
@@ -2203,14 +2299,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.Fixed32Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.Fixed32Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -2284,17 +2387,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.Fixed32Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.Fixed32Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=5616,
-  serialized_end=6170,
+  serialized_start=5856,
+  serialized_end=6440,
 )
 
 
 _FIXED64RULES = _descriptor.Descriptor(
   name='Fixed64Rules',
   full_name='p2p_validate.Fixed64Rules',
   filename=None,
@@ -2431,14 +2539,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.Fixed64Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.Fixed64Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -2512,17 +2627,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.Fixed64Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.Fixed64Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=6173,
-  serialized_end=6727,
+  serialized_start=6443,
+  serialized_end=7027,
 )
 
 
 _SFIXED32RULES = _descriptor.Descriptor(
   name='SFixed32Rules',
   full_name='p2p_validate.SFixed32Rules',
   filename=None,
@@ -2659,14 +2779,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.SFixed32Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.SFixed32Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -2740,17 +2867,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.SFixed32Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.SFixed32Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=6730,
-  serialized_end=7285,
+  serialized_start=7030,
+  serialized_end=7615,
 )
 
 
 _SFIXED64RULES = _descriptor.Descriptor(
   name='SFixed64Rules',
   full_name='p2p_validate.SFixed64Rules',
   filename=None,
@@ -2887,14 +3019,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.SFixed64Rules.title', index=18,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.SFixed64Rules.extra', index=19,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -2968,17 +3107,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.SFixed64Rules._title',
       index=13, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.SFixed64Rules._extra',
+      index=14, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=7288,
-  serialized_end=7843,
+  serialized_start=7618,
+  serialized_end=8203,
 )
 
 
 _BOOLRULES = _descriptor.Descriptor(
   name='BoolRules',
   full_name='p2p_validate.BoolRules',
   filename=None,
@@ -3052,14 +3196,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.BoolRules.title', index=9,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.BoolRules.extra', index=10,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -3108,17 +3259,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.BoolRules._title',
       index=8, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.BoolRules._extra',
+      index=9, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=7846,
-  serialized_end=8174,
+  serialized_start=8206,
+  serialized_end=8564,
 )
 
 
 _STRINGRULES = _descriptor.Descriptor(
   name='StringRules',
   full_name='p2p_validate.StringRules',
   filename=None,
@@ -3346,14 +3502,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.StringRules.title', index=31,
       number=34, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.StringRules.extra', index=32,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -3447,17 +3610,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.StringRules._title',
       index=17, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.StringRules._extra',
+      index=18, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=8177,
-  serialized_end=9067,
+  serialized_start=8567,
+  serialized_end=9487,
 )
 
 
 _BYTESRULES = _descriptor.Descriptor(
   name='BytesRules',
   full_name='p2p_validate.BytesRules',
   filename=None,
@@ -3622,14 +3790,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.BytesRules.title', index=22,
       number=24, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.BytesRules.extra', index=23,
+      number=25, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -3713,17 +3888,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.BytesRules._title',
       index=15, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.BytesRules._extra',
+      index=16, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=9070,
-  serialized_end=9766,
+  serialized_start=9490,
+  serialized_end=10216,
 )
 
 
 _ENUMRULES = _descriptor.Descriptor(
   name='EnumRules',
   full_name='p2p_validate.EnumRules',
   filename=None,
@@ -3818,14 +3998,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.EnumRules.title', index=12,
       number=18, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.EnumRules.extra', index=13,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -3869,17 +4056,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.EnumRules._title',
       index=7, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.EnumRules._extra',
+      index=8, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=9769,
-  serialized_end=10154,
+  serialized_start=10219,
+  serialized_end=10634,
 )
 
 
 _MESSAGERULES = _descriptor.Descriptor(
   name='MessageRules',
   full_name='p2p_validate.MessageRules',
   filename=None,
@@ -3974,14 +4166,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.MessageRules.title', index=12,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.MessageRules.extra', index=13,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -4035,17 +4234,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.MessageRules._title',
       index=9, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.MessageRules._extra',
+      index=10, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=10157,
-  serialized_end=10579,
+  serialized_start=10637,
+  serialized_end=11089,
 )
 
 
 _REPEATEDRULES = _descriptor.Descriptor(
   name='RepeatedRules',
   full_name='p2p_validate.RepeatedRules',
   filename=None,
@@ -4140,14 +4344,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.RepeatedRules.title', index=12,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.RepeatedRules.extra', index=13,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -4211,17 +4422,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.RepeatedRules._title',
       index=11, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.RepeatedRules._extra',
+      index=12, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=10582,
-  serialized_end=11067,
+  serialized_start=11092,
+  serialized_end=11607,
 )
 
 
 _MAPRULES = _descriptor.Descriptor(
   name='MapRules',
   full_name='p2p_validate.MapRules',
   filename=None,
@@ -4316,14 +4532,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.MapRules.title', index=12,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.MapRules.extra', index=13,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -4387,17 +4610,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.MapRules._title',
       index=11, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.MapRules._extra',
+      index=12, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=11070,
-  serialized_end=11574,
+  serialized_start=11610,
+  serialized_end=12144,
 )
 
 
 _ANYRULES = _descriptor.Descriptor(
   name='AnyRules',
   full_name='p2p_validate.AnyRules',
   filename=None,
@@ -4492,14 +4720,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.AnyRules.title', index=12,
       number=17, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.AnyRules.extra', index=13,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -4543,17 +4778,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.AnyRules._title',
       index=7, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.AnyRules._extra',
+      index=8, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=11577,
-  serialized_end=11967,
+  serialized_start=12147,
+  serialized_end=12567,
 )
 
 
 _DURATIONRULES = _descriptor.Descriptor(
   name='DurationRules',
   full_name='p2p_validate.DurationRules',
   filename=None,
@@ -4683,14 +4923,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.DurationRules.title', index=17,
       number=19, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.DurationRules.extra', index=18,
+      number=20, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -4759,17 +5006,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.DurationRules._title',
       index=12, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.DurationRules._extra',
+      index=13, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=11970,
-  serialized_end=12726,
+  serialized_start=12570,
+  serialized_end=13356,
 )
 
 
 _TIMESTAMPRULES = _descriptor.Descriptor(
   name='TimestampRules',
   full_name='p2p_validate.TimestampRules',
   filename=None,
@@ -4906,14 +5158,21 @@
     _descriptor.FieldDescriptor(
       name='title', full_name='p2p_validate.TimestampRules.title', index=18,
       number=20, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra', full_name='p2p_validate.TimestampRules.extra', index=19,
+      number=21, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -4997,17 +5256,22 @@
       create_key=_descriptor._internal_create_key,
     fields=[]),
     _descriptor.OneofDescriptor(
       name='_title', full_name='p2p_validate.TimestampRules._title',
       index=15, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
+    _descriptor.OneofDescriptor(
+      name='_extra', full_name='p2p_validate.TimestampRules._extra',
+      index=16, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=12729,
-  serialized_end=13534,
+  serialized_start=13359,
+  serialized_end=14194,
 )
 
 _FIELDRULES.fields_by_name['message'].message_type = _MESSAGERULES
 _FIELDRULES.fields_by_name['float'].message_type = _FLOATRULES
 _FIELDRULES.fields_by_name['double'].message_type = _DOUBLERULES
 _FIELDRULES.fields_by_name['int32'].message_type = _INT32RULES
 _FIELDRULES.fields_by_name['int64'].message_type = _INT64RULES
@@ -5141,14 +5405,17 @@
 _FLOATRULES.fields_by_name['field'].containing_oneof = _FLOATRULES.oneofs_by_name['_field']
 _FLOATRULES.oneofs_by_name['_type'].fields.append(
   _FLOATRULES.fields_by_name['type'])
 _FLOATRULES.fields_by_name['type'].containing_oneof = _FLOATRULES.oneofs_by_name['_type']
 _FLOATRULES.oneofs_by_name['_title'].fields.append(
   _FLOATRULES.fields_by_name['title'])
 _FLOATRULES.fields_by_name['title'].containing_oneof = _FLOATRULES.oneofs_by_name['_title']
+_FLOATRULES.oneofs_by_name['_extra'].fields.append(
+  _FLOATRULES.fields_by_name['extra'])
+_FLOATRULES.fields_by_name['extra'].containing_oneof = _FLOATRULES.oneofs_by_name['_extra']
 _DOUBLERULES.oneofs_by_name['default_config'].fields.append(
   _DOUBLERULES.fields_by_name['default'])
 _DOUBLERULES.fields_by_name['default'].containing_oneof = _DOUBLERULES.oneofs_by_name['default_config']
 _DOUBLERULES.oneofs_by_name['default_config'].fields.append(
   _DOUBLERULES.fields_by_name['default_factory'])
 _DOUBLERULES.fields_by_name['default_factory'].containing_oneof = _DOUBLERULES.oneofs_by_name['default_config']
 _DOUBLERULES.oneofs_by_name['default_config'].fields.append(
@@ -5192,14 +5459,17 @@
 _DOUBLERULES.fields_by_name['field'].containing_oneof = _DOUBLERULES.oneofs_by_name['_field']
 _DOUBLERULES.oneofs_by_name['_type'].fields.append(
   _DOUBLERULES.fields_by_name['type'])
 _DOUBLERULES.fields_by_name['type'].containing_oneof = _DOUBLERULES.oneofs_by_name['_type']
 _DOUBLERULES.oneofs_by_name['_title'].fields.append(
   _DOUBLERULES.fields_by_name['title'])
 _DOUBLERULES.fields_by_name['title'].containing_oneof = _DOUBLERULES.oneofs_by_name['_title']
+_DOUBLERULES.oneofs_by_name['_extra'].fields.append(
+  _DOUBLERULES.fields_by_name['extra'])
+_DOUBLERULES.fields_by_name['extra'].containing_oneof = _DOUBLERULES.oneofs_by_name['_extra']
 _INT32RULES.oneofs_by_name['default_config'].fields.append(
   _INT32RULES.fields_by_name['default'])
 _INT32RULES.fields_by_name['default'].containing_oneof = _INT32RULES.oneofs_by_name['default_config']
 _INT32RULES.oneofs_by_name['default_config'].fields.append(
   _INT32RULES.fields_by_name['default_factory'])
 _INT32RULES.fields_by_name['default_factory'].containing_oneof = _INT32RULES.oneofs_by_name['default_config']
 _INT32RULES.oneofs_by_name['default_config'].fields.append(
@@ -5243,14 +5513,17 @@
 _INT32RULES.fields_by_name['field'].containing_oneof = _INT32RULES.oneofs_by_name['_field']
 _INT32RULES.oneofs_by_name['_type'].fields.append(
   _INT32RULES.fields_by_name['type'])
 _INT32RULES.fields_by_name['type'].containing_oneof = _INT32RULES.oneofs_by_name['_type']
 _INT32RULES.oneofs_by_name['_title'].fields.append(
   _INT32RULES.fields_by_name['title'])
 _INT32RULES.fields_by_name['title'].containing_oneof = _INT32RULES.oneofs_by_name['_title']
+_INT32RULES.oneofs_by_name['_extra'].fields.append(
+  _INT32RULES.fields_by_name['extra'])
+_INT32RULES.fields_by_name['extra'].containing_oneof = _INT32RULES.oneofs_by_name['_extra']
 _INT64RULES.oneofs_by_name['default_config'].fields.append(
   _INT64RULES.fields_by_name['default'])
 _INT64RULES.fields_by_name['default'].containing_oneof = _INT64RULES.oneofs_by_name['default_config']
 _INT64RULES.oneofs_by_name['default_config'].fields.append(
   _INT64RULES.fields_by_name['default_factory'])
 _INT64RULES.fields_by_name['default_factory'].containing_oneof = _INT64RULES.oneofs_by_name['default_config']
 _INT64RULES.oneofs_by_name['default_config'].fields.append(
@@ -5294,14 +5567,17 @@
 _INT64RULES.fields_by_name['field'].containing_oneof = _INT64RULES.oneofs_by_name['_field']
 _INT64RULES.oneofs_by_name['_type'].fields.append(
   _INT64RULES.fields_by_name['type'])
 _INT64RULES.fields_by_name['type'].containing_oneof = _INT64RULES.oneofs_by_name['_type']
 _INT64RULES.oneofs_by_name['_title'].fields.append(
   _INT64RULES.fields_by_name['title'])
 _INT64RULES.fields_by_name['title'].containing_oneof = _INT64RULES.oneofs_by_name['_title']
+_INT64RULES.oneofs_by_name['_extra'].fields.append(
+  _INT64RULES.fields_by_name['extra'])
+_INT64RULES.fields_by_name['extra'].containing_oneof = _INT64RULES.oneofs_by_name['_extra']
 _UINT32RULES.oneofs_by_name['default_config'].fields.append(
   _UINT32RULES.fields_by_name['default'])
 _UINT32RULES.fields_by_name['default'].containing_oneof = _UINT32RULES.oneofs_by_name['default_config']
 _UINT32RULES.oneofs_by_name['default_config'].fields.append(
   _UINT32RULES.fields_by_name['default_factory'])
 _UINT32RULES.fields_by_name['default_factory'].containing_oneof = _UINT32RULES.oneofs_by_name['default_config']
 _UINT32RULES.oneofs_by_name['default_config'].fields.append(
@@ -5345,14 +5621,17 @@
 _UINT32RULES.fields_by_name['field'].containing_oneof = _UINT32RULES.oneofs_by_name['_field']
 _UINT32RULES.oneofs_by_name['_type'].fields.append(
   _UINT32RULES.fields_by_name['type'])
 _UINT32RULES.fields_by_name['type'].containing_oneof = _UINT32RULES.oneofs_by_name['_type']
 _UINT32RULES.oneofs_by_name['_title'].fields.append(
   _UINT32RULES.fields_by_name['title'])
 _UINT32RULES.fields_by_name['title'].containing_oneof = _UINT32RULES.oneofs_by_name['_title']
+_UINT32RULES.oneofs_by_name['_extra'].fields.append(
+  _UINT32RULES.fields_by_name['extra'])
+_UINT32RULES.fields_by_name['extra'].containing_oneof = _UINT32RULES.oneofs_by_name['_extra']
 _UINT64RULES.oneofs_by_name['default_config'].fields.append(
   _UINT64RULES.fields_by_name['default'])
 _UINT64RULES.fields_by_name['default'].containing_oneof = _UINT64RULES.oneofs_by_name['default_config']
 _UINT64RULES.oneofs_by_name['default_config'].fields.append(
   _UINT64RULES.fields_by_name['default_factory'])
 _UINT64RULES.fields_by_name['default_factory'].containing_oneof = _UINT64RULES.oneofs_by_name['default_config']
 _UINT64RULES.oneofs_by_name['default_config'].fields.append(
@@ -5396,14 +5675,17 @@
 _UINT64RULES.fields_by_name['field'].containing_oneof = _UINT64RULES.oneofs_by_name['_field']
 _UINT64RULES.oneofs_by_name['_type'].fields.append(
   _UINT64RULES.fields_by_name['type'])
 _UINT64RULES.fields_by_name['type'].containing_oneof = _UINT64RULES.oneofs_by_name['_type']
 _UINT64RULES.oneofs_by_name['_title'].fields.append(
   _UINT64RULES.fields_by_name['title'])
 _UINT64RULES.fields_by_name['title'].containing_oneof = _UINT64RULES.oneofs_by_name['_title']
+_UINT64RULES.oneofs_by_name['_extra'].fields.append(
+  _UINT64RULES.fields_by_name['extra'])
+_UINT64RULES.fields_by_name['extra'].containing_oneof = _UINT64RULES.oneofs_by_name['_extra']
 _SINT32RULES.oneofs_by_name['default_config'].fields.append(
   _SINT32RULES.fields_by_name['default'])
 _SINT32RULES.fields_by_name['default'].containing_oneof = _SINT32RULES.oneofs_by_name['default_config']
 _SINT32RULES.oneofs_by_name['default_config'].fields.append(
   _SINT32RULES.fields_by_name['default_factory'])
 _SINT32RULES.fields_by_name['default_factory'].containing_oneof = _SINT32RULES.oneofs_by_name['default_config']
 _SINT32RULES.oneofs_by_name['default_config'].fields.append(
@@ -5447,14 +5729,17 @@
 _SINT32RULES.fields_by_name['field'].containing_oneof = _SINT32RULES.oneofs_by_name['_field']
 _SINT32RULES.oneofs_by_name['_type'].fields.append(
   _SINT32RULES.fields_by_name['type'])
 _SINT32RULES.fields_by_name['type'].containing_oneof = _SINT32RULES.oneofs_by_name['_type']
 _SINT32RULES.oneofs_by_name['_title'].fields.append(
   _SINT32RULES.fields_by_name['title'])
 _SINT32RULES.fields_by_name['title'].containing_oneof = _SINT32RULES.oneofs_by_name['_title']
+_SINT32RULES.oneofs_by_name['_extra'].fields.append(
+  _SINT32RULES.fields_by_name['extra'])
+_SINT32RULES.fields_by_name['extra'].containing_oneof = _SINT32RULES.oneofs_by_name['_extra']
 _SINT64RULES.oneofs_by_name['default_config'].fields.append(
   _SINT64RULES.fields_by_name['default'])
 _SINT64RULES.fields_by_name['default'].containing_oneof = _SINT64RULES.oneofs_by_name['default_config']
 _SINT64RULES.oneofs_by_name['default_config'].fields.append(
   _SINT64RULES.fields_by_name['default_factory'])
 _SINT64RULES.fields_by_name['default_factory'].containing_oneof = _SINT64RULES.oneofs_by_name['default_config']
 _SINT64RULES.oneofs_by_name['default_config'].fields.append(
@@ -5498,14 +5783,17 @@
 _SINT64RULES.fields_by_name['field'].containing_oneof = _SINT64RULES.oneofs_by_name['_field']
 _SINT64RULES.oneofs_by_name['_type'].fields.append(
   _SINT64RULES.fields_by_name['type'])
 _SINT64RULES.fields_by_name['type'].containing_oneof = _SINT64RULES.oneofs_by_name['_type']
 _SINT64RULES.oneofs_by_name['_title'].fields.append(
   _SINT64RULES.fields_by_name['title'])
 _SINT64RULES.fields_by_name['title'].containing_oneof = _SINT64RULES.oneofs_by_name['_title']
+_SINT64RULES.oneofs_by_name['_extra'].fields.append(
+  _SINT64RULES.fields_by_name['extra'])
+_SINT64RULES.fields_by_name['extra'].containing_oneof = _SINT64RULES.oneofs_by_name['_extra']
 _FIXED32RULES.oneofs_by_name['default_config'].fields.append(
   _FIXED32RULES.fields_by_name['default'])
 _FIXED32RULES.fields_by_name['default'].containing_oneof = _FIXED32RULES.oneofs_by_name['default_config']
 _FIXED32RULES.oneofs_by_name['default_config'].fields.append(
   _FIXED32RULES.fields_by_name['default_factory'])
 _FIXED32RULES.fields_by_name['default_factory'].containing_oneof = _FIXED32RULES.oneofs_by_name['default_config']
 _FIXED32RULES.oneofs_by_name['default_config'].fields.append(
@@ -5549,14 +5837,17 @@
 _FIXED32RULES.fields_by_name['field'].containing_oneof = _FIXED32RULES.oneofs_by_name['_field']
 _FIXED32RULES.oneofs_by_name['_type'].fields.append(
   _FIXED32RULES.fields_by_name['type'])
 _FIXED32RULES.fields_by_name['type'].containing_oneof = _FIXED32RULES.oneofs_by_name['_type']
 _FIXED32RULES.oneofs_by_name['_title'].fields.append(
   _FIXED32RULES.fields_by_name['title'])
 _FIXED32RULES.fields_by_name['title'].containing_oneof = _FIXED32RULES.oneofs_by_name['_title']
+_FIXED32RULES.oneofs_by_name['_extra'].fields.append(
+  _FIXED32RULES.fields_by_name['extra'])
+_FIXED32RULES.fields_by_name['extra'].containing_oneof = _FIXED32RULES.oneofs_by_name['_extra']
 _FIXED64RULES.oneofs_by_name['default_config'].fields.append(
   _FIXED64RULES.fields_by_name['default'])
 _FIXED64RULES.fields_by_name['default'].containing_oneof = _FIXED64RULES.oneofs_by_name['default_config']
 _FIXED64RULES.oneofs_by_name['default_config'].fields.append(
   _FIXED64RULES.fields_by_name['default_factory'])
 _FIXED64RULES.fields_by_name['default_factory'].containing_oneof = _FIXED64RULES.oneofs_by_name['default_config']
 _FIXED64RULES.oneofs_by_name['default_config'].fields.append(
@@ -5600,14 +5891,17 @@
 _FIXED64RULES.fields_by_name['field'].containing_oneof = _FIXED64RULES.oneofs_by_name['_field']
 _FIXED64RULES.oneofs_by_name['_type'].fields.append(
   _FIXED64RULES.fields_by_name['type'])
 _FIXED64RULES.fields_by_name['type'].containing_oneof = _FIXED64RULES.oneofs_by_name['_type']
 _FIXED64RULES.oneofs_by_name['_title'].fields.append(
   _FIXED64RULES.fields_by_name['title'])
 _FIXED64RULES.fields_by_name['title'].containing_oneof = _FIXED64RULES.oneofs_by_name['_title']
+_FIXED64RULES.oneofs_by_name['_extra'].fields.append(
+  _FIXED64RULES.fields_by_name['extra'])
+_FIXED64RULES.fields_by_name['extra'].containing_oneof = _FIXED64RULES.oneofs_by_name['_extra']
 _SFIXED32RULES.oneofs_by_name['default_config'].fields.append(
   _SFIXED32RULES.fields_by_name['default'])
 _SFIXED32RULES.fields_by_name['default'].containing_oneof = _SFIXED32RULES.oneofs_by_name['default_config']
 _SFIXED32RULES.oneofs_by_name['default_config'].fields.append(
   _SFIXED32RULES.fields_by_name['default_factory'])
 _SFIXED32RULES.fields_by_name['default_factory'].containing_oneof = _SFIXED32RULES.oneofs_by_name['default_config']
 _SFIXED32RULES.oneofs_by_name['default_config'].fields.append(
@@ -5651,14 +5945,17 @@
 _SFIXED32RULES.fields_by_name['field'].containing_oneof = _SFIXED32RULES.oneofs_by_name['_field']
 _SFIXED32RULES.oneofs_by_name['_type'].fields.append(
   _SFIXED32RULES.fields_by_name['type'])
 _SFIXED32RULES.fields_by_name['type'].containing_oneof = _SFIXED32RULES.oneofs_by_name['_type']
 _SFIXED32RULES.oneofs_by_name['_title'].fields.append(
   _SFIXED32RULES.fields_by_name['title'])
 _SFIXED32RULES.fields_by_name['title'].containing_oneof = _SFIXED32RULES.oneofs_by_name['_title']
+_SFIXED32RULES.oneofs_by_name['_extra'].fields.append(
+  _SFIXED32RULES.fields_by_name['extra'])
+_SFIXED32RULES.fields_by_name['extra'].containing_oneof = _SFIXED32RULES.oneofs_by_name['_extra']
 _SFIXED64RULES.oneofs_by_name['default_config'].fields.append(
   _SFIXED64RULES.fields_by_name['default'])
 _SFIXED64RULES.fields_by_name['default'].containing_oneof = _SFIXED64RULES.oneofs_by_name['default_config']
 _SFIXED64RULES.oneofs_by_name['default_config'].fields.append(
   _SFIXED64RULES.fields_by_name['default_factory'])
 _SFIXED64RULES.fields_by_name['default_factory'].containing_oneof = _SFIXED64RULES.oneofs_by_name['default_config']
 _SFIXED64RULES.oneofs_by_name['default_config'].fields.append(
@@ -5702,14 +5999,17 @@
 _SFIXED64RULES.fields_by_name['field'].containing_oneof = _SFIXED64RULES.oneofs_by_name['_field']
 _SFIXED64RULES.oneofs_by_name['_type'].fields.append(
   _SFIXED64RULES.fields_by_name['type'])
 _SFIXED64RULES.fields_by_name['type'].containing_oneof = _SFIXED64RULES.oneofs_by_name['_type']
 _SFIXED64RULES.oneofs_by_name['_title'].fields.append(
   _SFIXED64RULES.fields_by_name['title'])
 _SFIXED64RULES.fields_by_name['title'].containing_oneof = _SFIXED64RULES.oneofs_by_name['_title']
+_SFIXED64RULES.oneofs_by_name['_extra'].fields.append(
+  _SFIXED64RULES.fields_by_name['extra'])
+_SFIXED64RULES.fields_by_name['extra'].containing_oneof = _SFIXED64RULES.oneofs_by_name['_extra']
 _BOOLRULES.oneofs_by_name['default_config'].fields.append(
   _BOOLRULES.fields_by_name['default'])
 _BOOLRULES.fields_by_name['default'].containing_oneof = _BOOLRULES.oneofs_by_name['default_config']
 _BOOLRULES.oneofs_by_name['default_config'].fields.append(
   _BOOLRULES.fields_by_name['miss_default'])
 _BOOLRULES.fields_by_name['miss_default'].containing_oneof = _BOOLRULES.oneofs_by_name['default_config']
 _BOOLRULES.oneofs_by_name['_const'].fields.append(
@@ -5732,14 +6032,17 @@
 _BOOLRULES.fields_by_name['field'].containing_oneof = _BOOLRULES.oneofs_by_name['_field']
 _BOOLRULES.oneofs_by_name['_type'].fields.append(
   _BOOLRULES.fields_by_name['type'])
 _BOOLRULES.fields_by_name['type'].containing_oneof = _BOOLRULES.oneofs_by_name['_type']
 _BOOLRULES.oneofs_by_name['_title'].fields.append(
   _BOOLRULES.fields_by_name['title'])
 _BOOLRULES.fields_by_name['title'].containing_oneof = _BOOLRULES.oneofs_by_name['_title']
+_BOOLRULES.oneofs_by_name['_extra'].fields.append(
+  _BOOLRULES.fields_by_name['extra'])
+_BOOLRULES.fields_by_name['extra'].containing_oneof = _BOOLRULES.oneofs_by_name['_extra']
 _STRINGRULES.oneofs_by_name['well_known'].fields.append(
   _STRINGRULES.fields_by_name['email'])
 _STRINGRULES.fields_by_name['email'].containing_oneof = _STRINGRULES.oneofs_by_name['well_known']
 _STRINGRULES.oneofs_by_name['well_known'].fields.append(
   _STRINGRULES.fields_by_name['hostname'])
 _STRINGRULES.fields_by_name['hostname'].containing_oneof = _STRINGRULES.oneofs_by_name['well_known']
 _STRINGRULES.oneofs_by_name['well_known'].fields.append(
@@ -5822,14 +6125,17 @@
 _STRINGRULES.fields_by_name['field'].containing_oneof = _STRINGRULES.oneofs_by_name['_field']
 _STRINGRULES.oneofs_by_name['_type'].fields.append(
   _STRINGRULES.fields_by_name['type'])
 _STRINGRULES.fields_by_name['type'].containing_oneof = _STRINGRULES.oneofs_by_name['_type']
 _STRINGRULES.oneofs_by_name['_title'].fields.append(
   _STRINGRULES.fields_by_name['title'])
 _STRINGRULES.fields_by_name['title'].containing_oneof = _STRINGRULES.oneofs_by_name['_title']
+_STRINGRULES.oneofs_by_name['_extra'].fields.append(
+  _STRINGRULES.fields_by_name['extra'])
+_STRINGRULES.fields_by_name['extra'].containing_oneof = _STRINGRULES.oneofs_by_name['_extra']
 _BYTESRULES.oneofs_by_name['default_config'].fields.append(
   _BYTESRULES.fields_by_name['default'])
 _BYTESRULES.fields_by_name['default'].containing_oneof = _BYTESRULES.oneofs_by_name['default_config']
 _BYTESRULES.oneofs_by_name['default_config'].fields.append(
   _BYTESRULES.fields_by_name['default_factory'])
 _BYTESRULES.fields_by_name['default_factory'].containing_oneof = _BYTESRULES.oneofs_by_name['default_config']
 _BYTESRULES.oneofs_by_name['default_config'].fields.append(
@@ -5885,14 +6191,17 @@
 _BYTESRULES.fields_by_name['field'].containing_oneof = _BYTESRULES.oneofs_by_name['_field']
 _BYTESRULES.oneofs_by_name['_type'].fields.append(
   _BYTESRULES.fields_by_name['type'])
 _BYTESRULES.fields_by_name['type'].containing_oneof = _BYTESRULES.oneofs_by_name['_type']
 _BYTESRULES.oneofs_by_name['_title'].fields.append(
   _BYTESRULES.fields_by_name['title'])
 _BYTESRULES.fields_by_name['title'].containing_oneof = _BYTESRULES.oneofs_by_name['_title']
+_BYTESRULES.oneofs_by_name['_extra'].fields.append(
+  _BYTESRULES.fields_by_name['extra'])
+_BYTESRULES.fields_by_name['extra'].containing_oneof = _BYTESRULES.oneofs_by_name['_extra']
 _ENUMRULES.oneofs_by_name['default_config'].fields.append(
   _ENUMRULES.fields_by_name['default'])
 _ENUMRULES.fields_by_name['default'].containing_oneof = _ENUMRULES.oneofs_by_name['default_config']
 _ENUMRULES.oneofs_by_name['default_config'].fields.append(
   _ENUMRULES.fields_by_name['default_factory'])
 _ENUMRULES.fields_by_name['default_factory'].containing_oneof = _ENUMRULES.oneofs_by_name['default_config']
 _ENUMRULES.oneofs_by_name['default_config'].fields.append(
@@ -5918,14 +6227,17 @@
 _ENUMRULES.fields_by_name['description'].containing_oneof = _ENUMRULES.oneofs_by_name['_description']
 _ENUMRULES.oneofs_by_name['_field'].fields.append(
   _ENUMRULES.fields_by_name['field'])
 _ENUMRULES.fields_by_name['field'].containing_oneof = _ENUMRULES.oneofs_by_name['_field']
 _ENUMRULES.oneofs_by_name['_title'].fields.append(
   _ENUMRULES.fields_by_name['title'])
 _ENUMRULES.fields_by_name['title'].containing_oneof = _ENUMRULES.oneofs_by_name['_title']
+_ENUMRULES.oneofs_by_name['_extra'].fields.append(
+  _ENUMRULES.fields_by_name['extra'])
+_ENUMRULES.fields_by_name['extra'].containing_oneof = _ENUMRULES.oneofs_by_name['_extra']
 _MESSAGERULES.oneofs_by_name['default_config'].fields.append(
   _MESSAGERULES.fields_by_name['default'])
 _MESSAGERULES.fields_by_name['default'].containing_oneof = _MESSAGERULES.oneofs_by_name['default_config']
 _MESSAGERULES.oneofs_by_name['default_config'].fields.append(
   _MESSAGERULES.fields_by_name['default_factory'])
 _MESSAGERULES.fields_by_name['default_factory'].containing_oneof = _MESSAGERULES.oneofs_by_name['default_config']
 _MESSAGERULES.oneofs_by_name['default_config'].fields.append(
@@ -5957,14 +6269,17 @@
 _MESSAGERULES.fields_by_name['field'].containing_oneof = _MESSAGERULES.oneofs_by_name['_field']
 _MESSAGERULES.oneofs_by_name['_type'].fields.append(
   _MESSAGERULES.fields_by_name['type'])
 _MESSAGERULES.fields_by_name['type'].containing_oneof = _MESSAGERULES.oneofs_by_name['_type']
 _MESSAGERULES.oneofs_by_name['_title'].fields.append(
   _MESSAGERULES.fields_by_name['title'])
 _MESSAGERULES.fields_by_name['title'].containing_oneof = _MESSAGERULES.oneofs_by_name['_title']
+_MESSAGERULES.oneofs_by_name['_extra'].fields.append(
+  _MESSAGERULES.fields_by_name['extra'])
+_MESSAGERULES.fields_by_name['extra'].containing_oneof = _MESSAGERULES.oneofs_by_name['_extra']
 _REPEATEDRULES.fields_by_name['items'].message_type = _FIELDRULES
 _REPEATEDRULES.oneofs_by_name['default_config'].fields.append(
   _REPEATEDRULES.fields_by_name['default_factory'])
 _REPEATEDRULES.fields_by_name['default_factory'].containing_oneof = _REPEATEDRULES.oneofs_by_name['default_config']
 _REPEATEDRULES.oneofs_by_name['default_config'].fields.append(
   _REPEATEDRULES.fields_by_name['miss_default'])
 _REPEATEDRULES.fields_by_name['miss_default'].containing_oneof = _REPEATEDRULES.oneofs_by_name['default_config']
@@ -5997,14 +6312,17 @@
 _REPEATEDRULES.fields_by_name['field'].containing_oneof = _REPEATEDRULES.oneofs_by_name['_field']
 _REPEATEDRULES.oneofs_by_name['_type'].fields.append(
   _REPEATEDRULES.fields_by_name['type'])
 _REPEATEDRULES.fields_by_name['type'].containing_oneof = _REPEATEDRULES.oneofs_by_name['_type']
 _REPEATEDRULES.oneofs_by_name['_title'].fields.append(
   _REPEATEDRULES.fields_by_name['title'])
 _REPEATEDRULES.fields_by_name['title'].containing_oneof = _REPEATEDRULES.oneofs_by_name['_title']
+_REPEATEDRULES.oneofs_by_name['_extra'].fields.append(
+  _REPEATEDRULES.fields_by_name['extra'])
+_REPEATEDRULES.fields_by_name['extra'].containing_oneof = _REPEATEDRULES.oneofs_by_name['_extra']
 _MAPRULES.fields_by_name['keys'].message_type = _FIELDRULES
 _MAPRULES.fields_by_name['values'].message_type = _FIELDRULES
 _MAPRULES.oneofs_by_name['default_config'].fields.append(
   _MAPRULES.fields_by_name['default_factory'])
 _MAPRULES.fields_by_name['default_factory'].containing_oneof = _MAPRULES.oneofs_by_name['default_config']
 _MAPRULES.oneofs_by_name['default_config'].fields.append(
   _MAPRULES.fields_by_name['miss_default'])
@@ -6038,14 +6356,17 @@
 _MAPRULES.fields_by_name['field'].containing_oneof = _MAPRULES.oneofs_by_name['_field']
 _MAPRULES.oneofs_by_name['_type'].fields.append(
   _MAPRULES.fields_by_name['type'])
 _MAPRULES.fields_by_name['type'].containing_oneof = _MAPRULES.oneofs_by_name['_type']
 _MAPRULES.oneofs_by_name['_title'].fields.append(
   _MAPRULES.fields_by_name['title'])
 _MAPRULES.fields_by_name['title'].containing_oneof = _MAPRULES.oneofs_by_name['_title']
+_MAPRULES.oneofs_by_name['_extra'].fields.append(
+  _MAPRULES.fields_by_name['extra'])
+_MAPRULES.fields_by_name['extra'].containing_oneof = _MAPRULES.oneofs_by_name['_extra']
 _ANYRULES.oneofs_by_name['default_config'].fields.append(
   _ANYRULES.fields_by_name['default'])
 _ANYRULES.fields_by_name['default'].containing_oneof = _ANYRULES.oneofs_by_name['default_config']
 _ANYRULES.oneofs_by_name['default_config'].fields.append(
   _ANYRULES.fields_by_name['default_factory'])
 _ANYRULES.fields_by_name['default_factory'].containing_oneof = _ANYRULES.oneofs_by_name['default_config']
 _ANYRULES.oneofs_by_name['default_config'].fields.append(
@@ -6071,14 +6392,17 @@
 _ANYRULES.fields_by_name['description'].containing_oneof = _ANYRULES.oneofs_by_name['_description']
 _ANYRULES.oneofs_by_name['_field'].fields.append(
   _ANYRULES.fields_by_name['field'])
 _ANYRULES.fields_by_name['field'].containing_oneof = _ANYRULES.oneofs_by_name['_field']
 _ANYRULES.oneofs_by_name['_title'].fields.append(
   _ANYRULES.fields_by_name['title'])
 _ANYRULES.fields_by_name['title'].containing_oneof = _ANYRULES.oneofs_by_name['_title']
+_ANYRULES.oneofs_by_name['_extra'].fields.append(
+  _ANYRULES.fields_by_name['extra'])
+_ANYRULES.fields_by_name['extra'].containing_oneof = _ANYRULES.oneofs_by_name['_extra']
 _DURATIONRULES.fields_by_name['const'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _DURATIONRULES.fields_by_name['lt'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _DURATIONRULES.fields_by_name['le'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _DURATIONRULES.fields_by_name['gt'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _DURATIONRULES.fields_by_name['ge'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _DURATIONRULES.fields_by_name['in'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _DURATIONRULES.fields_by_name['not_in'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
@@ -6128,14 +6452,17 @@
 _DURATIONRULES.fields_by_name['field'].containing_oneof = _DURATIONRULES.oneofs_by_name['_field']
 _DURATIONRULES.oneofs_by_name['_type'].fields.append(
   _DURATIONRULES.fields_by_name['type'])
 _DURATIONRULES.fields_by_name['type'].containing_oneof = _DURATIONRULES.oneofs_by_name['_type']
 _DURATIONRULES.oneofs_by_name['_title'].fields.append(
   _DURATIONRULES.fields_by_name['title'])
 _DURATIONRULES.fields_by_name['title'].containing_oneof = _DURATIONRULES.oneofs_by_name['_title']
+_DURATIONRULES.oneofs_by_name['_extra'].fields.append(
+  _DURATIONRULES.fields_by_name['extra'])
+_DURATIONRULES.fields_by_name['extra'].containing_oneof = _DURATIONRULES.oneofs_by_name['_extra']
 _TIMESTAMPRULES.fields_by_name['const'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _TIMESTAMPRULES.fields_by_name['lt'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _TIMESTAMPRULES.fields_by_name['le'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _TIMESTAMPRULES.fields_by_name['gt'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _TIMESTAMPRULES.fields_by_name['ge'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _TIMESTAMPRULES.fields_by_name['within'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _TIMESTAMPRULES.fields_by_name['default'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
@@ -6193,14 +6520,17 @@
 _TIMESTAMPRULES.fields_by_name['field'].containing_oneof = _TIMESTAMPRULES.oneofs_by_name['_field']
 _TIMESTAMPRULES.oneofs_by_name['_type'].fields.append(
   _TIMESTAMPRULES.fields_by_name['type'])
 _TIMESTAMPRULES.fields_by_name['type'].containing_oneof = _TIMESTAMPRULES.oneofs_by_name['_type']
 _TIMESTAMPRULES.oneofs_by_name['_title'].fields.append(
   _TIMESTAMPRULES.fields_by_name['title'])
 _TIMESTAMPRULES.fields_by_name['title'].containing_oneof = _TIMESTAMPRULES.oneofs_by_name['_title']
+_TIMESTAMPRULES.oneofs_by_name['_extra'].fields.append(
+  _TIMESTAMPRULES.fields_by_name['extra'])
+_TIMESTAMPRULES.fields_by_name['extra'].containing_oneof = _TIMESTAMPRULES.oneofs_by_name['_extra']
 DESCRIPTOR.message_types_by_name['FieldRules'] = _FIELDRULES
 DESCRIPTOR.message_types_by_name['FloatRules'] = _FLOATRULES
 DESCRIPTOR.message_types_by_name['DoubleRules'] = _DOUBLERULES
 DESCRIPTOR.message_types_by_name['Int32Rules'] = _INT32RULES
 DESCRIPTOR.message_types_by_name['Int64Rules'] = _INT64RULES
 DESCRIPTOR.message_types_by_name['UInt32Rules'] = _UINT32RULES
 DESCRIPTOR.message_types_by_name['UInt64Rules'] = _UINT64RULES
```

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -152,14 +152,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.float
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.float
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.float
@@ -205,14 +206,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.float | None = ...,
         lt: builtins.float | None = ...,
         le: builtins.float | None = ...,
         gt: builtins.float | None = ...,
@@ -226,26 +229,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -284,14 +290,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.float
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.float
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.float
@@ -337,14 +344,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.float | None = ...,
         lt: builtins.float | None = ...,
         le: builtins.float | None = ...,
         gt: builtins.float | None = ...,
@@ -358,26 +367,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -416,14 +428,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -469,14 +482,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -490,26 +505,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -548,14 +566,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -601,14 +620,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -622,26 +643,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -680,14 +704,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -733,14 +758,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -754,26 +781,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -812,14 +842,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -865,14 +896,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -886,26 +919,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -944,14 +980,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -997,14 +1034,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1018,26 +1057,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1076,14 +1118,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1129,14 +1172,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1150,26 +1195,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1208,14 +1256,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1261,14 +1310,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1282,26 +1333,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1340,14 +1394,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1393,14 +1448,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1414,26 +1471,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1472,14 +1532,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1525,14 +1586,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1546,26 +1609,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1604,14 +1670,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1657,14 +1724,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1678,26 +1747,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1727,14 +1799,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.bool
     """Const specifies that this field must be exactly the specified value"""
     enable: builtins.bool
     """Whether to enable this field, if not, the generated Model will not carry this field"""
     default: builtins.bool
     """The default value corresponding to the field, if not set,
     the default value is the default value of the corresponding type of the field
@@ -1749,41 +1822,46 @@
     """Set the corresponding sample value"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.bool | None = ...,
         enable: builtins.bool | None = ...,
         default: builtins.bool = ...,
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.bool | None = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_example", b"_example", "_field", b"_field", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "description", b"description", "enable", b"enable", "example", b"example", "field", b"field", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_example", b"_example", "_field", b"_field", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "description", b"description", "enable", b"enable", "example", b"example", "field", b"field", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_example", b"_example", "_extra", b"_extra", "_field", b"_field", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "description", b"description", "enable", b"enable", "example", b"example", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_example", b"_example", "_extra", b"_extra", "_field", b"_field", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "description", b"description", "enable", b"enable", "example", b"example", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_example", b"_example"]) -> typing_extensions.Literal["example"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_title", b"_title"]) -> typing_extensions.Literal["title"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_type", b"_type"]) -> typing_extensions.Literal["type"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["default_config", b"default_config"]) -> typing_extensions.Literal["default", "miss_default"] | None: ...
@@ -1823,14 +1901,15 @@
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.str
     """Const specifies that this field must be exactly the specified value"""
     len: builtins.int
     """Len specifies that this field must be the specified number of
     characters (Unicode code points). Note that the number of
     characters may differ from the number of bytes in the string.
     """
@@ -1933,14 +2012,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.str | None = ...,
         len: builtins.int | None = ...,
         min_length: builtins.int | None = ...,
         max_length: builtins.int | None = ...,
@@ -1967,28 +2048,31 @@
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.str = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_len", b"_len", "_max_length", b"_max_length", "_min_length", b"_min_length", "_not_contains", b"_not_contains", "_pattern", b"_pattern", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "address", b"address", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "email", b"email", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "hostname", b"hostname", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "len", b"len", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "not_contains", b"not_contains", "pattern", b"pattern", "prefix", b"prefix", "pydantic_type", b"pydantic_type", "suffix", b"suffix", "title", b"title", "type", b"type", "uri", b"uri", "uri_ref", b"uri_ref", "uuid", b"uuid", "well_known", b"well_known"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_len", b"_len", "_max_length", b"_max_length", "_min_length", b"_min_length", "_not_contains", b"_not_contains", "_pattern", b"_pattern", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "address", b"address", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "email", b"email", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "hostname", b"hostname", "in", b"in", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "len", b"len", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "not_contains", b"not_contains", "not_in", b"not_in", "pattern", b"pattern", "prefix", b"prefix", "pydantic_type", b"pydantic_type", "suffix", b"suffix", "title", b"title", "type", b"type", "uri", b"uri", "uri_ref", b"uri_ref", "uuid", b"uuid", "well_known", b"well_known"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_len", b"_len", "_max_length", b"_max_length", "_min_length", b"_min_length", "_not_contains", b"_not_contains", "_pattern", b"_pattern", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "address", b"address", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "email", b"email", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "hostname", b"hostname", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "len", b"len", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "not_contains", b"not_contains", "pattern", b"pattern", "prefix", b"prefix", "pydantic_type", b"pydantic_type", "suffix", b"suffix", "title", b"title", "type", b"type", "uri", b"uri", "uri_ref", b"uri_ref", "uuid", b"uuid", "well_known", b"well_known"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_len", b"_len", "_max_length", b"_max_length", "_min_length", b"_min_length", "_not_contains", b"_not_contains", "_pattern", b"_pattern", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "address", b"address", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "email", b"email", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "hostname", b"hostname", "in", b"in", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "len", b"len", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "not_contains", b"not_contains", "not_in", b"not_in", "pattern", b"pattern", "prefix", b"prefix", "pydantic_type", b"pydantic_type", "suffix", b"suffix", "title", b"title", "type", b"type", "uri", b"uri", "uri_ref", b"uri_ref", "uuid", b"uuid", "well_known", b"well_known"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_contains", b"_contains"]) -> typing_extensions.Literal["contains"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_len", b"_len"]) -> typing_extensions.Literal["len"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_max_length", b"_max_length"]) -> typing_extensions.Literal["max_length"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_min_length", b"_min_length"]) -> typing_extensions.Literal["min_length"] | None: ...
@@ -2037,14 +2121,15 @@
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     IP_FIELD_NUMBER: builtins.int
     IPV4_FIELD_NUMBER: builtins.int
     IPV6_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.bytes
     """Const specifies that this field must be exactly the specified value"""
     min_length: builtins.int
     """MinLen specifies that this field must be the specified number of bytes
     at a minimum
     """
     max_length: builtins.int
@@ -2104,14 +2189,16 @@
     """
     ipv6: builtins.bool
     """Ipv6 specifies that the field must be a valid IPv6 address in byte
     format
     """
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.bytes | None = ...,
         min_length: builtins.int | None = ...,
         max_length: builtins.int | None = ...,
         prefix: builtins.bytes | None = ...,
@@ -2129,28 +2216,31 @@
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         ip: builtins.bool = ...,
         ipv4: builtins.bool = ...,
         ipv6: builtins.bool = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_max_length", b"_max_length", "_min_length", b"_min_length", "_multiple_of", b"_multiple_of", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "prefix", b"prefix", "suffix", b"suffix", "title", b"title", "type", b"type", "well_known", b"well_known"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_max_length", b"_max_length", "_min_length", b"_min_length", "_multiple_of", b"_multiple_of", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "in", b"in", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "prefix", b"prefix", "suffix", b"suffix", "title", b"title", "type", b"type", "well_known", b"well_known"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_max_length", b"_max_length", "_min_length", b"_min_length", "_multiple_of", b"_multiple_of", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "prefix", b"prefix", "suffix", b"suffix", "title", b"title", "type", b"type", "well_known", b"well_known"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_max_length", b"_max_length", "_min_length", b"_min_length", "_multiple_of", b"_multiple_of", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "in", b"in", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "prefix", b"prefix", "suffix", b"suffix", "title", b"title", "type", b"type", "well_known", b"well_known"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_contains", b"_contains"]) -> typing_extensions.Literal["contains"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_max_length", b"_max_length"]) -> typing_extensions.Literal["max_length"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_min_length", b"_min_length"]) -> typing_extensions.Literal["min_length"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_multiple_of", b"_multiple_of"]) -> typing_extensions.Literal["multiple_of"] | None: ...
@@ -2185,14 +2275,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     @property
     def not_in(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """NotIn specifies that this field cannot be equal to one of the specified
         values
         """
@@ -2216,14 +2307,16 @@
     """Set the corresponding sample value"""
     example_factory: builtins.str
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         not_in: collections.abc.Iterable[builtins.int] | None = ...,
         enable: builtins.bool | None = ...,
         default: builtins.int = ...,
@@ -2231,26 +2324,29 @@
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.int = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_title", b"_title", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "miss_default", b"miss_default", "title", b"title"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_title", b"_title", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "in", b"in", "miss_default", b"miss_default", "not_in", b"not_in", "title", b"title"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_title", b"_title", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "title", b"title"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_title", b"_title", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "in", b"in", "miss_default", b"miss_default", "not_in", b"not_in", "title", b"title"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_title", b"_title"]) -> typing_extensions.Literal["title"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["default_config", b"default_config"]) -> typing_extensions.Literal["default", "default_factory", "miss_default"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["example_config", b"example_config"]) -> typing_extensions.Literal["example", "example_factory"] | None: ...
@@ -2273,14 +2369,15 @@
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     skip: builtins.bool
     """Skip specifies that the validation rules of this field should not be
     evaluated
     """
     required: builtins.bool
     """Required specifies that this field must be set"""
     enable: builtins.bool
@@ -2305,14 +2402,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         skip: builtins.bool | None = ...,
         required: builtins.bool | None = ...,
         enable: builtins.bool | None = ...,
         default: builtins.float = ...,
@@ -2321,24 +2420,27 @@
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_required", b"_required", "_skip", b"_skip", "_title", b"_title", "_type", b"_type", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "miss_default", b"miss_default", "required", b"required", "skip", b"skip", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_required", b"_required", "_skip", b"_skip", "_title", b"_title", "_type", b"_type", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "miss_default", b"miss_default", "required", b"required", "skip", b"skip", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_required", b"_required", "_skip", b"_skip", "_title", b"_title", "_type", b"_type", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "required", b"required", "skip", b"skip", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_required", b"_required", "_skip", b"_skip", "_title", b"_title", "_type", b"_type", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "required", b"required", "skip", b"skip", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_required", b"_required"]) -> typing_extensions.Literal["required"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_skip", b"_skip"]) -> typing_extensions.Literal["skip"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_title", b"_title"]) -> typing_extensions.Literal["title"] | None: ...
@@ -2365,14 +2467,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     min_items: builtins.int
     """MinItems specifies that this field must have the specified number of
     items at a minimum
     """
     max_items: builtins.int
     """MaxItems specifies that this field must have the specified number of
     items at a maximum
@@ -2404,14 +2507,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         min_items: builtins.int | None = ...,
         max_items: builtins.int | None = ...,
         unique: builtins.bool | None = ...,
         items: global___FieldRules | None = ...,
@@ -2420,24 +2525,27 @@
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_items", b"_items", "_max_items", b"_max_items", "_min_items", b"_min_items", "_title", b"_title", "_type", b"_type", "_unique", b"_unique", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "items", b"items", "max_items", b"max_items", "min_items", b"min_items", "miss_default", b"miss_default", "title", b"title", "type", b"type", "unique", b"unique"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_items", b"_items", "_max_items", b"_max_items", "_min_items", b"_min_items", "_title", b"_title", "_type", b"_type", "_unique", b"_unique", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "items", b"items", "max_items", b"max_items", "min_items", b"min_items", "miss_default", b"miss_default", "title", b"title", "type", b"type", "unique", b"unique"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_items", b"_items", "_max_items", b"_max_items", "_min_items", b"_min_items", "_title", b"_title", "_type", b"_type", "_unique", b"_unique", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "items", b"items", "max_items", b"max_items", "min_items", b"min_items", "miss_default", b"miss_default", "title", b"title", "type", b"type", "unique", b"unique"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_items", b"_items", "_max_items", b"_max_items", "_min_items", b"_min_items", "_title", b"_title", "_type", b"_type", "_unique", b"_unique", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "items", b"items", "max_items", b"max_items", "min_items", b"min_items", "miss_default", b"miss_default", "title", b"title", "type", b"type", "unique", b"unique"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_items", b"_items"]) -> typing_extensions.Literal["items"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_max_items", b"_max_items"]) -> typing_extensions.Literal["max_items"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_min_items", b"_min_items"]) -> typing_extensions.Literal["min_items"] | None: ...
@@ -2468,14 +2576,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     min_pairs: builtins.int
     """MinPairs specifies that this field must have the specified number of
     KVs at a minimum
     """
     max_pairs: builtins.int
     """MaxPairs specifies that this field must have the specified number of
     KVs at a maximum
@@ -2505,14 +2614,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         min_pairs: builtins.int | None = ...,
         max_pairs: builtins.int | None = ...,
         keys: global___FieldRules | None = ...,
         values: global___FieldRules | None = ...,
@@ -2521,24 +2632,27 @@
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_keys", b"_keys", "_max_pairs", b"_max_pairs", "_min_pairs", b"_min_pairs", "_title", b"_title", "_type", b"_type", "_values", b"_values", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "keys", b"keys", "max_pairs", b"max_pairs", "min_pairs", b"min_pairs", "miss_default", b"miss_default", "title", b"title", "type", b"type", "values", b"values"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_keys", b"_keys", "_max_pairs", b"_max_pairs", "_min_pairs", b"_min_pairs", "_title", b"_title", "_type", b"_type", "_values", b"_values", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "keys", b"keys", "max_pairs", b"max_pairs", "min_pairs", b"min_pairs", "miss_default", b"miss_default", "title", b"title", "type", b"type", "values", b"values"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_keys", b"_keys", "_max_pairs", b"_max_pairs", "_min_pairs", b"_min_pairs", "_title", b"_title", "_type", b"_type", "_values", b"_values", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "keys", b"keys", "max_pairs", b"max_pairs", "min_pairs", b"min_pairs", "miss_default", b"miss_default", "title", b"title", "type", b"type", "values", b"values"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_keys", b"_keys", "_max_pairs", b"_max_pairs", "_min_pairs", b"_min_pairs", "_title", b"_title", "_type", b"_type", "_values", b"_values", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "keys", b"keys", "max_pairs", b"max_pairs", "min_pairs", b"min_pairs", "miss_default", b"miss_default", "title", b"title", "type", b"type", "values", b"values"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_keys", b"_keys"]) -> typing_extensions.Literal["keys"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_max_pairs", b"_max_pairs"]) -> typing_extensions.Literal["max_pairs"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_min_pairs", b"_min_pairs"]) -> typing_extensions.Literal["min_pairs"] | None: ...
@@ -2571,14 +2685,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     required: builtins.bool
     """Required specifies that this field must be set"""
     @property
     def not_in(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """NotIn specifies that this field's `type_url` must not be equal to any of
         the specified values.
         """
@@ -2602,14 +2717,16 @@
     """Set the corresponding sample value"""
     example_factory: builtins.str
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         required: builtins.bool | None = ...,
         not_in: collections.abc.Iterable[builtins.str] | None = ...,
         enable: builtins.bool | None = ...,
         default: builtins.str = ...,
@@ -2617,24 +2734,27 @@
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.str = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_required", b"_required", "_title", b"_title", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "miss_default", b"miss_default", "required", b"required", "title", b"title"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_required", b"_required", "_title", b"_title", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "in", b"in", "miss_default", b"miss_default", "not_in", b"not_in", "required", b"required", "title", b"title"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_required", b"_required", "_title", b"_title", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "required", b"required", "title", b"title"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_required", b"_required", "_title", b"_title", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "in", b"in", "miss_default", b"miss_default", "not_in", b"not_in", "required", b"required", "title", b"title"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_required", b"_required"]) -> typing_extensions.Literal["required"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_title", b"_title"]) -> typing_extensions.Literal["title"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["default_config", b"default_config"]) -> typing_extensions.Literal["default", "default_factory", "miss_default"] | None: ...
@@ -2664,14 +2784,15 @@
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     @property
     def const(self) -> google.protobuf.duration_pb2.Duration:
         """Const specifies that this field must be exactly the specified value"""
     @property
     def lt(self) -> google.protobuf.duration_pb2.Duration:
         """Lt specifies that this field must be less than the specified value,
         exclusive
@@ -2720,14 +2841,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: google.protobuf.duration_pb2.Duration | None = ...,
         lt: google.protobuf.duration_pb2.Duration | None = ...,
         le: google.protobuf.duration_pb2.Duration | None = ...,
         gt: google.protobuf.duration_pb2.Duration | None = ...,
@@ -2740,26 +2863,29 @@
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: google.protobuf.duration_pb2.Duration | None = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -2798,14 +2924,15 @@
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     @property
     def const(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Const specifies that this field must be exactly the specified value"""
     @property
     def lt(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Lt specifies that this field must be less than the specified value,
         exclusive
@@ -2863,14 +2990,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         lt: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         le: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         gt: google.protobuf.timestamp_pb2.Timestamp | None = ...,
@@ -2885,26 +3014,29 @@
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_gt_now", b"_gt_now", "_le", b"_le", "_lt", b"_lt", "_lt_now", b"_lt_now", "_title", b"_title", "_type", b"_type", "_within", b"_within", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "gt_now", b"gt_now", "le", b"le", "lt", b"lt", "lt_now", b"lt_now", "miss_default", b"miss_default", "title", b"title", "type", b"type", "within", b"within"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_gt_now", b"_gt_now", "_le", b"_le", "_lt", b"_lt", "_lt_now", b"_lt_now", "_title", b"_title", "_type", b"_type", "_within", b"_within", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "gt_now", b"gt_now", "le", b"le", "lt", b"lt", "lt_now", b"lt_now", "miss_default", b"miss_default", "title", b"title", "type", b"type", "within", b"within"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_gt_now", b"_gt_now", "_le", b"_le", "_lt", b"_lt", "_lt_now", b"_lt_now", "_title", b"_title", "_type", b"_type", "_within", b"_within", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "gt_now", b"gt_now", "le", b"le", "lt", b"lt", "lt_now", b"lt_now", "miss_default", b"miss_default", "title", b"title", "type", b"type", "within", b"within"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_gt_now", b"_gt_now", "_le", b"_le", "_lt", b"_lt", "_lt_now", b"_lt_now", "_title", b"_title", "_type", b"_type", "_within", b"_within", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "gt_now", b"gt_now", "le", b"le", "lt", b"lt", "lt_now", b"lt_now", "miss_default", b"miss_default", "title", b"title", "type", b"type", "within", b"within"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt_now", b"_gt_now"]) -> typing_extensions.Literal["gt_now"] | None: ...
```

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/validate_pb2.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,64 +12,64 @@
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/p2p_validate.proto\x12\x0cp2p_validate\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x81\x08\n\nFieldRules\x12\x30\n\x07message\x18\x11 \x01(\x0b\x32\x1a.p2p_validate.MessageRulesH\x01\x88\x01\x01\x12)\n\x05\x66loat\x18\x01 \x01(\x0b\x32\x18.p2p_validate.FloatRulesH\x00\x12+\n\x06\x64ouble\x18\x02 \x01(\x0b\x32\x19.p2p_validate.DoubleRulesH\x00\x12)\n\x05int32\x18\x03 \x01(\x0b\x32\x18.p2p_validate.Int32RulesH\x00\x12)\n\x05int64\x18\x04 \x01(\x0b\x32\x18.p2p_validate.Int64RulesH\x00\x12+\n\x06uint32\x18\x05 \x01(\x0b\x32\x19.p2p_validate.UInt32RulesH\x00\x12+\n\x06uint64\x18\x06 \x01(\x0b\x32\x19.p2p_validate.UInt64RulesH\x00\x12+\n\x06sint32\x18\x07 \x01(\x0b\x32\x19.p2p_validate.SInt32RulesH\x00\x12+\n\x06sint64\x18\x08 \x01(\x0b\x32\x19.p2p_validate.SInt64RulesH\x00\x12-\n\x07\x66ixed32\x18\t \x01(\x0b\x32\x1a.p2p_validate.Fixed32RulesH\x00\x12-\n\x07\x66ixed64\x18\n \x01(\x0b\x32\x1a.p2p_validate.Fixed64RulesH\x00\x12/\n\x08sfixed32\x18\x0b \x01(\x0b\x32\x1b.p2p_validate.SFixed32RulesH\x00\x12/\n\x08sfixed64\x18\x0c \x01(\x0b\x32\x1b.p2p_validate.SFixed64RulesH\x00\x12\'\n\x04\x62ool\x18\r \x01(\x0b\x32\x17.p2p_validate.BoolRulesH\x00\x12+\n\x06string\x18\x0e \x01(\x0b\x32\x19.p2p_validate.StringRulesH\x00\x12)\n\x05\x62ytes\x18\x0f \x01(\x0b\x32\x18.p2p_validate.BytesRulesH\x00\x12\'\n\x04\x65num\x18\x10 \x01(\x0b\x32\x17.p2p_validate.EnumRulesH\x00\x12/\n\x08repeated\x18\x12 \x01(\x0b\x32\x1b.p2p_validate.RepeatedRulesH\x00\x12%\n\x03map\x18\x13 \x01(\x0b\x32\x16.p2p_validate.MapRulesH\x00\x12%\n\x03\x61ny\x18\x14 \x01(\x0b\x32\x16.p2p_validate.AnyRulesH\x00\x12/\n\x08\x64uration\x18\x15 \x01(\x0b\x32\x1b.p2p_validate.DurationRulesH\x00\x12\x31\n\ttimestamp\x18\x16 \x01(\x0b\x32\x1c.p2p_validate.TimestampRulesH\x00\x42\x06\n\x04typeB\n\n\x08_message\"\xa8\x04\n\nFloatRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x02H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x02H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x02H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x02H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x02H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x02\x12\x0e\n\x06not_in\x18\x07 \x03(\x02\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0b\x44oubleRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x01H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x01H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x01H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x01H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x01H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x01\x12\x0e\n\x06not_in\x18\x07 \x03(\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa8\x04\n\nInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x05H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x05H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x05H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x05H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x05\x12\x0e\n\x06not_in\x18\x07 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa8\x04\n\nInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x03H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x03H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x03H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x03H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x03H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x03\x12\x0e\n\x06not_in\x18\x07 \x03(\x03\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0bUInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\rH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\rH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\rH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\rH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\rH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\r\x12\x0e\n\x06not_in\x18\x07 \x03(\r\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0bUInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x04H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x04H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x04H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x04\x12\x0e\n\x06not_in\x18\x07 \x03(\x04\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0bSInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x11H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x11H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x11H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x11H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x11H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x11\x12\x0e\n\x06not_in\x18\x07 \x03(\x11\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa9\x04\n\x0bSInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x12H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x12H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x12H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x12H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x12H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x12\x12\x0e\n\x06not_in\x18\x07 \x03(\x12\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xaa\x04\n\x0c\x46ixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x07H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x07H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x07H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x07H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x07H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x07\x12\x0e\n\x06not_in\x18\x07 \x03(\x07\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xaa\x04\n\x0c\x46ixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x06H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x06H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x06H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x06H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x06H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x06\x12\x0e\n\x06not_in\x18\x07 \x03(\x06\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xab\x04\n\rSFixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0fH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x0fH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x0fH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x0fH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x0fH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x0f\x12\x0e\n\x06not_in\x18\x07 \x03(\x0f\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xab\x04\n\rSFixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x10H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x10H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x10H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x10H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x10H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x10\x12\x0e\n\x06not_in\x18\x07 \x03(\x10\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xc8\x02\n\tBoolRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x08H\x01\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x02 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x03 \x01(\x08H\x00\x12\x16\n\x0cmiss_default\x18\x04 \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x04\x88\x01\x01\x12\x14\n\x07\x65xample\x18\x07 \x01(\x08H\x05\x88\x01\x01\x12\x12\n\x05\x66ield\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x11\n\x04type\x18\t \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x08\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\n\n\x08_exampleB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xfa\x06\n\x0bStringRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\tH\x03\x88\x01\x01\x12\x10\n\x03len\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmin_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x17\n\nmax_length\x18\x04 \x01(\x04H\x06\x88\x01\x01\x12\x14\n\x07pattern\x18\x05 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x06prefix\x18\x06 \x01(\tH\x08\x88\x01\x01\x12\x13\n\x06suffix\x18\x07 \x01(\tH\t\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x08 \x01(\tH\n\x88\x01\x01\x12\x19\n\x0cnot_contains\x18\t \x01(\tH\x0b\x88\x01\x01\x12\n\n\x02in\x18\n \x03(\t\x12\x0e\n\x06not_in\x18\x0b \x03(\t\x12\x0f\n\x05\x65mail\x18\x0c \x01(\x08H\x00\x12\x12\n\x08hostname\x18\r \x01(\x08H\x00\x12\x0c\n\x02ip\x18\x0e \x01(\x08H\x00\x12\x0e\n\x04ipv4\x18\x0f \x01(\x08H\x00\x12\x0e\n\x04ipv6\x18\x10 \x01(\x08H\x00\x12\r\n\x03uri\x18\x11 \x01(\x08H\x00\x12\x11\n\x07uri_ref\x18\x12 \x01(\x08H\x00\x12\x11\n\x07\x61\x64\x64ress\x18\x15 \x01(\x08H\x00\x12\x0e\n\x04uuid\x18\x16 \x01(\x08H\x00\x12\x17\n\rpydantic_type\x18\x63 \x01(\tH\x00\x12\x13\n\x06\x65nable\x18\x17 \x01(\x08H\x0c\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x18 \x01(\tH\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x19 \x01(\tH\x01\x12\x16\n\x0cmiss_default\x18\x1a \x01(\x08H\x01\x12\x12\n\x05\x61lias\x18\x1b \x01(\tH\r\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x1c \x01(\tH\x0e\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x1e \x01(\tH\x02\x12\x19\n\x0f\x65xample_factory\x18\x1f \x01(\tH\x02\x12\x12\n\x05\x66ield\x18  \x01(\tH\x0f\x88\x01\x01\x12\x11\n\x04type\x18! \x01(\tH\x10\x88\x01\x01\x12\x12\n\x05title\x18\" \x01(\tH\x11\x88\x01\x01\x42\x0c\n\nwell_knownB\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x06\n\x04_lenB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\n\n\x08_patternB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\x0f\n\r_not_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xb8\x05\n\nBytesRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0cH\x03\x88\x01\x01\x12\x17\n\nmin_length\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmax_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06prefix\x18\x05 \x01(\x0cH\x06\x88\x01\x01\x12\x13\n\x06suffix\x18\x06 \x01(\x0cH\x07\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x07 \x01(\x0cH\x08\x88\x01\x01\x12\n\n\x02in\x18\x08 \x03(\x0c\x12\x0e\n\x06not_in\x18\t \x03(\x0c\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\t\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0cH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\n\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x10 \x01(\x02H\x0c\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x11 \x01(\x0cH\x01\x12\x19\n\x0f\x65xample_factory\x18\x12 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x14 \x01(\tH\x0e\x88\x01\x01\x12\x0c\n\x02ip\x18\x15 \x01(\x08H\x02\x12\x0e\n\x04ipv4\x18\x16 \x01(\x08H\x02\x12\x0e\n\x04ipv6\x18\x17 \x01(\x08H\x02\x12\x12\n\x05title\x18\x18 \x01(\tH\x0f\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\nwell_knownB\x08\n\x06_constB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\x81\x03\n\tEnumRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\n\n\x02in\x18\x03 \x03(\x05\x12\x0e\n\x06not_in\x18\x04 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x05H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x05H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x12 \x01(\tH\x07\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_title\"\xa6\x03\n\x0cMessageRules\x12\x11\n\x04skip\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\x15\n\x08required\x18\x02 \x01(\x08H\x03\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x04\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x05\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x06\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x07\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x08\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\t\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x07\n\x05_skipB\x0b\n\t_requiredB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xe5\x03\n\rRepeatedRules\x12\x16\n\tmin_items\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_items\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x13\n\x06unique\x18\x03 \x01(\x08H\x04\x88\x01\x01\x12,\n\x05items\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_itemsB\x0c\n\n_max_itemsB\t\n\x07_uniqueB\x08\n\x06_itemsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xf8\x03\n\x08MapRules\x12\x16\n\tmin_pairs\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_pairs\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12+\n\x04keys\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x04\x88\x01\x01\x12-\n\x06values\x18\x05 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_pairsB\x0c\n\n_max_pairsB\x07\n\x05_keysB\t\n\x07_valuesB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\x86\x03\n\x08\x41nyRules\x12\x15\n\x08required\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\n\n\x02in\x18\x02 \x03(\t\x12\x0e\n\x06not_in\x18\x03 \x03(\t\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\tH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0e \x01(\tH\x01\x12\x19\n\x0f\x65xample_factory\x18\x0f \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x10 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x11 \x01(\tH\x07\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0b\n\t_requiredB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_title\"\xf4\x05\n\rDurationRules\x12-\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationH\x02\x88\x01\x01\x12*\n\x02lt\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationH\x03\x88\x01\x01\x12*\n\x02le\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationH\x04\x88\x01\x01\x12*\n\x02gt\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationH\x05\x88\x01\x01\x12*\n\x02ge\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationH\x06\x88\x01\x01\x12%\n\x02in\x18\x07 \x03(\x0b\x32\x19.google.protobuf.Duration\x12)\n\x06not_in\x18\x08 \x03(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x06\x65nable\x18\x0e \x01(\x08H\x07\x88\x01\x01\x12,\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12,\n\x07\x65xample\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationH\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\n\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0c\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title\"\xa5\x06\n\x0eTimestampRules\x12.\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12+\n\x02lt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12+\n\x02le\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x12+\n\x02gt\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12+\n\x02ge\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x13\n\x06lt_now\x18\x07 \x01(\x08H\x07\x88\x01\x01\x12\x13\n\x06gt_now\x18\x08 \x01(\x08H\x08\x88\x01\x01\x12.\n\x06within\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\t\x88\x01\x01\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\n\x88\x01\x01\x12-\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0c\x88\x01\x01\x12-\n\x07\x65xample\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x12\x19\n\x0f\x65xample_factory\x18\x11 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x12 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x13 \x01(\tH\x0e\x88\x01\x01\x12\x12\n\x05title\x18\x14 \x01(\tH\x0f\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_lt_nowB\t\n\x07_gt_nowB\t\n\x07_withinB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_title:4\n\x07ignored\x12\x1f.google.protobuf.MessageOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:3\n\x08required\x12\x1d.google.protobuf.OneofOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:J\n\x05rules\x12\x1d.google.protobuf.FieldOptions\x18\xb1\x08 \x01(\x0b\x32\x18.p2p_validate.FieldRules\x88\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/p2p_validate.proto\x12\x0cp2p_validate\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x81\x08\n\nFieldRules\x12\x30\n\x07message\x18\x11 \x01(\x0b\x32\x1a.p2p_validate.MessageRulesH\x01\x88\x01\x01\x12)\n\x05\x66loat\x18\x01 \x01(\x0b\x32\x18.p2p_validate.FloatRulesH\x00\x12+\n\x06\x64ouble\x18\x02 \x01(\x0b\x32\x19.p2p_validate.DoubleRulesH\x00\x12)\n\x05int32\x18\x03 \x01(\x0b\x32\x18.p2p_validate.Int32RulesH\x00\x12)\n\x05int64\x18\x04 \x01(\x0b\x32\x18.p2p_validate.Int64RulesH\x00\x12+\n\x06uint32\x18\x05 \x01(\x0b\x32\x19.p2p_validate.UInt32RulesH\x00\x12+\n\x06uint64\x18\x06 \x01(\x0b\x32\x19.p2p_validate.UInt64RulesH\x00\x12+\n\x06sint32\x18\x07 \x01(\x0b\x32\x19.p2p_validate.SInt32RulesH\x00\x12+\n\x06sint64\x18\x08 \x01(\x0b\x32\x19.p2p_validate.SInt64RulesH\x00\x12-\n\x07\x66ixed32\x18\t \x01(\x0b\x32\x1a.p2p_validate.Fixed32RulesH\x00\x12-\n\x07\x66ixed64\x18\n \x01(\x0b\x32\x1a.p2p_validate.Fixed64RulesH\x00\x12/\n\x08sfixed32\x18\x0b \x01(\x0b\x32\x1b.p2p_validate.SFixed32RulesH\x00\x12/\n\x08sfixed64\x18\x0c \x01(\x0b\x32\x1b.p2p_validate.SFixed64RulesH\x00\x12\'\n\x04\x62ool\x18\r \x01(\x0b\x32\x17.p2p_validate.BoolRulesH\x00\x12+\n\x06string\x18\x0e \x01(\x0b\x32\x19.p2p_validate.StringRulesH\x00\x12)\n\x05\x62ytes\x18\x0f \x01(\x0b\x32\x18.p2p_validate.BytesRulesH\x00\x12\'\n\x04\x65num\x18\x10 \x01(\x0b\x32\x17.p2p_validate.EnumRulesH\x00\x12/\n\x08repeated\x18\x12 \x01(\x0b\x32\x1b.p2p_validate.RepeatedRulesH\x00\x12%\n\x03map\x18\x13 \x01(\x0b\x32\x16.p2p_validate.MapRulesH\x00\x12%\n\x03\x61ny\x18\x14 \x01(\x0b\x32\x16.p2p_validate.AnyRulesH\x00\x12/\n\x08\x64uration\x18\x15 \x01(\x0b\x32\x1b.p2p_validate.DurationRulesH\x00\x12\x31\n\ttimestamp\x18\x16 \x01(\x0b\x32\x1c.p2p_validate.TimestampRulesH\x00\x42\x06\n\x04typeB\n\n\x08_message\"\xc6\x04\n\nFloatRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x02H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x02H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x02H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x02H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x02H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x02\x12\x0e\n\x06not_in\x18\x07 \x03(\x02\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0b\x44oubleRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x01H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x01H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x01H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x01H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x01H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x01\x12\x0e\n\x06not_in\x18\x07 \x03(\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc6\x04\n\nInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x05H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x05H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x05H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x05H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x05\x12\x0e\n\x06not_in\x18\x07 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc6\x04\n\nInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x03H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x03H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x03H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x03H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x03H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x03\x12\x0e\n\x06not_in\x18\x07 \x03(\x03\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0bUInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\rH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\rH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\rH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\rH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\rH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\r\x12\x0e\n\x06not_in\x18\x07 \x03(\r\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0bUInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x04H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x04H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x04H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x04\x12\x0e\n\x06not_in\x18\x07 \x03(\x04\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0bSInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x11H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x11H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x11H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x11H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x11H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x11\x12\x0e\n\x06not_in\x18\x07 \x03(\x11\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc7\x04\n\x0bSInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x12H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x12H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x12H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x12H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x12H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x12\x12\x0e\n\x06not_in\x18\x07 \x03(\x12\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc8\x04\n\x0c\x46ixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x07H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x07H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x07H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x07H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x07H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x07\x12\x0e\n\x06not_in\x18\x07 \x03(\x07\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc8\x04\n\x0c\x46ixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x06H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x06H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x06H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x06H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x06H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x06\x12\x0e\n\x06not_in\x18\x07 \x03(\x06\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc9\x04\n\rSFixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0fH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x0fH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x0fH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x0fH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x0fH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x0f\x12\x0e\n\x06not_in\x18\x07 \x03(\x0f\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc9\x04\n\rSFixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x10H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x10H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x10H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x10H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x10H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x10\x12\x0e\n\x06not_in\x18\x07 \x03(\x10\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xe6\x02\n\tBoolRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x08H\x01\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x02 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x03 \x01(\x08H\x00\x12\x16\n\x0cmiss_default\x18\x04 \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x04\x88\x01\x01\x12\x14\n\x07\x65xample\x18\x07 \x01(\x08H\x05\x88\x01\x01\x12\x12\n\x05\x66ield\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x11\n\x04type\x18\t \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x08\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\t\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\n\n\x08_exampleB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x98\x07\n\x0bStringRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\tH\x03\x88\x01\x01\x12\x10\n\x03len\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmin_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x17\n\nmax_length\x18\x04 \x01(\x04H\x06\x88\x01\x01\x12\x14\n\x07pattern\x18\x05 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x06prefix\x18\x06 \x01(\tH\x08\x88\x01\x01\x12\x13\n\x06suffix\x18\x07 \x01(\tH\t\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x08 \x01(\tH\n\x88\x01\x01\x12\x19\n\x0cnot_contains\x18\t \x01(\tH\x0b\x88\x01\x01\x12\n\n\x02in\x18\n \x03(\t\x12\x0e\n\x06not_in\x18\x0b \x03(\t\x12\x0f\n\x05\x65mail\x18\x0c \x01(\x08H\x00\x12\x12\n\x08hostname\x18\r \x01(\x08H\x00\x12\x0c\n\x02ip\x18\x0e \x01(\x08H\x00\x12\x0e\n\x04ipv4\x18\x0f \x01(\x08H\x00\x12\x0e\n\x04ipv6\x18\x10 \x01(\x08H\x00\x12\r\n\x03uri\x18\x11 \x01(\x08H\x00\x12\x11\n\x07uri_ref\x18\x12 \x01(\x08H\x00\x12\x11\n\x07\x61\x64\x64ress\x18\x15 \x01(\x08H\x00\x12\x0e\n\x04uuid\x18\x16 \x01(\x08H\x00\x12\x17\n\rpydantic_type\x18\x63 \x01(\tH\x00\x12\x13\n\x06\x65nable\x18\x17 \x01(\x08H\x0c\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x18 \x01(\tH\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x19 \x01(\tH\x01\x12\x16\n\x0cmiss_default\x18\x1a \x01(\x08H\x01\x12\x12\n\x05\x61lias\x18\x1b \x01(\tH\r\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x1c \x01(\tH\x0e\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x1e \x01(\tH\x02\x12\x19\n\x0f\x65xample_factory\x18\x1f \x01(\tH\x02\x12\x12\n\x05\x66ield\x18  \x01(\tH\x0f\x88\x01\x01\x12\x11\n\x04type\x18! \x01(\tH\x10\x88\x01\x01\x12\x12\n\x05title\x18\" \x01(\tH\x11\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x12\x88\x01\x01\x42\x0c\n\nwell_knownB\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x06\n\x04_lenB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\n\n\x08_patternB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\x0f\n\r_not_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xd6\x05\n\nBytesRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0cH\x03\x88\x01\x01\x12\x17\n\nmin_length\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmax_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06prefix\x18\x05 \x01(\x0cH\x06\x88\x01\x01\x12\x13\n\x06suffix\x18\x06 \x01(\x0cH\x07\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x07 \x01(\x0cH\x08\x88\x01\x01\x12\n\n\x02in\x18\x08 \x03(\x0c\x12\x0e\n\x06not_in\x18\t \x03(\x0c\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\t\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0cH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\n\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x10 \x01(\x02H\x0c\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x11 \x01(\x0cH\x01\x12\x19\n\x0f\x65xample_factory\x18\x12 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x14 \x01(\tH\x0e\x88\x01\x01\x12\x0c\n\x02ip\x18\x15 \x01(\x08H\x02\x12\x0e\n\x04ipv4\x18\x16 \x01(\x08H\x02\x12\x0e\n\x04ipv6\x18\x17 \x01(\x08H\x02\x12\x12\n\x05title\x18\x18 \x01(\tH\x0f\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x19 \x01(\tH\x10\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\nwell_knownB\x08\n\x06_constB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x9f\x03\n\tEnumRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\n\n\x02in\x18\x03 \x03(\x05\x12\x0e\n\x06not_in\x18\x04 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x05H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x05H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x12 \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x08\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_titleB\x08\n\x06_extra\"\xc4\x03\n\x0cMessageRules\x12\x11\n\x04skip\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\x15\n\x08required\x18\x02 \x01(\x08H\x03\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x04\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x05\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x06\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x07\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x08\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\t\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\n\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x07\n\x05_skipB\x0b\n\t_requiredB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x83\x04\n\rRepeatedRules\x12\x16\n\tmin_items\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_items\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x13\n\x06unique\x18\x03 \x01(\x08H\x04\x88\x01\x01\x12,\n\x05items\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0c\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_itemsB\x0c\n\n_max_itemsB\t\n\x07_uniqueB\x08\n\x06_itemsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x96\x04\n\x08MapRules\x12\x16\n\tmin_pairs\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_pairs\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12+\n\x04keys\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x04\x88\x01\x01\x12-\n\x06values\x18\x05 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0c\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_pairsB\x0c\n\n_max_pairsB\x07\n\x05_keysB\t\n\x07_valuesB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xa4\x03\n\x08\x41nyRules\x12\x15\n\x08required\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\n\n\x02in\x18\x02 \x03(\t\x12\x0e\n\x06not_in\x18\x03 \x03(\t\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\tH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0e \x01(\tH\x01\x12\x19\n\x0f\x65xample_factory\x18\x0f \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x10 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x11 \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x08\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0b\n\t_requiredB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_titleB\x08\n\x06_extra\"\x92\x06\n\rDurationRules\x12-\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationH\x02\x88\x01\x01\x12*\n\x02lt\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationH\x03\x88\x01\x01\x12*\n\x02le\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationH\x04\x88\x01\x01\x12*\n\x02gt\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationH\x05\x88\x01\x01\x12*\n\x02ge\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationH\x06\x88\x01\x01\x12%\n\x02in\x18\x07 \x03(\x0b\x32\x19.google.protobuf.Duration\x12)\n\x06not_in\x18\x08 \x03(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x06\x65nable\x18\x0e \x01(\x08H\x07\x88\x01\x01\x12,\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12,\n\x07\x65xample\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationH\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\n\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc3\x06\n\x0eTimestampRules\x12.\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12+\n\x02lt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12+\n\x02le\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x12+\n\x02gt\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12+\n\x02ge\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x13\n\x06lt_now\x18\x07 \x01(\x08H\x07\x88\x01\x01\x12\x13\n\x06gt_now\x18\x08 \x01(\x08H\x08\x88\x01\x01\x12.\n\x06within\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\t\x88\x01\x01\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\n\x88\x01\x01\x12-\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0c\x88\x01\x01\x12-\n\x07\x65xample\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x12\x19\n\x0f\x65xample_factory\x18\x11 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x12 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x13 \x01(\tH\x0e\x88\x01\x01\x12\x12\n\x05title\x18\x14 \x01(\tH\x0f\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x15 \x01(\tH\x10\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_lt_nowB\t\n\x07_gt_nowB\t\n\x07_withinB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra:4\n\x07ignored\x12\x1f.google.protobuf.MessageOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:3\n\x08required\x12\x1d.google.protobuf.OneofOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:J\n\x05rules\x12\x1d.google.protobuf.FieldOptions\x18\xb1\x08 \x01(\x0b\x32\x18.p2p_validate.FieldRules\x88\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protos.p2p_validate_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(ignored)
   google_dot_protobuf_dot_descriptor__pb2.OneofOptions.RegisterExtension(required)
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(rules)
 
   DESCRIPTOR._options = None
   _FIELDRULES._serialized_start=143
   _FIELDRULES._serialized_end=1168
   _FLOATRULES._serialized_start=1171
-  _FLOATRULES._serialized_end=1723
-  _DOUBLERULES._serialized_start=1726
-  _DOUBLERULES._serialized_end=2279
-  _INT32RULES._serialized_start=2282
-  _INT32RULES._serialized_end=2834
-  _INT64RULES._serialized_start=2837
-  _INT64RULES._serialized_end=3389
-  _UINT32RULES._serialized_start=3392
-  _UINT32RULES._serialized_end=3945
-  _UINT64RULES._serialized_start=3948
-  _UINT64RULES._serialized_end=4501
-  _SINT32RULES._serialized_start=4504
-  _SINT32RULES._serialized_end=5057
-  _SINT64RULES._serialized_start=5060
-  _SINT64RULES._serialized_end=5613
-  _FIXED32RULES._serialized_start=5616
-  _FIXED32RULES._serialized_end=6170
-  _FIXED64RULES._serialized_start=6173
-  _FIXED64RULES._serialized_end=6727
-  _SFIXED32RULES._serialized_start=6730
-  _SFIXED32RULES._serialized_end=7285
-  _SFIXED64RULES._serialized_start=7288
-  _SFIXED64RULES._serialized_end=7843
-  _BOOLRULES._serialized_start=7846
-  _BOOLRULES._serialized_end=8174
-  _STRINGRULES._serialized_start=8177
-  _STRINGRULES._serialized_end=9067
-  _BYTESRULES._serialized_start=9070
-  _BYTESRULES._serialized_end=9766
-  _ENUMRULES._serialized_start=9769
-  _ENUMRULES._serialized_end=10154
-  _MESSAGERULES._serialized_start=10157
-  _MESSAGERULES._serialized_end=10579
-  _REPEATEDRULES._serialized_start=10582
-  _REPEATEDRULES._serialized_end=11067
-  _MAPRULES._serialized_start=11070
-  _MAPRULES._serialized_end=11574
-  _ANYRULES._serialized_start=11577
-  _ANYRULES._serialized_end=11967
-  _DURATIONRULES._serialized_start=11970
-  _DURATIONRULES._serialized_end=12726
-  _TIMESTAMPRULES._serialized_start=12729
-  _TIMESTAMPRULES._serialized_end=13534
+  _FLOATRULES._serialized_end=1753
+  _DOUBLERULES._serialized_start=1756
+  _DOUBLERULES._serialized_end=2339
+  _INT32RULES._serialized_start=2342
+  _INT32RULES._serialized_end=2924
+  _INT64RULES._serialized_start=2927
+  _INT64RULES._serialized_end=3509
+  _UINT32RULES._serialized_start=3512
+  _UINT32RULES._serialized_end=4095
+  _UINT64RULES._serialized_start=4098
+  _UINT64RULES._serialized_end=4681
+  _SINT32RULES._serialized_start=4684
+  _SINT32RULES._serialized_end=5267
+  _SINT64RULES._serialized_start=5270
+  _SINT64RULES._serialized_end=5853
+  _FIXED32RULES._serialized_start=5856
+  _FIXED32RULES._serialized_end=6440
+  _FIXED64RULES._serialized_start=6443
+  _FIXED64RULES._serialized_end=7027
+  _SFIXED32RULES._serialized_start=7030
+  _SFIXED32RULES._serialized_end=7615
+  _SFIXED64RULES._serialized_start=7618
+  _SFIXED64RULES._serialized_end=8203
+  _BOOLRULES._serialized_start=8206
+  _BOOLRULES._serialized_end=8564
+  _STRINGRULES._serialized_start=8567
+  _STRINGRULES._serialized_end=9487
+  _BYTESRULES._serialized_start=9490
+  _BYTESRULES._serialized_end=10216
+  _ENUMRULES._serialized_start=10219
+  _ENUMRULES._serialized_end=10634
+  _MESSAGERULES._serialized_start=10637
+  _MESSAGERULES._serialized_end=11089
+  _REPEATEDRULES._serialized_start=11092
+  _REPEATEDRULES._serialized_end=11607
+  _MAPRULES._serialized_start=11610
+  _MAPRULES._serialized_end=12144
+  _ANYRULES._serialized_start=12147
+  _ANYRULES._serialized_end=12567
+  _DURATIONRULES._serialized_start=12570
+  _DURATIONRULES._serialized_end=13356
+  _TIMESTAMPRULES._serialized_start=13359
+  _TIMESTAMPRULES._serialized_end=14194
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -152,14 +152,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.float
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.float
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.float
@@ -205,14 +206,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.float | None = ...,
         lt: builtins.float | None = ...,
         le: builtins.float | None = ...,
         gt: builtins.float | None = ...,
@@ -226,26 +229,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -284,14 +290,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.float
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.float
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.float
@@ -337,14 +344,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.float | None = ...,
         lt: builtins.float | None = ...,
         le: builtins.float | None = ...,
         gt: builtins.float | None = ...,
@@ -358,26 +367,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -416,14 +428,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -469,14 +482,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -490,26 +505,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -548,14 +566,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -601,14 +620,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -622,26 +643,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -680,14 +704,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -733,14 +758,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -754,26 +781,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -812,14 +842,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -865,14 +896,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -886,26 +919,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -944,14 +980,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -997,14 +1034,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1018,26 +1057,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1076,14 +1118,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1129,14 +1172,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1150,26 +1195,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1208,14 +1256,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1261,14 +1310,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1282,26 +1333,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1340,14 +1394,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1393,14 +1448,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1414,26 +1471,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1472,14 +1532,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1525,14 +1586,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1546,26 +1609,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1604,14 +1670,15 @@
     DESCRIPTION_FIELD_NUMBER: builtins.int
     MULTIPLE_OF_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     lt: builtins.int
     """Lt specifies that this field must be less than the specified value,
     exclusive
     """
     le: builtins.int
@@ -1657,14 +1724,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         lt: builtins.int | None = ...,
         le: builtins.int | None = ...,
         gt: builtins.int | None = ...,
@@ -1678,26 +1747,29 @@
         description: builtins.str | None = ...,
         multiple_of: builtins.float | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_multiple_of", b"_multiple_of", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -1727,14 +1799,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.bool
     """Const specifies that this field must be exactly the specified value"""
     enable: builtins.bool
     """Whether to enable this field, if not, the generated Model will not carry this field"""
     default: builtins.bool
     """The default value corresponding to the field, if not set,
     the default value is the default value of the corresponding type of the field
@@ -1749,41 +1822,46 @@
     """Set the corresponding sample value"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.bool | None = ...,
         enable: builtins.bool | None = ...,
         default: builtins.bool = ...,
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.bool | None = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_example", b"_example", "_field", b"_field", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "description", b"description", "enable", b"enable", "example", b"example", "field", b"field", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_example", b"_example", "_field", b"_field", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "description", b"description", "enable", b"enable", "example", b"example", "field", b"field", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_example", b"_example", "_extra", b"_extra", "_field", b"_field", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "description", b"description", "enable", b"enable", "example", b"example", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_example", b"_example", "_extra", b"_extra", "_field", b"_field", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "description", b"description", "enable", b"enable", "example", b"example", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_example", b"_example"]) -> typing_extensions.Literal["example"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_title", b"_title"]) -> typing_extensions.Literal["title"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_type", b"_type"]) -> typing_extensions.Literal["type"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["default_config", b"default_config"]) -> typing_extensions.Literal["default", "miss_default"] | None: ...
@@ -1823,14 +1901,15 @@
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.str
     """Const specifies that this field must be exactly the specified value"""
     len: builtins.int
     """Len specifies that this field must be the specified number of
     characters (Unicode code points). Note that the number of
     characters may differ from the number of bytes in the string.
     """
@@ -1933,14 +2012,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.str | None = ...,
         len: builtins.int | None = ...,
         min_length: builtins.int | None = ...,
         max_length: builtins.int | None = ...,
@@ -1967,28 +2048,31 @@
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.str = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_len", b"_len", "_max_length", b"_max_length", "_min_length", b"_min_length", "_not_contains", b"_not_contains", "_pattern", b"_pattern", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "address", b"address", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "email", b"email", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "hostname", b"hostname", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "len", b"len", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "not_contains", b"not_contains", "pattern", b"pattern", "prefix", b"prefix", "pydantic_type", b"pydantic_type", "suffix", b"suffix", "title", b"title", "type", b"type", "uri", b"uri", "uri_ref", b"uri_ref", "uuid", b"uuid", "well_known", b"well_known"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_len", b"_len", "_max_length", b"_max_length", "_min_length", b"_min_length", "_not_contains", b"_not_contains", "_pattern", b"_pattern", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "address", b"address", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "email", b"email", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "hostname", b"hostname", "in", b"in", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "len", b"len", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "not_contains", b"not_contains", "not_in", b"not_in", "pattern", b"pattern", "prefix", b"prefix", "pydantic_type", b"pydantic_type", "suffix", b"suffix", "title", b"title", "type", b"type", "uri", b"uri", "uri_ref", b"uri_ref", "uuid", b"uuid", "well_known", b"well_known"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_len", b"_len", "_max_length", b"_max_length", "_min_length", b"_min_length", "_not_contains", b"_not_contains", "_pattern", b"_pattern", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "address", b"address", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "email", b"email", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "hostname", b"hostname", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "len", b"len", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "not_contains", b"not_contains", "pattern", b"pattern", "prefix", b"prefix", "pydantic_type", b"pydantic_type", "suffix", b"suffix", "title", b"title", "type", b"type", "uri", b"uri", "uri_ref", b"uri_ref", "uuid", b"uuid", "well_known", b"well_known"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_len", b"_len", "_max_length", b"_max_length", "_min_length", b"_min_length", "_not_contains", b"_not_contains", "_pattern", b"_pattern", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "address", b"address", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "email", b"email", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "hostname", b"hostname", "in", b"in", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "len", b"len", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "not_contains", b"not_contains", "not_in", b"not_in", "pattern", b"pattern", "prefix", b"prefix", "pydantic_type", b"pydantic_type", "suffix", b"suffix", "title", b"title", "type", b"type", "uri", b"uri", "uri_ref", b"uri_ref", "uuid", b"uuid", "well_known", b"well_known"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_contains", b"_contains"]) -> typing_extensions.Literal["contains"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_len", b"_len"]) -> typing_extensions.Literal["len"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_max_length", b"_max_length"]) -> typing_extensions.Literal["max_length"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_min_length", b"_min_length"]) -> typing_extensions.Literal["min_length"] | None: ...
@@ -2037,14 +2121,15 @@
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     IP_FIELD_NUMBER: builtins.int
     IPV4_FIELD_NUMBER: builtins.int
     IPV6_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.bytes
     """Const specifies that this field must be exactly the specified value"""
     min_length: builtins.int
     """MinLen specifies that this field must be the specified number of bytes
     at a minimum
     """
     max_length: builtins.int
@@ -2104,14 +2189,16 @@
     """
     ipv6: builtins.bool
     """Ipv6 specifies that the field must be a valid IPv6 address in byte
     format
     """
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.bytes | None = ...,
         min_length: builtins.int | None = ...,
         max_length: builtins.int | None = ...,
         prefix: builtins.bytes | None = ...,
@@ -2129,28 +2216,31 @@
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         ip: builtins.bool = ...,
         ipv4: builtins.bool = ...,
         ipv6: builtins.bool = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_max_length", b"_max_length", "_min_length", b"_min_length", "_multiple_of", b"_multiple_of", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "prefix", b"prefix", "suffix", b"suffix", "title", b"title", "type", b"type", "well_known", b"well_known"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_max_length", b"_max_length", "_min_length", b"_min_length", "_multiple_of", b"_multiple_of", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "in", b"in", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "prefix", b"prefix", "suffix", b"suffix", "title", b"title", "type", b"type", "well_known", b"well_known"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_max_length", b"_max_length", "_min_length", b"_min_length", "_multiple_of", b"_multiple_of", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "prefix", b"prefix", "suffix", b"suffix", "title", b"title", "type", b"type", "well_known", b"well_known"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_contains", b"_contains", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_max_length", b"_max_length", "_min_length", b"_min_length", "_multiple_of", b"_multiple_of", "_prefix", b"_prefix", "_suffix", b"_suffix", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "contains", b"contains", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "in", b"in", "ip", b"ip", "ipv4", b"ipv4", "ipv6", b"ipv6", "max_length", b"max_length", "min_length", b"min_length", "miss_default", b"miss_default", "multiple_of", b"multiple_of", "not_in", b"not_in", "prefix", b"prefix", "suffix", b"suffix", "title", b"title", "type", b"type", "well_known", b"well_known"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_contains", b"_contains"]) -> typing_extensions.Literal["contains"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_max_length", b"_max_length"]) -> typing_extensions.Literal["max_length"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_min_length", b"_min_length"]) -> typing_extensions.Literal["min_length"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_multiple_of", b"_multiple_of"]) -> typing_extensions.Literal["multiple_of"] | None: ...
@@ -2185,14 +2275,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     const: builtins.int
     """Const specifies that this field must be exactly the specified value"""
     @property
     def not_in(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """NotIn specifies that this field cannot be equal to one of the specified
         values
         """
@@ -2216,14 +2307,16 @@
     """Set the corresponding sample value"""
     example_factory: builtins.str
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: builtins.int | None = ...,
         not_in: collections.abc.Iterable[builtins.int] | None = ...,
         enable: builtins.bool | None = ...,
         default: builtins.int = ...,
@@ -2231,26 +2324,29 @@
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.int = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_title", b"_title", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "miss_default", b"miss_default", "title", b"title"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_title", b"_title", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "in", b"in", "miss_default", b"miss_default", "not_in", b"not_in", "title", b"title"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_title", b"_title", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "title", b"title"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_title", b"_title", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "in", b"in", "miss_default", b"miss_default", "not_in", b"not_in", "title", b"title"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_title", b"_title"]) -> typing_extensions.Literal["title"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["default_config", b"default_config"]) -> typing_extensions.Literal["default", "default_factory", "miss_default"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["example_config", b"example_config"]) -> typing_extensions.Literal["example", "example_factory"] | None: ...
@@ -2273,14 +2369,15 @@
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     skip: builtins.bool
     """Skip specifies that the validation rules of this field should not be
     evaluated
     """
     required: builtins.bool
     """Required specifies that this field must be set"""
     enable: builtins.bool
@@ -2305,14 +2402,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         skip: builtins.bool | None = ...,
         required: builtins.bool | None = ...,
         enable: builtins.bool | None = ...,
         default: builtins.float = ...,
@@ -2321,24 +2420,27 @@
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.float = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_required", b"_required", "_skip", b"_skip", "_title", b"_title", "_type", b"_type", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "miss_default", b"miss_default", "required", b"required", "skip", b"skip", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_required", b"_required", "_skip", b"_skip", "_title", b"_title", "_type", b"_type", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "miss_default", b"miss_default", "required", b"required", "skip", b"skip", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_required", b"_required", "_skip", b"_skip", "_title", b"_title", "_type", b"_type", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "required", b"required", "skip", b"skip", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_required", b"_required", "_skip", b"_skip", "_title", b"_title", "_type", b"_type", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "required", b"required", "skip", b"skip", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_required", b"_required"]) -> typing_extensions.Literal["required"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_skip", b"_skip"]) -> typing_extensions.Literal["skip"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_title", b"_title"]) -> typing_extensions.Literal["title"] | None: ...
@@ -2365,14 +2467,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     min_items: builtins.int
     """MinItems specifies that this field must have the specified number of
     items at a minimum
     """
     max_items: builtins.int
     """MaxItems specifies that this field must have the specified number of
     items at a maximum
@@ -2404,14 +2507,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         min_items: builtins.int | None = ...,
         max_items: builtins.int | None = ...,
         unique: builtins.bool | None = ...,
         items: global___FieldRules | None = ...,
@@ -2420,24 +2525,27 @@
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_items", b"_items", "_max_items", b"_max_items", "_min_items", b"_min_items", "_title", b"_title", "_type", b"_type", "_unique", b"_unique", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "items", b"items", "max_items", b"max_items", "min_items", b"min_items", "miss_default", b"miss_default", "title", b"title", "type", b"type", "unique", b"unique"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_items", b"_items", "_max_items", b"_max_items", "_min_items", b"_min_items", "_title", b"_title", "_type", b"_type", "_unique", b"_unique", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "items", b"items", "max_items", b"max_items", "min_items", b"min_items", "miss_default", b"miss_default", "title", b"title", "type", b"type", "unique", b"unique"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_items", b"_items", "_max_items", b"_max_items", "_min_items", b"_min_items", "_title", b"_title", "_type", b"_type", "_unique", b"_unique", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "items", b"items", "max_items", b"max_items", "min_items", b"min_items", "miss_default", b"miss_default", "title", b"title", "type", b"type", "unique", b"unique"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_items", b"_items", "_max_items", b"_max_items", "_min_items", b"_min_items", "_title", b"_title", "_type", b"_type", "_unique", b"_unique", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "items", b"items", "max_items", b"max_items", "min_items", b"min_items", "miss_default", b"miss_default", "title", b"title", "type", b"type", "unique", b"unique"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_items", b"_items"]) -> typing_extensions.Literal["items"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_max_items", b"_max_items"]) -> typing_extensions.Literal["max_items"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_min_items", b"_min_items"]) -> typing_extensions.Literal["min_items"] | None: ...
@@ -2468,14 +2576,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     min_pairs: builtins.int
     """MinPairs specifies that this field must have the specified number of
     KVs at a minimum
     """
     max_pairs: builtins.int
     """MaxPairs specifies that this field must have the specified number of
     KVs at a maximum
@@ -2505,14 +2614,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         min_pairs: builtins.int | None = ...,
         max_pairs: builtins.int | None = ...,
         keys: global___FieldRules | None = ...,
         values: global___FieldRules | None = ...,
@@ -2521,24 +2632,27 @@
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_keys", b"_keys", "_max_pairs", b"_max_pairs", "_min_pairs", b"_min_pairs", "_title", b"_title", "_type", b"_type", "_values", b"_values", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "keys", b"keys", "max_pairs", b"max_pairs", "min_pairs", b"min_pairs", "miss_default", b"miss_default", "title", b"title", "type", b"type", "values", b"values"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_keys", b"_keys", "_max_pairs", b"_max_pairs", "_min_pairs", b"_min_pairs", "_title", b"_title", "_type", b"_type", "_values", b"_values", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "keys", b"keys", "max_pairs", b"max_pairs", "min_pairs", b"min_pairs", "miss_default", b"miss_default", "title", b"title", "type", b"type", "values", b"values"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_keys", b"_keys", "_max_pairs", b"_max_pairs", "_min_pairs", b"_min_pairs", "_title", b"_title", "_type", b"_type", "_values", b"_values", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "keys", b"keys", "max_pairs", b"max_pairs", "min_pairs", b"min_pairs", "miss_default", b"miss_default", "title", b"title", "type", b"type", "values", b"values"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_keys", b"_keys", "_max_pairs", b"_max_pairs", "_min_pairs", b"_min_pairs", "_title", b"_title", "_type", b"_type", "_values", b"_values", "alias", b"alias", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "keys", b"keys", "max_pairs", b"max_pairs", "min_pairs", b"min_pairs", "miss_default", b"miss_default", "title", b"title", "type", b"type", "values", b"values"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_keys", b"_keys"]) -> typing_extensions.Literal["keys"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_max_pairs", b"_max_pairs"]) -> typing_extensions.Literal["max_pairs"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_min_pairs", b"_min_pairs"]) -> typing_extensions.Literal["min_pairs"] | None: ...
@@ -2571,14 +2685,15 @@
     MISS_DEFAULT_FIELD_NUMBER: builtins.int
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     required: builtins.bool
     """Required specifies that this field must be set"""
     @property
     def not_in(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """NotIn specifies that this field's `type_url` must not be equal to any of
         the specified values.
         """
@@ -2602,14 +2717,16 @@
     """Set the corresponding sample value"""
     example_factory: builtins.str
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         required: builtins.bool | None = ...,
         not_in: collections.abc.Iterable[builtins.str] | None = ...,
         enable: builtins.bool | None = ...,
         default: builtins.str = ...,
@@ -2617,24 +2734,27 @@
         miss_default: builtins.bool = ...,
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: builtins.str = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_required", b"_required", "_title", b"_title", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "miss_default", b"miss_default", "required", b"required", "title", b"title"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_required", b"_required", "_title", b"_title", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "in", b"in", "miss_default", b"miss_default", "not_in", b"not_in", "required", b"required", "title", b"title"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_required", b"_required", "_title", b"_title", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "miss_default", b"miss_default", "required", b"required", "title", b"title"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_required", b"_required", "_title", b"_title", "alias", b"alias", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "in", b"in", "miss_default", b"miss_default", "not_in", b"not_in", "required", b"required", "title", b"title"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_required", b"_required"]) -> typing_extensions.Literal["required"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_title", b"_title"]) -> typing_extensions.Literal["title"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["default_config", b"default_config"]) -> typing_extensions.Literal["default", "default_factory", "miss_default"] | None: ...
@@ -2664,14 +2784,15 @@
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     @property
     def const(self) -> google.protobuf.duration_pb2.Duration:
         """Const specifies that this field must be exactly the specified value"""
     @property
     def lt(self) -> google.protobuf.duration_pb2.Duration:
         """Lt specifies that this field must be less than the specified value,
         exclusive
@@ -2720,14 +2841,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: google.protobuf.duration_pb2.Duration | None = ...,
         lt: google.protobuf.duration_pb2.Duration | None = ...,
         le: google.protobuf.duration_pb2.Duration | None = ...,
         gt: google.protobuf.duration_pb2.Duration | None = ...,
@@ -2740,26 +2863,29 @@
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: google.protobuf.duration_pb2.Duration | None = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "title", b"title", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_le", b"_le", "_lt", b"_lt", "_title", b"_title", "_type", b"_type", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "in", b"in", "le", b"le", "lt", b"lt", "miss_default", b"miss_default", "not_in", b"not_in", "title", b"title", "type", b"type"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_le", b"_le"]) -> typing_extensions.Literal["le"] | None: ...
@@ -2798,14 +2924,15 @@
     ALIAS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXAMPLE_FIELD_NUMBER: builtins.int
     EXAMPLE_FACTORY_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
+    EXTRA_FIELD_NUMBER: builtins.int
     @property
     def const(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Const specifies that this field must be exactly the specified value"""
     @property
     def lt(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Lt specifies that this field must be less than the specified value,
         exclusive
@@ -2863,14 +2990,16 @@
     """Set the corresponding sample value factory function, support template variables"""
     field: builtins.str
     """Set the Field object corresponding to the field, support template variables"""
     type: builtins.str
     """Set the type object corresponding to the field, support template variables"""
     title: builtins.str
     """The title corresponding to the field"""
+    extra: builtins.str
+    """Field's custom extension parameter in the format Json"""
     def __init__(
         self,
         *,
         const: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         lt: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         le: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         gt: google.protobuf.timestamp_pb2.Timestamp | None = ...,
@@ -2885,26 +3014,29 @@
         alias: builtins.str | None = ...,
         description: builtins.str | None = ...,
         example: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         example_factory: builtins.str = ...,
         field: builtins.str | None = ...,
         type: builtins.str | None = ...,
         title: builtins.str | None = ...,
+        extra: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_gt_now", b"_gt_now", "_le", b"_le", "_lt", b"_lt", "_lt_now", b"_lt_now", "_title", b"_title", "_type", b"_type", "_within", b"_within", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "gt_now", b"gt_now", "le", b"le", "lt", b"lt", "lt_now", b"lt_now", "miss_default", b"miss_default", "title", b"title", "type", b"type", "within", b"within"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_gt_now", b"_gt_now", "_le", b"_le", "_lt", b"_lt", "_lt_now", b"_lt_now", "_title", b"_title", "_type", b"_type", "_within", b"_within", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "field", b"field", "ge", b"ge", "gt", b"gt", "gt_now", b"gt_now", "le", b"le", "lt", b"lt", "lt_now", b"lt_now", "miss_default", b"miss_default", "title", b"title", "type", b"type", "within", b"within"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_gt_now", b"_gt_now", "_le", b"_le", "_lt", b"_lt", "_lt_now", b"_lt_now", "_title", b"_title", "_type", b"_type", "_within", b"_within", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "gt_now", b"gt_now", "le", b"le", "lt", b"lt", "lt_now", b"lt_now", "miss_default", b"miss_default", "title", b"title", "type", b"type", "within", b"within"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_alias", b"_alias", "_const", b"_const", "_description", b"_description", "_enable", b"_enable", "_extra", b"_extra", "_field", b"_field", "_ge", b"_ge", "_gt", b"_gt", "_gt_now", b"_gt_now", "_le", b"_le", "_lt", b"_lt", "_lt_now", b"_lt_now", "_title", b"_title", "_type", b"_type", "_within", b"_within", "alias", b"alias", "const", b"const", "default", b"default", "default_config", b"default_config", "default_factory", b"default_factory", "description", b"description", "enable", b"enable", "example", b"example", "example_config", b"example_config", "example_factory", b"example_factory", "extra", b"extra", "field", b"field", "ge", b"ge", "gt", b"gt", "gt_now", b"gt_now", "le", b"le", "lt", b"lt", "lt_now", b"lt_now", "miss_default", b"miss_default", "title", b"title", "type", b"type", "within", b"within"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_alias", b"_alias"]) -> typing_extensions.Literal["alias"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_const", b"_const"]) -> typing_extensions.Literal["const"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_description", b"_description"]) -> typing_extensions.Literal["description"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_enable", b"_enable"]) -> typing_extensions.Literal["enable"] | None: ...
     @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_extra", b"_extra"]) -> typing_extensions.Literal["extra"] | None: ...
+    @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_field", b"_field"]) -> typing_extensions.Literal["field"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_ge", b"_ge"]) -> typing_extensions.Literal["ge"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt", b"_gt"]) -> typing_extensions.Literal["gt"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_gt_now", b"_gt_now"]) -> typing_extensions.Literal["gt_now"] | None: ...
```

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/validate_pb2.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/protos/protos/validate_pb2.pyi` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/protos/protos/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/types.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/protobuf_to_pydantic/util.py` & `protobuf_to_pydantic-0.1.7.1/protobuf_to_pydantic/util.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7/pyproject.toml` & `protobuf_to_pydantic-0.1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protobuf_to_pydantic"
-version = "v0.1.7"
+version = "v0.1.7.1"
 description = "Convert Protobuf-generated Python objects to Pydantic.BaseModel objects with parameter checksum"
 authors = ["So1n <so1n897046026@gmail.com>"]
 license = "Apache Software License"
 readme = "./README.md"
 repository = "https://github.com/so1n/protobuf_to_pydantic"
 homepage = "https://github.com/so1n/protobuf_to_pydantic"
 packages = [
```

### Comparing `protobuf_to_pydantic-0.1.7/setup.py` & `protobuf_to_pydantic-0.1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 entry_points = \
 {'console_scripts': ['protoc-gen-protobuf-to-pydantic = '
                      'protobuf_to_pydantic.plugin.main:main']}
 
 setup_kwargs = {
     'name': 'protobuf-to-pydantic',
-    'version': '0.1.7',
+    'version': '0.1.7.1',
     'description': 'Convert Protobuf-generated Python objects to Pydantic.BaseModel objects with parameter checksum',
     'long_description': '# protobuf_to_pydantic\nGenerate the `pydantic.Base Model` class (and the corresponding source code) with parameter verification function through the Protobuf file\n\n> NOTE:\n>  - Only supports proto3\n\n[中文文档](https://github.com/so1n/protobuf_to_pydantic/blob/master/README_ZH.md)\n# 1.Installation\n```bash\npip install protobuf_to_pydantic\n```\n\n# 2.Quick Start\n`protobuf_to_pydantic` currently has two methods to generate `pydantic.BaseModel` objects through Protobuf files,\nThe first method is to generate the corresponding `Python` code file through the Protobuf file in the form of a plugin.\nThe second method is to generate the corresponding `pydantic.BaseModel` object based on the `Message` object at runtime.\n\n## 2.1.Directly generate `pydantic.BaseModel` code files through plugins\n> Note: The `protobuf-to-pydantic` plugin depends on `mypy-protobuf`, please install `mypy-protobuf` through the command `python -m pip install protobuf-to-pydanitc[mypy-protobuf]`.\n### 2.1.1.Use of plugin\nThe plugin method is the most recommended way to use `protobuf-to-pydantic`,\nit supports the most complete functions, and it is also very simple to use, assuming that the code corresponding to the Protobuf file is usually generated by the following command:\n```bash\npython -m grpc_tools.protoc -I. example.proto\n```\nThen after installing `protobuf-to-pydantic`, can use the `--protobuf-to-pydantic out` option to use `protobuf-to-pydantic`, the command is as follows:\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=. example.proto\n```\n\nAmong them, `--protobuf-to-pydantic out=.` indicates the use of the `prorobuf-to-pydanitc` plugin, and declares that the output location of the `protobuf-to-pydantic` plugin is `.` (indicating the use of `grpc tools.proto ` to use the output path),\nIn this way, the `protobuf-to-pydantic` plugin will write its own generated content in the corresponding file (the file name ends with `p2p.py`), such as `protobuf-to-pydantic` is `example.proto `The generated code file is named `example_p2p.py`\n\n### 2.1.2.Plugin configuration\n`protobuf-to-pydantic` supports configuration functions by reading a `Python` file.\nDevelopers first need to create a configuration file in the current path of the running command, the file name is `plugin_config.py`, and write the following code:\n```Python\nimport logging\nfrom typing import List, Type\n\nfrom google.protobuf.any_pb2 import Any  # type: ignore\nfrom pydantic import confloat, conint\nfrom pydantic.fields import FieldInfo\n\nfrom protobuf_to_pydantic.gen_model import DescTemplate\n\n# Configure the log output format and log level of the plugin, which is very useful when debugging\nlogging.basicConfig(format="[%(asctime)s %(levelname)s] %(message)s", datefmt="%y-%m-%d %H:%M:%S", level=logging.DEBUG)\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\ndef customer_any() -> Any:\n    return Any  # type: ignore\n\n\n# For the configuration of the local template, see the use of the local template for details\nlocal_dict = {\n    "CustomerField": CustomerField,\n    "confloat": confloat,\n    "conint": conint,\n    "customer_any": customer_any,\n}\n# Specifies the start of key comments\ncomment_prefix = "p2p"\n# Specify the class of the template, you can extend the template by inheriting this class, see the chapter on custom templates for details\ndesc_template: Type[DescTemplate] = DescTemplate\n# Specify the protobuf files of which packages to ignore, and the messages of the ignored packages will not be parsed\nignore_pkg_list: List[str] = ["validate", "p2p_validate"]\n# Specifies the generated file name suffix (without .py)\nfile_name_suffix = "_p2p"\n```\nNext, change `--protobuf-to-pydantic out=.` in the command to `--protobuf-to-pydantic out=config path=plugin config.py:.`, as follows:\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto\n```\nAmong them, `config path=plugin_config.py` on the left side of `:` indicates that the configuration file path to be read is `plugin_config.py`, and the right side of `:` still declares the output of the `protobuf-to-pydantic` plugin The position is `.`.\nIn this way, the `protobuf-to-pydantic` plugin can be loaded into the configuration file specified by the developer when it is running, and then run according to the configuration defined by the configuration file.\n\n> Note: 更多配置内容见`protobuf_to_pydantic/plugin/config.py`文件\n> Note: For more information on configuration, see the \'protobuf_to_pydantic/plugin/config.py\'\n## 2.2.Generate a `pydantic.BaseModel` object at runtime\n`protobuf_to_pydantic` can generate the corresponding `pydantic.BaseModel` object based on the `Message` object at runtime。\n\nFor example, the `UserMessage` in the following Protobuf file named `demo.proto`:\n```protobuf\n// path: ./demo.proto\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\nmessage UserMessage {\n  string uid=1;\n  int32 age=2;\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  string user_name=6;\n}\n```\nThrough `grpc_tools.protoc`, the corresponding `Python` code can be generated according to the Protobuf file (the file name at this time is `demo_pb2.py`),\nand the `msg_to_pydantic_model` method of `protobuf_to_pydantic` can read the generated Proto file at runtime Message object data,\nand generate the corresponding `pydantic.BaseModel` object:\n\n```Python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom . import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n\n# output\n# {\n#   \'uid\': FieldInfo(default=\'\', extra={}),\n#   \'age\': FieldInfo(default=0, extra={}),\n#   \'height\': FieldInfo(default=0.0, extra={}),\n#   \'sex\': FieldInfo(default=0, extra={}),\n#   \'is_adult\': FieldInfo(default=False, extra={}),\n#   \'user_name\': FieldInfo(default=\'\', extra={})\n#  }\n```\nThrough the output results, it can be found that the generated `pydantic.BaseModel` object also contains `uid`, `age`, `height`, `sex`, `is adult` and `user name` fields, and their corresponding `default` The information is consistent with the `UserMessage` in the Protobuf file.\n\nIn addition to generating the corresponding `pydantic.BaseModel` object at runtime, `protobuf-to-pydantic` also supports converting the `pydantic.BaseModel` object to the corresponding `Python` code text at runtime (only compatible with `protobuf_to_pydantic `generated `pydantic.BaseModel` object).\nAmong them, the `pydantic_model_to_py_code` method of `protobuf_to_pydantic` is used to generate code text, and the `pydantic_model_to_py_file` method of `protobuf_to_pydantic` is used to generate code files,\nthe sample code of `pydantic_model_to_py_file` method of `protobuf_to_pydantic` is as follows:\n```Python\nfrom protobuf_to_pydantic import msg_to_pydantic_model, pydantic_model_to_py_file\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\npydantic_model_to_py_file(\n    "./demo_gen_code.py",\n    msg_to_pydantic_model(demo_pb2.NestedMessage),\n)\n```\nThe code will first convert `demo_pb2.NestedMessage` into a `pydantic.BaseModel` object, and then the generated object will be converted into the corresponding code content by the `pydantic_model_to_py_file` method and written to `demo_gen_code.py` file.\n\n## 2.3.Parameter verification\nThe `Message` object generated according to the Protobuf file will only carry a small amount of information. This is because the ordinary Protobuf file does not have enough parameter verification related information, which requires us to improve the parameter verification information of the `Message` object through some additional ways.\nCurrently `protobuf_to_pydantic` supports multiple ways to obtain other information of the Message, so that the generated `pydantic.BaseModel` object has the function of parameter verification.\n\n> NOTE:\n>  - 1.The text annotation function is not the focus of subsequent function development, and the P2P mode is recommended。\n>  - 2.Plugin mode only supports PGV and P2P mode\n\n### 2.3.1.Text annotation\nDevelopers can write comments that meet the requirements of `protobuf_to_pydantic` for each field in the Protobuf file to provide parameter verification information for `protobuf_to_pydantic`, such as the following example:\n```protobuf\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\n// user info\nmessage UserMessage {\n  // p2p: {"miss_default": true, "example": "10086"}\n  // p2p: {"title": "UID"}\n  string uid=1; // p2p: {"description": "user union id"}\n  // p2p: {"example": 18, "title": "use age", "ge": 0}\n  int32 age=2;\n  // p2p: {"ge": 0, "le": 2.5}\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  // p2p: {"description": "user name"}\n  // p2p: {"default": "", "min_length": 1, "max_length": "10", "example": "so1n"}\n  string user_name=6;\n}\n```\nIn this example, each annotation that can be used by `protobuf_to_pydantic` starts with `p2p:` (supports customization) and is followed by a complete Json string. If you are familiar with the usage of `pydantic`, you can find This Json string contains the verification information corresponding to `pydantic.Field`. For example, the `uid` field in `UserMessage` contains a total of 4 pieces of information as follows：\n\n| Column       | Meaning                                                                               |\n|--------------|---------------------------------------------------------------------------------------|\n| miss_default | Indicates that the generated field does not have a default value                      |\n| example      | An example value representing the generated field is 10086                            |\n| title        | Indicates that the schema name of the field is UID                                    |\n | description  | The schema documentation for the representation field is described as `user_union_id` |\n\n> Note:\n>   - 1.Currently only single-line comments are supported and comments must be a complete Json data (no line breaks).\n>   - 2.multi line comments are not supported。\n\nWhen these annotations are written, `protobuf_to_pydantic` will bring the corresponding information for each field when converting the Message into the corresponding `Pydantic.BaseModel` object, as follows:\n\n```python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage, parse_msg_desc_method=demo_pb2)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   \'uid\': FieldInfo(default=PydanticUndefined, title=\'UID\', description=\'user union id\', extra={\'example\': \'10086\'}),\n#   \'age\': FieldInfo(default=0, title=\'use age\', ge=0, extra={\'example\': 18}),\n#   \'height\': FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   \'sex\': FieldInfo(default=0, extra={}),\n#   \'is_adult\': FieldInfo(default=False, extra={}),\n#   \'user_name\': FieldInfo(default=\'\', description=\'user name\', min_length=1, max_length=10, extra={\'example\': \'so1n\'})\n# }\n```\nIt can be seen from the output results that the output fields carry the corresponding information. In addition, the difference between this code and the above is that the `msg_to_pydantic_model` function sets a keyword parameter named `parse_msg_desc_method` and its value is `demo_pb2`, which enables `protobuf_to_pydantic` to obtain additional information for each field in the Message object through comments in the `.pyi` file of the `demo_pb2` module.\n\n> Note：This function requires the use of the [mypy-protobuf](https://github.com/nipunn1313/mypy-protobuf) plugin when generating the corresponding `Python` code from the Protobuf file, and the specified output path of the pyi file is the same as the generated `Python` code path to take effect at the same time.\n\nIn addition to obtaining comments through the `.pyi` file, `protobuf_to_pydantic` also supports setting the value of `parse_msg_desc_method` to the root directory path specified when the Message object is generated, so that `protobuf_to_pydantic` can parse the comments of the Protobuf file corresponding to the Message object. getting information。\n\n\nFor example, the project structure of the `protobuf_to_pydantic` sample code is as follows:\n```bash\n./protobuf_to_pydantic/\n├── example/\n│ ├── python_example_proto_code/\n│ └── example_proto/\n├── protobuf_to_pydantic/\n└── /\n```\n\nThe Protobuf file is stored in the `example/example_proto` folder, and then run the following command in the `example` directory to generate the `Python` code file corresponding to Protobuf:\n```bash\ncd example\n\npython -m grpc_tools.protoc\n  --python_out=./python_example_proto_code \\\n  --grpc_python_out=./python_example_proto_code \\\n  -I. \\\n```\nThen the path to be filled in at this time is `./protobuf_to_pydantic/example`, the code is as follows：\n\n```python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.UserMessage, parse_msg_desc_method="./protobuf_to_pydantic/example"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   \'uid\': FieldInfo(default=PydanticUndefined, title=\'UID\', description=\'user union id\', extra={\'example\': \'10086\'}),\n#   \'age\': FieldInfo(default=0, title=\'use age\', ge=0, extra={\'example\': 18}),\n#   \'height\': FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   \'sex\': FieldInfo(default=0, extra={}),\n#   \'is_adult\': FieldInfo(default=False, extra={}),\n#   \'user_name\': FieldInfo(default=\'\', description=\'user name\', min_length=1, max_length=10, extra={\'example\': \'so1n\'})\n# }\n```\nFrom the result, it can be seen that the information carried by the field is the same as the result obtained by the module\n> NOTE: This method requires [lark](https://github.com/lark-parser/lark) to be installed in advance and the Protobuf file must exist in the running project.\n\n### 2.3.2.PGV(protoc-gen-validate)\nCurrently, the commonly used object validation method in the Protobuf ecosystem is to directly use the [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate) project, while [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate) project also supports multiple languages, and most Protobuf developers will write `pgv` rules once so that different languages support the same validation rules.\n\nAnd `protobuf-to-pydantic` also supports parsing the verification rules of `pgv` so that the generated `pydantic.BaseModel` class has corresponding verification logic,\nIt is very simple to use `Pgv` verification rules in `protobuf_to_pydantic`. First, you need to write the corresponding `Pgv` rules in the Protobuf file, and then fill in `parse_msg_desc_method` when converting through `msg_to_pydantic_model` method The value is `PGV`, the code is as follows:\n```Python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.validate import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest, parse_msg_desc_method="PGV"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   \'const_test\': FieldInfo(default=1.0, const=True, extra={}),\n#   \'range_e_test\': FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   \'range_test\': FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   \'in_test\': FieldInfo(default=0.0, extra={\'in\': [1.0, 2.0, 3.0]}),\n#   \'not_in_test\': FieldInfo(default=0.0, extra={\'not_in\': [1.0, 2.0, 3.0]}),\n#   \'ignore_test\': FieldInfo(default=0.0, extra={})\n# }\n```\n\n> Note:\n>  - 1.For the usage of `Pgv`, see: [protoc-gen-validate doc](https://github.com/bufbuild/protoc-gen-validate/blob/main/README.md#constraint-rules)\n>  - 2.Need to install `Pgv` through `pip install protoc_gen_validate` Or download [validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/common/validate.proto) to the protobuf directory in the project to write pgv rules in the Protobuf file.\n\n\n### 2.2.3.P2p\nThe verification rules of `Pgv` are written in the Option attribute of each field of `Message`, and there are better code specifications, so the readability of Protobuf files carrying `Pgv` verification rules is higher than that of Protobuf carrying comments At the same time, when writing `Pgv` rules, you can also experience the convenience brought by IDE auto-completion, but it only supports verification-related logic, and the feature richness is not as good as the file comment mode.\n\nThe `P2P` mode is an extension of the `PGV` mode, which incorporates some functions of text annotations. This mode satisfies the customization of the attributes of each `Field` in most `pydantic.BaseModel`, such as the following Protobuf file:\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\n\nimport "example_proto/common/p2p_validate.proto";\n\n\nmessage FloatTest {\n  float const_test = 1 [(p2p_validate.rules).float.const = 1];\n  float range_e_test = 2 [(p2p_validate.rules).float = {ge: 1, le: 10}];\n  float range_test = 3[(p2p_validate.rules).float = {gt: 1, lt: 10}];\n  float in_test = 4[(p2p_validate.rules).float = {in: [1,2,3]}];\n  float not_in_test = 5[(p2p_validate.rules).float = {not_in: [1,2,3]}];\n  float default_test = 6[(p2p_validate.rules).float.default = 1.0];\n  float not_enable_test = 7[(p2p_validate.rules).float.enable = false];\n  float default_factory_test = 8[(p2p_validate.rules).float.default_factory = "p2p@builtin|float"];\n  float miss_default_test = 9[(p2p_validate.rules).float.miss_default = true];\n  float alias_test = 10 [(p2p_validate.rules).float.alias = "alias"];\n  float desc_test = 11 [(p2p_validate.rules).float.description = "test desc"];\n  float multiple_of_test = 12 [(p2p_validate.rules).float.multiple_of = 3.0];\n  float example_test = 13 [(p2p_validate.rules).float.example = 1.0];\n  float example_factory = 14 [(p2p_validate.rules).float.example_factory = "p2p@builtin|float"];\n  float field_test = 15[(p2p_validate.rules).float.field = "p2p@local|CustomerField"];\n  float type_test = 16[(p2p_validate.rules).float.type = "p2p@local|confloat"];\n  float title_test = 17 [(p2p_validate.rules).float.title = "title_test"];\n}\n```\n`protobuf_to_pydantic` can read the generated Message object at runtime and generate a `pydantic.BaseModel` object with the corresponding information:\n\n```python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel, confloat\nfrom pydantic.fields import FieldInfo\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.p2p_validate import demo_pb2\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\nDemoModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest,\n    local_dict={"CustomerField": CustomerField, "confloat": confloat},\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in DemoModel.__fields__.items()\n    }\n)\n# output:\n# {\n#   \'const_test\': FieldInfo(default=1.0, const=True, extra={}),\n#   \'range_e_test\': FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   \'range_test\': FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   \'in_test\': FieldInfo(default=0.0, extra={\'in\': [1.0, 2.0, 3.0]}),\n#   \'not_in_test\': FieldInfo(default=0.0, extra={\'not_in\': [1.0, 2.0, 3.0]}),\n#   \'default_test\': FieldInfo(default=1.0, extra={}),\n#   \'default_factory_test\': FieldInfo(default=PydanticUndefined, default_factory=<class \'float\'>, extra={}),\n#   \'miss_default_test\': FieldInfo(extra={}),\n#   \'alias_test\': FieldInfo(default=0.0, alias=\'alias\', alias_priority=2, extra={}),\n#   \'desc_test\': FieldInfo(default=0.0, description=\'test desc\', extra={}),\n#   \'multiple_of_test\': FieldInfo(default=0.0, multiple_of=3, extra={}),\n#   \'example_test\': FieldInfo(default=0.0, extra={\'example\': 1.0}),\n#   \'example_factory\': FieldInfo(default=0.0, extra={\'example\': <class \'float\'>}),\n#   \'field_test\': CustomerField(default=0.0, extra={}),\n#   \'type_test\': FieldInfo(default=0.0, extra={}),\n#   \'title_test\': FieldInfo(default=0.0, title=\'title_test\', extra={})\n#   }\n```\nIt is worth noting that this code does not explicitly specify that the value of `parse_msg_desc_method` is `p2p`, because `p2p` is already the default rule of `protobuf_to_pydantic`.\n\n> Note: See the template chapter for the usage of `local_dict`\n\n > Note:\n>  - 1.See the template chapter for the usage of `local_dict`\n>  - 2.If the reference to the Proto file fails, you need to download [p2p_validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/protos/protobuf_to_pydantic/protos/p2p_validate.proto) in the project and use it in the Protobuf file。\n\n\n\n\n### 2.3.3.Other parameter support\nIn addition to the parameters of `FieldInfo`, the file comment mode and `p2p` mode of `protobuf_to_pydantic` also support the following parameters:\n- miss_default：By default, the default value of each field in the corresponding `pydantic.BaseModel` object is the same as the default value of each field in the Message, but when `miss default` is `true`, the setting of the default value will be canceled .\n- enable: By default, `pydantic.BaseModel` will convert every field in the Message. If some fields do not want to be converted, you can set `enable` to `false`\n- const: Specifies the value of the field\'s constant. Note: The const of `pydantic.BaseModel` only supports bool variables. When `const` is `True`, the accepted value can only be the value set by `default`, and the default value carried by the Message generated by protobuf corresponds to The null value of type does not match `pydantic.BaseModel`, so `protobuf_to_pydantic` makes some changes to the input of this value, but after `const` sets the value, the `cost` property in the generated field is `True` `, and `default` becomes the corresponding value of the setting.\n- type: To expand the current type, for example, if you want to increase the verification of the bank card number through the `pydantic.types.Payment Card Number` type, you can specify the field type as `Payment Card Number` by the following method:\n  ```protobuf\n  // common example\n  message UserPayMessage {\n    string bank_number=1; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n  }\n  // p2p example\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n  }\n  ```\n\n> Note:\n>   If you don\'t know `pydantic`, you can use the following two URLs to learn what parameters Field supports:\n>\n>   - https://pydantic-docs.helpmanual.io/usage/types/#constrained-types\n>\n>   - https://pydantic-docs.helpmanual.io/usage/schema/#field-customization\n\n### 2.3.4.Template\nIn some cases, the value we fill in is a method or function of a certain library in `Python` (such as the value of `type` parameter and `default_factory` parameter), which cannot be realized through Json syntax。\nAt this time, template parameters can be used to solve the corresponding problems. Currently `protobuf_to_pydantic` supports a variety of template parameters。\n\n> Note:The `p2p` string at the beginning of the template can be defined by the comment prefix variable\n\n\n#### 2.3.4.1.`p2p@import`\nThis template is used to indicate that the value is a variable under other modules. The specific usage method is as follows:\n```protobuf\n// comment example\nmessage UserPayMessage {\n  string bank_number=1; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n}\n\n// p2p example\nmessage UserPayMessage {\n  string bank_number=1[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n}\n\n// p2p other example\n// Since the imported type happens to belong to the `pydantic.types` module, string.pydantic type can be used directly in `p2p` mode\nmessage UserPayMessage {\n  string bank_number=1[(p2p_validate.rules).string.pydantic_type = "PaymentCardNumber"];\n}\n```\n\nThe syntax in the format of `p2p{template method}|{module to be imported: A}|{variable in the module: B}` is used here, which means that `B` object needs to be imported and applied through `from A import B` ,\nThrough the definition of the template, `protobuf_to_pydantic` will convert the corresponding Message into the following `pydantic.BaseModel`:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n# p2p@import|pydantic.types|PaymentCardNumber\nfrom pydantic.types import PaymentCardNumber\n\nclass UserPayMessage(BaseModel):\n    bank_number: PaymentCardNumber = FieldInfo(default="", extra={})\n```\n\n#### 2.3.4.2.`p2p@import_instance`\nThe `p2p@import` template just imports and uses the variables of a certain library, while `p2p@import instance` imports the class of a certain library first,\nand finally instantiates it with the specified parameters. The method of use is as follows:\n```protobuf\nmessage AnyTest {\n  google.protobuf.Any default_test = 23 [\n    (p2p_validate.rules).any.default = \'p2p@import_instance|google.protobuf.any_pb2|Any|{"type_url": "type.googleapis.com/google.protobuf.Duration"}\'\n\n  ];\n}\n```\nHere is the `p2p{template method}|{module to be imported}|{corresponding class}|{corresponding parameter}` syntax, through the definition of the template, `protobuf_to_pydantic` will convert the corresponding Message is the following `pydantic.BaseModel` object:\n```python\nfrom google.protobuf.any_pb2 import Any as AnyMessage\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass AnyTest(BaseModel):\n    default_test: AnyMessage = FieldInfo(\n        default=AnyMessage(type_url="type.googleapis.com/google.protobuf.Duration")\n    )\n```\n\n#### 2.3.4.3.`p2p@local`\nThis template is used to introduce user-defined variables. The syntax in the format `{template method}|{local variable to be used}` is used here, as follows:\n```protobuf\n// comment example\nmessage UserPayMessage {\n  google.protobuf.Timestamp exp=1; // p2p: {"default_factory": "p2p@local|exp_time"}\n}\n// p2p example\nmessage UserPayMessage {\n  google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.default_factory= "p2p@local|exp_time"];\n}\n```\nThen register the corresponding value through the parameter `local_dict` when calling the `msg_to_pydantic_model` method. The fake code is as follows:\n```Python\nimport time\n\n\ndef exp_time() -> float:\n  return time.time()\n\nmsg_to_pydantic_model(\n    demo_pb2.NestedMessage,\n    local_dict={"exp_time": exp_time},  # <----\n)\n```\nIn this way, `protobuf_to_pydantic` can generate a `pydantic.BaseModel` object that meets the requirements:\n```python\nfrom datetime import datetime\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nfrom . import exp_time\n\nclass UserPayMessage(BaseModel):\n    exp: datetime = FieldInfo(default_factory=exp_time, extra={})\n```\n\n> Note: See the sample code for specific calling and generation methods.\n\n#### 2.3.4.4.`p2p@builtin`\nWhen the variable to be used comes from a built-in function, this template can be used directly (it can be considered as a simplified version of the `p2p@local` template), and the syntax is as follows:\n```protobuf\n// comment example\nmessage UserPayMessage {\n  google.protobuf.Timestamp exp=1; // p2p: {"type": "p2p@builtin|float"}\n}\n\n// p2p example\nmessage UserPayMessage {\n  google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.type= "p2p@builtin|float"];\n}\n```\nIn this way, `protobuf_to_pydantic` can generate a `pydantic.BaseModel` object that meets the requirements:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass UserPayMessage(BaseModel):\n    exp: float = FieldInfo()\n```\n#### 2.3.4.5.Custom template\nCurrently, `protobuf_to_pydantic` only supports several templates. If you have more template requirements, you can extend the template by inheriting the `DescTemplate` class.\nFor example, there is a strange requirement that the default value of the field is the timestamp when the Message object is generated as a `pydantic.BaseModel` object, but the timestamp has two versions, one version has a timestamp of length 10 and the other has a length of 13, so write the following Protobuf file:\n```protobuf\nmessage TimestampTest{\n  int32 timestamp_10 = 1[(p2p_validate.rules).int32.default = "p2p@timestamp|10"];\n  int32 timestamp_13 = 2[(p2p_validate.rules).int32.default = "p2p@timestamp|13"];\n}\n```\nThis file uses the custom `p2p@timestamp|{x}` syntax, where `x` only has two values of 10 and 13, and then you can write code according to this template behavior, the code is as follows:\n```python\nimport time\nfrom typing import Any, List\nfrom protobuf_to_pydantic.gen_model import DescTemplate\n\n\nclass CustomDescTemplate(DescTemplate):\n    def template_timestamp(self, template_var_list: List[str]) -> Any:\n        timestamp: float = time.time()\n        length: str = template_var_list[0]\n        if length == "10":\n            return int(timestamp)\n        elif length == "13":\n            return int(timestamp * 100)\n        else:\n            raise KeyError(f"timestamp template not support value:{length}")\n\n\nfrom .demo_pb2 import TimestampTest # fake code\nfrom protobuf_to_pydantic import msg_to_pydantic_model\n\nmsg_to_pydantic_model(\n    TimestampTest,\n    desc_template=CustomDescTemplate\n)\n```\nThis code first creates a `CustomDescTemplate` class inherited from `DescTemplate`, and this class adds a `template_timestamp` method to match the syntax of `p2p@timestamp`,\nThen specify the template class as `CustomDescTemplate` through the `desc_template` key parameter in `msg_to_pydantic_model`, so that `msg_to_pydantic_model` will generate the following code (assuming the code generated when the timestamp is 1600000000 ):\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nclass TimestampTest(BaseModel):\n    timestamp_10: int = FieldInfo(default=1600000000)\n    timestamp_13: int = FieldInfo(default=1600000000000)\n```\n\n## 3.Code formatting\nCode generated directly via `protobuf_to_pydantic` is not perfect, but `protobuf+type_pydantic` can rely on different formatting tools to generate code that conforms to the `Python` specification.\nCurrently supported formatting tools are `autoflake`, `black` and `isort`, but the prerequisite for using these tools is that the corresponding formatting tools are installed in the current running environment.\n\nIn addition, developers can decide how the formatter will execute through the `pyproject.toml` configuration file, an example of `pyproject.toml` as follows:\n```toml\n# Controls which formatters protobuf-to-pydantic can use, false means that the formatter is not used (default is true)\n[tool.protobuf-to-pydantic.format]\nblack = true\nisort = true\nautoflake = true\n\n# See the black configuration documentation:https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-format\n[tool.black]\nline-length = 120\ntarget-version = [\'py37\']\n\n# See the isort configuration documentation:https://pycqa.github.io/isort/docs/configuration/config_files.html#pyprojecttoml-preferred-format\n[tool.isort]\nprofile = "black"\nmulti_line_output = 3\ninclude_trailing_comma = true\nforce_grid_wrap = 0\nuse_parentheses = true\nensure_newline_before_comments = true\nline_length = 120\n\n# See the autoflake configuration documentation:https://github.com/PyCQA/autoflake#configuration\n[tool.autoflake]\nin-place = true\nremove-all-unused-imports = true\nremove-unused-variables = true\n```\n\n## 4.example\n`protobuf_to_pydantic` provides some simple sample code, the following is the path of the sample code and protobuf file, just for reference:\n\n| Implication                           | Example Protobuf                                                                            | Example code                                                                         |\n|------------------------------|---------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|\n| Generate Model code with validation rules based on p2p schema | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/example_proto/p2p_validate | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/p2p_validate_example |\n| Generate the basic Model code               | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/example_proto/demo         | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/simple_example      |\n| Generate Model code with validation rules from .pyi files     | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/example_proto/demo         | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/text_comment_example |\n| Generate Model code with validation rules from protobuf files | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/example_proto/validate     | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/validate_example    |\n',
     'author': 'So1n',
     'author_email': 'so1n897046026@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/so1n/protobuf_to_pydantic',
```

### Comparing `protobuf_to_pydantic-0.1.7/PKG-INFO` & `protobuf_to_pydantic-0.1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf-to-pydantic
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Convert Protobuf-generated Python objects to Pydantic.BaseModel objects with parameter checksum
 Home-page: https://github.com/so1n/protobuf_to_pydantic
 License: Apache Software License
 Author: So1n
 Author-email: so1n897046026@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

