# Comparing `tmp/syft-0.8.0b5.tar.gz` & `tmp/syft-0.8.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.0b5.tar", last modified: Sun Apr  2 12:34:23 2023, max compression
+gzip compressed data, was "syft-0.8.0b6.tar", last modified: Sun Apr  9 12:33:59 2023, max compression
```

## Comparing `syft-0.8.0b5.tar` & `syft-0.8.0b6.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.951447 syft-0.8.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-02 12:32:15.000000 syft-0.8.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-02 12:32:15.000000 syft-0.8.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-02 12:34:23.951447 syft-0.8.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-02 12:32:15.000000 syft-0.8.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-02 12:32:15.000000 syft-0.8.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-02 12:34:23.951447 syft-0.8.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-02 12:32:15.000000 syft-0.8.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.903446 syft-0.8.0b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.915446 syft-0.8.0b5/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-02 12:32:27.000000 syft-0.8.0b5/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-02 12:32:27.000000 syft-0.8.0b5/src/syft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.919446 syft-0.8.0b5/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.919446 syft-0.8.0b5/src/syft/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.919446 syft-0.8.0b5/src/syft/core/node/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.947447 syft-0.8.0b5/src/syft/core/node/new/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    26475 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/data_subject_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/dataset_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/metadata_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/node_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/project_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/sqlite_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/third_party.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/user_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/new/worker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    24026 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/core/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/experimental_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.947447 syft-0.8.0b5/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.951447 syft-0.8.0b5/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15416 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/gevent_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/user_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-02 12:32:15.000000 syft-0.8.0b5/src/syft/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 12:34:23.919446 syft-0.8.0b5/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-02 12:34:23.000000 syft-0.8.0b5/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-02 12:34:23.000000 syft-0.8.0b5/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 12:34:23.000000 syft-0.8.0b5/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 12:34:23.000000 syft-0.8.0b5/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-02 12:34:23.000000 syft-0.8.0b5/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-02 12:34:23.000000 syft-0.8.0b5/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.383129 syft-0.8.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-09 12:31:26.000000 syft-0.8.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 12:31:26.000000 syft-0.8.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-09 12:33:59.383129 syft-0.8.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-09 12:31:24.000000 syft-0.8.0b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-09 12:31:26.000000 syft-0.8.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-09 12:33:59.387129 syft-0.8.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-09 12:31:26.000000 syft-0.8.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.359127 syft-0.8.0b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.363127 syft-0.8.0b6/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-09 12:31:42.000000 syft-0.8.0b6/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-09 12:31:42.000000 syft-0.8.0b6/src/syft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.367128 syft-0.8.0b6/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.367128 syft-0.8.0b6/src/syft/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.367128 syft-0.8.0b6/src/syft/core/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.383129 syft-0.8.0b6/src/syft/core/node/new/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26475 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/data_subject_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/dataset_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/metadata_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/node_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/project_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/sqlite_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/third_party.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23989 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/user_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/new/worker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23988 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/core/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/experimental_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.383129 syft-0.8.0b6/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.383129 syft-0.8.0b6/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15416 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/gevent_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-09 12:31:26.000000 syft-0.8.0b6/src/syft/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:33:59.367128 syft-0.8.0b6/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:33:59.000000 syft-0.8.0b6/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.0b5/LICENSE` & `syft-0.8.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/PKG-INFO` & `syft-0.8.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b5
+Version: 0.8.0b6
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b5 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.0b6 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.0b5/README.md` & `syft-0.8.0b6/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/setup.cfg` & `syft-0.8.0b6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.0-beta.5"
+version = attr: "0.8.0-beta.6"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.0b5/src/syft/VERSION` & `syft-0.8.0b6/src/syft/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.0-beta.5"
+__version__ = "0.8.0-beta.6"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.0b5/src/syft/__init__.py` & `syft-0.8.0b6/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     IMPORTANT: syft.core should be very careful when importing functionality from outside of syft
     core!!! Since we plan to drop syft core down to a language (such as C++ or Rust)
     this can create future complications with lower level languages calling
     higher level ones.
 To begin your education in Syft, continue to the :py:mod:`syft.core.node.vm.vm` module...
 """
 
-__version__ = "0.8.0-beta.5"
+__version__ = "0.8.0-beta.6"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
```

### Comparing `syft-0.8.0b5/src/syft/core/node/__init__.py` & `syft-0.8.0b6/src/syft/core/node/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/action_object.py` & `syft-0.8.0b6/src/syft/core/node/new/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/action_service.py` & `syft-0.8.0b6/src/syft/core/node/new/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/action_store.py` & `syft-0.8.0b6/src/syft/core/node/new/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/action_types.py` & `syft-0.8.0b6/src/syft/core/node/new/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/api.py` & `syft-0.8.0b6/src/syft/core/node/new/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/array.py` & `syft-0.8.0b6/src/syft/core/node/new/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/arrow.py` & `syft-0.8.0b6/src/syft/core/node/new/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/client.py` & `syft-0.8.0b6/src/syft/core/node/new/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/connection.py` & `syft-0.8.0b6/src/syft/core/node/new/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/context.py` & `syft-0.8.0b6/src/syft/core/node/new/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/credentials.py` & `syft-0.8.0b6/src/syft/core/node/new/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/data_subject.py` & `syft-0.8.0b6/src/syft/core/node/new/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/data_subject_member.py` & `syft-0.8.0b6/src/syft/core/node/new/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/data_subject_member_service.py` & `syft-0.8.0b6/src/syft/core/node/new/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/data_subject_service.py` & `syft-0.8.0b6/src/syft/core/node/new/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/dataset.py` & `syft-0.8.0b6/src/syft/core/node/new/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/dataset_service.py` & `syft-0.8.0b6/src/syft/core/node/new/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/dataset_stash.py` & `syft-0.8.0b6/src/syft/core/node/new/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/datetime.py` & `syft-0.8.0b6/src/syft/core/node/new/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/decorators.py` & `syft-0.8.0b6/src/syft/core/node/new/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/deserialize.py` & `syft-0.8.0b6/src/syft/core/node/new/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/dict_document_store.py` & `syft-0.8.0b6/src/syft/core/node/new/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/document_store.py` & `syft-0.8.0b6/src/syft/core/node/new/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # future
 from __future__ import annotations
 
 # stdlib
 from functools import partial
+import sys
 import types
+import typing
 from typing import Any
 from typing import Dict
-from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
-from typing import _GenericAlias
 
 # third party
 from pydantic import BaseModel
 from result import Err
 from result import Ok
 from result import Result
 from typeguard import check_type
@@ -40,120 +40,125 @@
         name: str
             Identifier to be used as prefix by stores and for partitioning
     """
 
     name: str
 
 
-def first_or_none(result: Any) -> Optional[Any]:
+def first_or_none(result: Any) -> Ok:
     if hasattr(result, "__len__") and len(result) > 0:
         return Ok(result[0])
     return Ok(None)
 
 
+if sys.version_info >= (3, 9):
+
+    def is_generic_alias(t: type):
+        return isinstance(t, (types.GenericAlias, typing._GenericAlias))
+
+else:
+
+    def is_generic_alias(t: type):
+        return isinstance(t, typing._GenericAlias)
+
+
 class StoreClientConfig(BaseModel):
     """Base Client specific configuration"""
 
     pass
 
 
 @serializable()
 class PartitionKey(BaseModel):
     key: str
     type_: Union[type, object]
 
     def __eq__(self, other: Any) -> bool:
-        if type(other) == type(self):
-            return self.key == other.key and self.type_ == other.type_
-        return False
+        return (
+            type(other) == type(self)
+            and self.key == other.key
+            and self.type_ == other.type_
+        )
 
-    def with_obj(self, obj: SyftObject) -> QueryKey:
+    def with_obj(self, obj: Any) -> QueryKey:
         return QueryKey.from_obj(partition_key=self, obj=obj)
 
-    def is_valid_list(self, obj: SyftObject) -> bool:
+    def extract_list(self, obj: Any) -> List:
         # not a list and matches the internal list type of the _GenericAlias
         if not isinstance(obj, list):
-            if not isinstance(obj, self.type_.__args__):
+            if not isinstance(obj, typing.get_args(self.type_)):
                 obj = getattr(obj, self.key)
                 if isinstance(obj, (types.FunctionType, types.MethodType)):
                     obj = obj()
 
-            if not isinstance(obj, list) and isinstance(obj, self.type_.__args__):
+            if not isinstance(obj, list) and isinstance(
+                obj, typing.get_args(self.type_)
+            ):
                 # still not a list but the right type
                 obj = [obj]
 
         # is a list type so lets compare directly
         check_type("obj", obj, self.type_)
         return obj
 
     @property
     def type_list(self) -> bool:
-        if isinstance(self.type_, _GenericAlias) and self.type_.__origin__ == list:
-            return True
-        return False
+        return is_generic_alias(self.type_) and self.type_.__origin__ == list
 
 
 @serializable()
 class PartitionKeys(BaseModel):
-    pks: Union[PartitionKey, Tuple[PartitionKey, ...]]
+    pks: Union[PartitionKey, Tuple[PartitionKey, ...], List[PartitionKey]]
 
     @property
-    def all(self) -> Iterable[PartitionKey]:
-        # make sure we always return Tuple's even if theres a single value
-        _keys = self.pks if isinstance(self.pks, (tuple, list)) else (self.pks,)
-        return _keys
+    def all(self) -> List[PartitionKey]:
+        # make sure we always return a list even if there's a single value
+        return self.pks if isinstance(self.pks, (tuple, list)) else [self.pks]
 
-    def with_obj(self, obj: SyftObject) -> QueryKeys:
+    def with_obj(self, obj: Any) -> QueryKeys:
         return QueryKeys.from_obj(partition_keys=self, obj=obj)
 
-    def with_tuple(self, *args: Tuple[Any, ...]) -> QueryKeys:
+    def with_tuple(self, *args: Any) -> QueryKeys:
         return QueryKeys.from_tuple(partition_keys=self, args=args)
 
     def add(self, pk: PartitionKey) -> PartitionKeys:
         return PartitionKeys(pks=list(self.all) + [pk])
 
     @staticmethod
     def from_dict(cks_dict: Dict[str, type]) -> PartitionKeys:
         pks = []
         for k, t in cks_dict.items():
             pks.append(PartitionKey(key=k, type_=t))
         return PartitionKeys(pks=pks)
 
-    def make(self, *obj_arg: Union[SyftObject, Tuple[Any, ...]]) -> QueryKeys:
-        if isinstance(obj_arg, SyftObject):
-            return self.with_obj(obj_arg)
-        else:
-            return self.with_tuple(*obj_arg)
-
 
 @serializable()
 class QueryKey(PartitionKey):
     value: Any
 
     def __eq__(self, other: Any) -> bool:
-        if type(other) == type(self):
-            return (
-                self.key == other.key
-                and self.type_ == other.type_
-                and self.value == other.value
-            )
-        return False
+        return (
+            type(other) == type(self)
+            and self.key == other.key
+            and self.type_ == other.type_
+            and self.value == other.value
+        )
 
     @property
     def partition_key(self) -> PartitionKey:
         return PartitionKey(key=self.key, type_=self.type_)
 
     @staticmethod
-    def from_obj(partition_key: PartitionKey, obj: SyftObject) -> List[Any]:
+    def from_obj(partition_key: PartitionKey, obj: Any) -> QueryKey:
         pk_key = partition_key.key
         pk_type = partition_key.type_
 
         # 🟡 TODO: support more advanced types than List[type]
         if partition_key.type_list:
-            pk_value = partition_key.is_valid_list(obj)
+            pk_value = partition_key.extract_list(obj)
         else:
             if isinstance(obj, pk_type):
                 pk_value = obj
             else:
                 pk_value = getattr(obj, pk_key)
                 # object has a method for getting these types
                 # we can't use properties because we don't seem to be able to get the
@@ -183,56 +188,55 @@
 
 
 @serializable()
 class PartitionKeysWithUID(PartitionKeys):
     uid_pk: PartitionKey
 
     @property
-    def all(self) -> Iterable[PartitionKey]:
+    def all(self) -> List[PartitionKey]:
         all_keys = self.pks if isinstance(self.pks, (tuple, list)) else [self.pks]
         if self.uid_pk not in all_keys:
             all_keys.insert(0, self.uid_pk)
         return all_keys
 
 
 @serializable()
 class QueryKeys(SyftBaseModel):
-    qks: Union[QueryKey, Tuple[QueryKey, ...]]
+    qks: Union[QueryKey, Tuple[QueryKey, ...], List[QueryKey]]
 
     @property
-    def all(self) -> Iterable[QueryKey]:
-        # make sure we always return Tuple's even if theres a single value
-        _keys = self.qks if isinstance(self.qks, (tuple, list)) else (self.qks,)
-        return _keys
+    def all(self) -> List[QueryKey]:
+        # make sure we always return a list even if there's a single value
+        return self.qks if isinstance(self.qks, (tuple, list)) else [self.qks]
 
     @staticmethod
     def from_obj(partition_keys: PartitionKeys, obj: SyftObject) -> QueryKeys:
         qks = []
         for partition_key in partition_keys.all:
             pk_key = partition_key.key
             pk_type = partition_key.type_
             pk_value = getattr(obj, pk_key)
             # object has a method for getting these types
             # we can't use properties because we don't seem to be able to get the
             # return types
             if isinstance(pk_value, (types.FunctionType, types.MethodType)):
                 pk_value = pk_value()
             if partition_key.type_list:
-                pk_value = partition_key.is_valid_list(obj)
+                pk_value = partition_key.extract_list(obj)
             else:
                 if pk_value and not isinstance(pk_value, pk_type):
                     raise Exception(
                         f"PartitionKey {pk_value} of type {type(pk_value)} must be {pk_type}."
                     )
             qk = QueryKey(key=pk_key, type_=pk_type, value=pk_value)
             qks.append(qk)
         return QueryKeys(qks=qks)
 
     @staticmethod
-    def from_tuple(partition_keys: PartitionKeys, args: Tuple[Any, ...]) -> QueryKeys:
+    def from_tuple(partition_keys: PartitionKeys, args: Tuple) -> QueryKeys:
         qks = []
         for partition_key, pk_value in zip(partition_keys.all, args):
             pk_key = partition_key.key
             pk_type = partition_key.type_
             if not isinstance(pk_value, pk_type):
                 raise Exception(
                     f"PartitionKey {pk_value} of type {type(pk_value)} must be {pk_type}."
@@ -318,22 +322,18 @@
             self.searchable_cks = self.settings.searchable_keys.all
         except BaseException as e:
             return Err(str(e))
 
         return Ok()
 
     def matches_unique_cks(self, partition_key: PartitionKey) -> bool:
-        if partition_key in self.unique_cks:
-            return True
-        return False
+        return partition_key in self.unique_cks
 
     def matches_searchable_cks(self, partition_key: PartitionKey) -> bool:
-        if partition_key in self.searchable_cks:
-            return True
-        return False
+        return partition_key in self.searchable_cks
 
     def store_query_key(self, obj: Any) -> QueryKey:
         return self.settings.store_key.with_obj(obj)
 
     def store_query_keys(self, objs: Any) -> QueryKeys:
         return QueryKeys(qks=[self.store_query_key(obj) for obj in objs])
```

### Comparing `syft-0.8.0b5/src/syft/core/node/new/grid_url.py` & `syft-0.8.0b6/src/syft/core/node/new/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/kv_document_store.py` & `syft-0.8.0b6/src/syft/core/node/new/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/linked_obj.py` & `syft-0.8.0b6/src/syft/core/node/new/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/locks.py` & `syft-0.8.0b6/src/syft/core/node/new/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/message_service.py` & `syft-0.8.0b6/src/syft/core/node/new/message_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/message_stash.py` & `syft-0.8.0b6/src/syft/core/node/new/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/messages.py` & `syft-0.8.0b6/src/syft/core/node/new/messages.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/metadata_service.py` & `syft-0.8.0b6/src/syft/core/node/new/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/metadata_stash.py` & `syft-0.8.0b6/src/syft/core/node/new/metadata_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/mongo_client.py` & `syft-0.8.0b6/src/syft/core/node/new/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/mongo_codecs.py` & `syft-0.8.0b6/src/syft/core/node/new/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/mongo_document_store.py` & `syft-0.8.0b6/src/syft/core/node/new/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/network_service.py` & `syft-0.8.0b6/src/syft/core/node/new/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/node.py` & `syft-0.8.0b6/src/syft/core/node/new/node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/node_metadata.py` & `syft-0.8.0b6/src/syft/core/node/new/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/numpy.py` & `syft-0.8.0b6/src/syft/core/node/new/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/pandas.py` & `syft-0.8.0b6/src/syft/core/node/new/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/project.py` & `syft-0.8.0b6/src/syft/core/node/new/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/project_service.py` & `syft-0.8.0b6/src/syft/core/node/new/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/project_stash.py` & `syft-0.8.0b6/src/syft/core/node/new/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/queue_stash.py` & `syft-0.8.0b6/src/syft/core/node/new/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/recursive.py` & `syft-0.8.0b6/src/syft/core/node/new/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/recursive_primitives.py` & `syft-0.8.0b6/src/syft/core/node/new/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/request.py` & `syft-0.8.0b6/src/syft/core/node/new/request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/request_service.py` & `syft-0.8.0b6/src/syft/core/node/new/request_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,18 +48,19 @@
     ) -> Union[Request, SyftError]:
         """Submit a Request"""
         try:
             result = self.stash.set(request.to(Request, context=context))
             if result.is_ok():
                 request = result.ok()
                 link = LinkedObject.with_context(request, context=context)
-                user_verify_key = context.node.get_service_method(
-                    UserService.user_verify_key
+                admin_verify_key = context.node.get_service_method(
+                    UserService.admin_verify_key
                 )
-                root_verify_key = user_verify_key(email="info@openmined.org")
+
+                root_verify_key = admin_verify_key()
                 if send_message:
                     message = CreateMessage(
                         subject="Approval Request",
                         from_user_verify_key=context.credentials,
                         to_user_verify_key=root_verify_key,
                         linked_obj=link,
                     )
```

### Comparing `syft-0.8.0b5/src/syft/core/node/new/request_stash.py` & `syft-0.8.0b6/src/syft/core/node/new/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/response.py` & `syft-0.8.0b6/src/syft/core/node/new/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/serializable.py` & `syft-0.8.0b6/src/syft/core/node/new/serializable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # stdlib
+from typing import List
 from typing import Optional
-from typing import Sequence
 from typing import TypeVar
 
 # syft absolute
 import syft
 
 # relative
 from .recursive import recursive_serde_register
 
 module_type = type(syft)
 
 
-T = TypeVar("T")
+T = TypeVar("T", bound=type)
 
 
 def serializable(
-    attrs: Sequence[str] = [],
-    without: Sequence[str] = [],
+    attrs: Optional[List[str]] = None,
+    without: Optional[List[str]] = None,
     inherit: Optional[bool] = True,
     inheritable: Optional[bool] = True,
 ) -> T:
     """
     Recursively serialize attributes of the class.
 
     Args:
```

### Comparing `syft-0.8.0b5/src/syft/core/node/new/service.py` & `syft-0.8.0b6/src/syft/core/node/new/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/signature.py` & `syft-0.8.0b6/src/syft/core/node/new/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/sqlite_document_store.py` & `syft-0.8.0b6/src/syft/core/node/new/sqlite_document_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         ddtype: Optional[type] = None,
     ) -> None:
         self.index_name = index_name
         self.settings = settings
         self.store_config = store_config
         self._ddtype = ddtype
         self._db: Dict[int, sqlite3.Connection] = {}
-        self._cur: Dict[int, sqlite3.Connection] = {}
+        self._cur: Dict[int, sqlite3.Cursor] = {}
         self.create_table()
 
     @property
     def table_name(self) -> str:
         return f"{self.settings.name}_{self.index_name}"
 
     def _connect(self) -> None:
@@ -308,28 +308,32 @@
             data corruption.
         `timeout`: int
             How many seconds the connection should wait before raising an exception, if the database
             is locked by another connection. If another connection opens a transaction to modify the
             database, it will be locked until that transaction is committed. Default five seconds.
     """
 
-    filename: Optional[str]
-    path: Optional[Union[str, Path]] = None
+    filename: Optional[str] = None
+    path: Union[str, Path]
     check_same_thread: bool = True
     timeout: int = 5
 
-    @property
-    def temp_path(self) -> str:
-        return tempfile.gettempdir()
+    def __init__(
+        self,
+        filename: Optional[str] = None,
+        path: Optional[Union[str, Path]] = None,
+        *args,
+        **kwargs,
+    ):
+        path_ = tempfile.gettempdir() if path is None else path
+        super().__init__(filename=filename, path=path_, *args, **kwargs)
 
     @property
-    def file_path(self) -> str:
-        path = self.path if self.path else self.temp_path
-        path = Path(path)
-        return path / self.filename
+    def file_path(self) -> Optional[Path]:
+        return Path(self.path) / self.filename if self.filename is not None else None
 
 
 @serializable()
 class SQLiteStoreConfig(StoreConfig):
     """SQLite Store config, used by SQLiteStorePartition
 
     Parameters:
```

### Comparing `syft-0.8.0b5/src/syft/core/node/new/syft_object.py` & `syft-0.8.0b6/src/syft/core/node/new/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/test_service.py` & `syft-0.8.0b6/src/syft/core/node/new/test_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/third_party.py` & `syft-0.8.0b6/src/syft/core/node/new/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/transforms.py` & `syft-0.8.0b6/src/syft/core/node/new/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/twin_object.py` & `syft-0.8.0b6/src/syft/core/node/new/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/uid.py` & `syft-0.8.0b6/src/syft/core/node/new/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/user.py` & `syft-0.8.0b6/src/syft/core/node/new/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/user_code.py` & `syft-0.8.0b6/src/syft/core/node/new/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/user_code_parse.py` & `syft-0.8.0b6/src/syft/core/node/new/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/user_code_service.py` & `syft-0.8.0b6/src/syft/core/node/new/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/user_code_stash.py` & `syft-0.8.0b6/src/syft/core/node/new/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/user_roles.py` & `syft-0.8.0b6/src/syft/core/node/new/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/user_service.py` & `syft-0.8.0b6/src/syft/core/node/new/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/user_stash.py` & `syft-0.8.0b6/src/syft/core/node/new/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/util.py` & `syft-0.8.0b6/src/syft/core/node/new/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/verification.py` & `syft-0.8.0b6/src/syft/core/node/new/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/new/worker_settings.py` & `syft-0.8.0b6/src/syft/core/node/new/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/core/node/worker.py` & `syft-0.8.0b6/src/syft/core/node/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # third party
 import gevent
 import gipc
 from gipc.gipc import _GIPCDuplexHandle
 from nacl.signing import SigningKey
 from result import Err
 from result import Result
+from typing_extensions import Self
 
 # relative
 from ... import __version__
 from ...external import OBLV
 from ...telemetry import instrument
 from ...util import random_name
 from .new.action_service import ActionService
@@ -190,65 +191,66 @@
             create_oblv_key_pair(worker=self)
 
         self.services = services
         self._construct_services()
 
         create_admin_new(  # nosec B106
             name="Jane Doe",
-            email="info@openmined.org",
-            password="changethis",
+            email=root_email,
+            password=root_password,
             node=self,
         )
 
         self.client_cache = {}
         self.node_type = node_type
 
         self.post_init()
 
-    @staticmethod
+    @classmethod
     def named(
+        cls,
         name: str,
         processes: int = 0,
         reset: bool = False,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
-    ) -> Worker:
+    ) -> Self:
         name_hash = hashlib.sha256(name.encode("utf8")).digest()
         uid = UID(name_hash[0:16])
         key = SyftSigningKey(SigningKey(name_hash))
         if reset:
             store_config = SQLiteStoreClientConfig()
             store_config.filename = f"{uid}.sqlite"
             with contextlib.suppress(FileNotFoundError):
                 if os.path.exists(store_config.file_path):
                     os.unlink(store_config.file_path)
 
-        return Worker(
+        return cls(
             name=name,
             id=uid,
             signing_key=key,
             processes=processes,
             local_db=local_db,
             sqlite_path=sqlite_path,
         )
 
     def is_root(self, credentials: SyftVerifyKey) -> bool:
         return credentials == self.signing_key.verify_key
 
     @property
-    def root_client(self) -> Any:
+    def root_client(self):
         # relative
         from .new.client import PythonConnection
         from .new.client import SyftClient
 
         connection = PythonConnection(node=self)
         return SyftClient(connection=connection, credentials=self.signing_key)
 
     @property
-    def guest_client(self) -> Any:
+    def guest_client(self):
         # relative
         from .new.client import PythonConnection
         from .new.client import SyftClient
 
         connection = PythonConnection(node=self)
         return SyftClient(connection=connection, credentials=SyftSigningKey.generate())
 
@@ -274,15 +276,14 @@
                 document_store_config = SQLiteStoreConfig(client_config=client_config)
             else:
                 document_store_config = DictStoreConfig()
         if (
             isinstance(document_store_config, SQLiteStoreConfig)
             and document_store_config.client_config.filename is None
         ):
-            document_store_config.client_config.filename
             document_store_config.client_config.filename = f"{self.id}.sqlite"
             print(
                 f"SQLite Store Path:\n!open file://{document_store_config.client_config.file_path}\n"
             )
         document_store = document_store_config.store_type
         self.document_store_config = document_store_config
```

### Comparing `syft-0.8.0b5/src/syft/deploy.py` & `syft-0.8.0b6/src/syft/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/experimental_flags.py` & `syft-0.8.0b6/src/syft/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/__init__.py` & `syft-0.8.0b6/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/oblv/__init__.py` & `syft-0.8.0b6/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/oblv/deployment.py` & `syft-0.8.0b6/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/oblv/deployment_client.py` & `syft-0.8.0b6/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/oblv/exceptions.py` & `syft-0.8.0b6/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/oblv/oblv_keys.py` & `syft-0.8.0b6/src/syft/external/oblv/oblv_keys.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.0b6/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.0b6/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/external/oblv/oblv_service.py` & `syft-0.8.0b6/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/filterwarnings.py` & `syft-0.8.0b6/src/syft/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/gevent_patch.py` & `syft-0.8.0b6/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/logger.py` & `syft-0.8.0b6/src/syft/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/registry.py` & `syft-0.8.0b6/src/syft/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/search.py` & `syft-0.8.0b6/src/syft/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/telemetry.py` & `syft-0.8.0b6/src/syft/telemetry.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 # stdlib
 import os
+from typing import Callable
 from typing import Optional
+from typing import TypeVar
+from typing import Union
+
+# third party
+from typing_extensions import Concatenate
+from typing_extensions import ParamSpec
 
 
 def str_to_bool(bool_str: Optional[str]) -> bool:
     result = False
     bool_str = str(bool_str).lower()
     if bool_str == "true" or bool_str == "1":
         result = True
     return result
 
 
 TRACE_MODE = str_to_bool(os.environ.get("TRACE", "False"))
 
 
-def setup_tracer():
+T = TypeVar("T", bound=Union[Callable, type])
+P = ParamSpec("P")
+
+
+def setup_tracer() -> Callable[Concatenate[T, P], T]:
     if not TRACE_MODE:
 
-        def noop(func):
+        def noop(func: T) -> T:
             return func
 
         return noop
 
     print("OpenTelemetry Tracing enabled")
     service_name = os.environ.get("SERVICE_NAME", "client")
     jaeger_host = os.environ.get("JAEGER_HOST", "localhost")
```

### Comparing `syft-0.8.0b5/src/syft/trace_decorator.py` & `syft-0.8.0b6/src/syft/trace_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import asyncio
 from functools import wraps
 import inspect
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import TypeVar
+from typing import Union
 
 # third party
 from opentelemetry import trace
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Tracer
 
 
@@ -33,25 +34,25 @@
 
     @staticmethod
     def set_default_attributes(attributes: Dict[str, str] = None):
         for att in attributes:
             TracingDecoratorOptions.default_attributes[att] = attributes[att]
 
 
-T = TypeVar("T")
+T = TypeVar("T", bound=Optional[Union[Callable, type]])
 
 
 def instrument(
-    _func_or_class: Optional[T] = None,
+    _func_or_class: T = None,
     *,
     span_name: str = "",
     record_exception: bool = True,
     attributes: Optional[Dict[str, str]] = None,
     existing_tracer: Optional[Tracer] = None,
-    ignore=False
+    ignore=False,
 ):
     """
     A decorator to instrument a class or function with an OTEL tracing span.
     :param cls: internal, used to specify scope of instrumentation
     :param _func_or_class: The function or span to instrument, this is automatically assigned
     :param span_name: Specify the span name explicitly, rather than use the naming convention.
     This parameter has no effect for class decorators: str
```

### Comparing `syft-0.8.0b5/src/syft/user_settings.py` & `syft-0.8.0b6/src/syft/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/util.py` & `syft-0.8.0b6/src/syft/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft/version_compare.py` & `syft-0.8.0b6/src/syft/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft.egg-info/PKG-INFO` & `syft-0.8.0b6/src/syft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.0b5
+Version: 0.8.0b6
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.0b5 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.0b6 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.0b5/src/syft.egg-info/SOURCES.txt` & `syft-0.8.0b6/src/syft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syft-0.8.0b5/src/syft.egg-info/requires.txt` & `syft-0.8.0b6/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

