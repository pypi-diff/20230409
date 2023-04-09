# Comparing `tmp/runtimepy-1.1.1.tar.gz` & `tmp/runtimepy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-1.1.1.tar", last modified: Sat Apr  8 08:38:53 2023, max compression
+gzip compressed data, was "runtimepy-1.2.0.tar", last modified: Sun Apr  9 08:16:17 2023, max compression
```

## Comparing `runtimepy-1.1.1.tar` & `runtimepy-1.2.0.tar`

### file list

```diff
@@ -1,125 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.719376 runtimepy-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 08:36:54.000000 runtimepy-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-08 08:38:53.719376 runtimepy-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-08 08:36:54.000000 runtimepy-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-08 08:36:54.000000 runtimepy-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.699376 runtimepy-1.1.1/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.703376 runtimepy-1.1.1/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.703376 runtimepy-1.1.1/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/channel/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/channel/environment/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.703376 runtimepy-1.1.1/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.703376 runtimepy-1.1.1/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.703376 runtimepy-1.1.1/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.691376 runtimepy-1.1.1/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.703376 runtimepy-1.1.1/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.707376 runtimepy-1.1.1/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.707376 runtimepy-1.1.1/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/mixins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.707376 runtimepy-1.1.1/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.707376 runtimepy-1.1.1/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/arbiter/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/arbiter/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.707376 runtimepy-1.1.1/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/tcp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.707376 runtimepy-1.1.1/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.711376 runtimepy-1.1.1/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/udp/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.711376 runtimepy-1.1.1/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.711376 runtimepy-1.1.1/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.711376 runtimepy-1.1.1/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.711376 runtimepy-1.1.1/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.715376 runtimepy-1.1.1/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.715376 runtimepy-1.1.1/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.715376 runtimepy-1.1.1/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.715376 runtimepy-1.1.1/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/task/basic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.715376 runtimepy-1.1.1/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.715376 runtimepy-1.1.1/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.715376 runtimepy-1.1.1/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-08 08:36:54.000000 runtimepy-1.1.1/runtimepy/tui/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.699376 runtimepy-1.1.1/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-08 08:38:53.000000 runtimepy-1.1.1/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-08 08:38:53.000000 runtimepy-1.1.1/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 08:38:53.000000 runtimepy-1.1.1/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-08 08:38:53.000000 runtimepy-1.1.1/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-08 08:38:53.000000 runtimepy-1.1.1/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 08:38:53.000000 runtimepy-1.1.1/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 08:38:53.719376 runtimepy-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-08 08:36:54.000000 runtimepy-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 08:38:53.719376 runtimepy-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-08 08:36:54.000000 runtimepy-1.1.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-08 08:36:54.000000 runtimepy-1.1.1/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-08 08:36:54.000000 runtimepy-1.1.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.256465 runtimepy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 08:14:51.000000 runtimepy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-09 08:16:17.256465 runtimepy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-09 08:14:51.000000 runtimepy-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-09 08:14:51.000000 runtimepy-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.240465 runtimepy-1.2.0/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.240465 runtimepy-1.2.0/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/environment/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.236465 runtimepy-1.2.0/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/mixins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.244464 runtimepy-1.2.0/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/udp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.248465 runtimepy-1.2.0/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.252465 runtimepy-1.2.0/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.252465 runtimepy-1.2.0/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.252465 runtimepy-1.2.0/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/task/basic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.252465 runtimepy-1.2.0/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.256465 runtimepy-1.2.0/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.256465 runtimepy-1.2.0/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-09 08:14:51.000000 runtimepy-1.2.0/runtimepy/tui/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.240465 runtimepy-1.2.0/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 08:16:17.000000 runtimepy-1.2.0/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:16:17.256465 runtimepy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-09 08:14:51.000000 runtimepy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:16:17.256465 runtimepy-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-09 08:14:51.000000 runtimepy-1.2.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-09 08:14:51.000000 runtimepy-1.2.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-09 08:14:51.000000 runtimepy-1.2.0/tests/test_resources.py
```

### Comparing `runtimepy-1.1.1/LICENSE` & `runtimepy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/PKG-INFO` & `runtimepy-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.1.1
+Version: 1.2.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=182b46b499d24cb62c9688e373b88345
+    hash=ce3f1316217e521947cc4b3047971525
     =====================================
 -->
 
-# runtimepy ([1.1.1](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.2.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
@@ -64,28 +64,63 @@
 # Introduction
 
 # Command-line Options
 
 ```
 $ ./venv3.8/bin/runtimepy -h
 
-usage: runtimepy [-h] [--version] [-v] [-C DIR] {tui,noop} ...
+usage: runtimepy [-h] [--version] [-v] [-C DIR] {arbiter,tui,noop} ...
 
 A framework for implementing Python services.
 
 optional arguments:
-  -h, --help         show this help message and exit
-  --version          show program's version number and exit
-  -v, --verbose      set to increase logging verbosity
-  -C DIR, --dir DIR  execute from a specific directory
+  -h, --help          show this help message and exit
+  --version           show program's version number and exit
+  -v, --verbose       set to increase logging verbosity
+  -C DIR, --dir DIR   execute from a specific directory
 
 commands:
-  {tui,noop}         set of available commands
-    tui              run a terminal interface for the channel environment
-    noop             command stub (does nothing)
+  {arbiter,tui,noop}  set of available commands
+    arbiter           run a connection-arbiter application from a config
+    tui               run a terminal interface for the channel environment
+    noop              command stub (does nothing)
+
+```
+
+## Sub-command Options
+
+### `arbiter`
+
+```
+$ ./venv3.8/bin/runtimepy arbiter -h
+
+usage: runtimepy arbiter [-h] config
+
+positional arguments:
+  config      the configuration to load
+
+optional arguments:
+  -h, --help  show this help message and exit
+
+```
+
+### `tui`
+
+```
+$ ./venv3.8/bin/runtimepy tui -h
+
+usage: runtimepy tui [-h] [-i ITERATIONS] [-r RATE]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i ITERATIONS, --iterations ITERATIONS
+                        maximum number of program iterations (if greater than
+                        zero, default: 0)
+  -r RATE, --rate RATE  frequency (in Hz) to run the interface (default: 60.0
+                        Hz)
 
 ```
 
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `runtimepy`'s source.
```

### Comparing `runtimepy-1.1.1/pyproject.toml` & `runtimepy-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "1.1.1"
+version = "1.2.0"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-1.1.1/runtimepy/app.py` & `runtimepy-1.2.0/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/channel/__init__.py` & `runtimepy-1.2.0/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/channel/environment/__init__.py` & `runtimepy-1.2.0/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/channel/environment/array.py` & `runtimepy-1.2.0/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/channel/environment/base.py` & `runtimepy-1.2.0/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/channel/environment/create.py` & `runtimepy-1.2.0/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/channel/environment/file.py` & `runtimepy-1.2.0/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/channel/environment/names.py` & `runtimepy-1.2.0/runtimepy/channel/environment/names.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/channel/registry.py` & `runtimepy-1.2.0/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/codec/protocol/base.py` & `runtimepy-1.2.0/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/codec/protocol/json.py` & `runtimepy-1.2.0/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/commands/tui.py` & `runtimepy-1.2.0/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-1.2.0/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/entry.py` & `runtimepy-1.2.0/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/enum/__init__.py` & `runtimepy-1.2.0/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/enum/registry.py` & `runtimepy-1.2.0/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/enum/type.py` & `runtimepy-1.2.0/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/mapping.py` & `runtimepy-1.2.0/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/mixins/enum.py` & `runtimepy-1.2.0/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/mixins/regex.py` & `runtimepy-1.2.0/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/__init__.py` & `runtimepy-1.2.0/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/arbiter/base.py` & `runtimepy-1.2.0/runtimepy/net/arbiter/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     def __init__(
         self,
         manager: _ConnectionManager = None,
         stop_sig: _asyncio.Event = None,
         namespace: _Namespace = None,
         logger: _LoggerType = None,
+        app: NetworkApplication = init_only,
     ) -> None:
         """Initialize this connection arbiter."""
 
         _LoggerMixin.__init__(self, logger=logger)
 
         if manager is None:
             manager = _ConnectionManager()
@@ -61,14 +62,18 @@
 
         if stop_sig is None:
             stop_sig = _asyncio.Event()
         self.stop_sig = stop_sig
 
         _NamespaceMixin.__init__(self, namespace=namespace)
 
+        # A fallback application. Set a class attribute so this can be more
+        # easily externally updated.
+        self._app = app
+
         # Keep track of connection objects.
         self._connections: ConnectionMap = {}
         self._deferred_connections: _MutableMapping[
             str, _Awaitable[_Connection]
         ] = {}
 
         self._servers: _List[ServerTask] = []
@@ -110,15 +115,15 @@
                 self._register_connection(connection, name)
 
             result = True
 
         return result
 
     async def _entry(
-        self, app: NetworkApplication, check_connections: bool = True
+        self, app: NetworkApplication = None, check_connections: bool = True
     ) -> int:
         """
         Ensures connections are given a chance to initialize, run the
         application, clean up connections and return the application's result.
         """
 
         result = -1
@@ -145,27 +150,31 @@
             # Run application, but only if all the registered connections are
             # still alive after initialization.
             if not check_connections or not any(
                 x.disabled for x in self._connections.values()
             ):
                 async with _AsyncExitStack() as stack:
                     self.logger.info("Application starting.")
+
+                    if app is None:
+                        app = self._app
+
                     result = await app(stack, self._connections)
                     self.logger.info("Application returned %d.", result)
 
         finally:
             for conn in self._connections.values():
                 conn.disable(f"app exit {result}")
             self.stop_sig.set()
 
         return result
 
     async def app(
         self,
-        app: NetworkApplication = init_only,
+        app: NetworkApplication = None,
         check_connections: bool = True,
     ) -> int:
         """
         Run the application alongside the connection manager and server tasks.
         """
 
         result = await _asyncio.gather(
@@ -173,15 +182,15 @@
             self.manager.manage(self.stop_sig),
             *self._servers,
         )
         return int(result[0])
 
     def run(
         self,
-        app: NetworkApplication = init_only,
+        app: NetworkApplication = None,
         eloop: _asyncio.AbstractEventLoop = None,
         signals: _Iterable[int] = None,
         check_connections: bool = True,
     ) -> int:
         """Run the application until the stop signal is set."""
 
         return _run_handle_stop(
```

### Comparing `runtimepy-1.1.1/runtimepy/net/arbiter/factory.py` & `runtimepy-1.2.0/runtimepy/net/arbiter/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     def register_factory(
         self, factory: ConnectionFactory, *namespaces: str
     ) -> bool:
         """Attempt to register a connection factory."""
 
         result = False
 
+        assert isinstance(factory, ConnectionFactory), factory
+
         name = factory.__class__.__name__
         snake_name = obj_class_to_snake(factory)
 
         if name not in self._factories and snake_name not in self._factories:
             self._factories[name] = factory
             self._factories[snake_name] = factory
             self._names[factory] = [*namespaces]
```

### Comparing `runtimepy-1.1.1/runtimepy/net/arbiter/tcp.py` & `runtimepy-1.2.0/runtimepy/net/arbiter/tcp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/arbiter/udp.py` & `runtimepy-1.2.0/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/arbiter/websocket.py` & `runtimepy-1.2.0/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/connection.py` & `runtimepy-1.2.0/runtimepy/net/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self._text_messages: _asyncio.Queue[str] = _asyncio.Queue()
         self.tx_text_hwm: int = 0
         self._binary_messages: _asyncio.Queue[BinaryMessage] = _asyncio.Queue()
         self.tx_binary_hwm: int = 0
 
         self._tasks: _List[_asyncio.Task[None]] = []
         self.initialized = _asyncio.Event()
+        self.disabled_event = _asyncio.Event()
         self.init()
 
     def init(self) -> None:
         """Initialize this instance."""
 
     async def async_init(self) -> bool:
         """A runtime initialization routine (executes during 'process')."""
@@ -98,14 +99,17 @@
             self._enabled = False
 
             # Cancel tasks.
             for task in self._tasks:
                 if not task.done():
                     task.cancel()
 
+            # Signal that this connection has been disabled.
+            self.disabled_event.set()
+
     async def _wait_sig(self, stop_sig: _asyncio.Event) -> None:
         """Disable the connection if a stop signal gets set."""
         await stop_sig.wait()
         self.disable("stop signal")
 
     async def _async_init(self) -> None:
         """Run this connection's initialization routine."""
```

### Comparing `runtimepy-1.1.1/runtimepy/net/manager.py` & `runtimepy-1.2.0/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/mixin.py` & `runtimepy-1.2.0/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/tcp/connection.py` & `runtimepy-1.2.0/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-1.2.0/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-1.2.0/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/net/udp/connection.py` & `runtimepy-1.2.0/runtimepy/net/udp/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 # built-in
 from abc import abstractmethod as _abstractmethod
 import asyncio as _asyncio
 from asyncio import DatagramProtocol as _DatagramProtocol
 from asyncio import DatagramTransport as _DatagramTransport
-from logging import getLogger
+from logging import getLogger as _getLogger
 import socket as _socket
 from typing import Tuple as _Tuple
 from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 
 # third-party
@@ -21,14 +21,16 @@
 
 # internal
 from runtimepy.net import IpHost, get_free_socket
 from runtimepy.net.connection import BinaryMessage as _BinaryMessage
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.mixin import TransportMixin as _TransportMixin
 
+LOG = _getLogger(__name__)
+
 
 class UdpQueueProtocol(_DatagramProtocol):
     """A simple UDP protocol that populates a message queue."""
 
     logger: _LoggerType
 
     def __init__(self) -> None:
@@ -63,15 +65,15 @@
 
         _TransportMixin.__init__(self, transport)
 
         # Re-assign with updated type information.
         self._transport: _DatagramTransport = transport
 
         self._protocol = protocol
-        super().__init__(getLogger(self.logger_name("UDP ")))
+        super().__init__(_getLogger(self.logger_name("UDP ")))
         self._protocol.logger = self.logger
 
     @_abstractmethod
     async def process_datagram(
         self, data: bytes, addr: _Tuple[str, int]
     ) -> bool:
         """Process a datagram."""
@@ -92,14 +94,16 @@
 
     @classmethod
     async def create_connection(cls: _Type[T], **kwargs) -> T:
         """Create a UDP connection."""
 
         eloop = _asyncio.get_event_loop()
 
+        LOG.debug("kwargs: %s", {**kwargs})
+
         transport: _DatagramTransport
         (
             transport,
             protocol,
         ) = await eloop.create_datagram_endpoint(UdpQueueProtocol, **kwargs)
         return cls(transport, protocol)
```

### Comparing `runtimepy-1.1.1/runtimepy/net/websocket/connection.py` & `runtimepy-1.2.0/runtimepy/net/websocket/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,15 +106,35 @@
         """
 
         async def _handler(protocol: _WebSocketServerProtocol) -> None:
             """A handler that runs the callers initialization function."""
             conn = cls(protocol)
             if init is None or await init(conn):
                 if manager is not None:
+                    # Allow the connection manager to process this connection.
                     await manager.queue.put(conn)
+
+                    # Wait for either the connection to be disabled, or for
+                    # the stop signal to be set.
+                    tasks = [_asyncio.create_task(conn.disabled_event.wait())]
+                    if stop_sig is not None:
+                        tasks.append(_asyncio.create_task(stop_sig.wait()))
+
+                    # Wait for the event and cancel the task that didn't
+                    # complete.
+                    _, pending = await _asyncio.wait(
+                        tasks,
+                        return_when=_asyncio.FIRST_COMPLETED,
+                    )
+                    for task in pending:
+                        task.cancel()
+                        await task
+
+                # If there's no connection manager, just process the
+                # connection here.
                 else:
                     await conn.process(stop_sig=stop_sig)
 
         return _handler
 
     @classmethod
     @_asynccontextmanager
```

### Comparing `runtimepy-1.1.1/runtimepy/primitives/__init__.py` & `runtimepy-1.2.0/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/array.py` & `runtimepy-1.2.0/runtimepy/primitives/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/base.py` & `runtimepy-1.2.0/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/bool.py` & `runtimepy-1.2.0/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/byte_order.py` & `runtimepy-1.2.0/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/field/__init__.py` & `runtimepy-1.2.0/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/field/fields.py` & `runtimepy-1.2.0/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-1.2.0/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/field/manager/base.py` & `runtimepy-1.2.0/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/float.py` & `runtimepy-1.2.0/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/int.py` & `runtimepy-1.2.0/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/string.py` & `runtimepy-1.2.0/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/type/__init__.py` & `runtimepy-1.2.0/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/type/base.py` & `runtimepy-1.2.0/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/type/float.py` & `runtimepy-1.2.0/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/primitives/type/int.py` & `runtimepy-1.2.0/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/registry/__init__.py` & `runtimepy-1.2.0/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/registry/bool.py` & `runtimepy-1.2.0/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/registry/item.py` & `runtimepy-1.2.0/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/registry/name.py` & `runtimepy-1.2.0/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/schemas.py` & `runtimepy-1.2.0/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/task/__init__.py` & `runtimepy-1.2.0/runtimepy/task/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/task/basic/__init__.py` & `runtimepy-1.2.0/runtimepy/task/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/tui/channels/__init__.py` & `runtimepy-1.2.0/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy/tui/task.py` & `runtimepy-1.2.0/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/runtimepy.egg-info/PKG-INFO` & `runtimepy-1.2.0/runtimepy.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 1.1.1
+Version: 1.2.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=182b46b499d24cb62c9688e373b88345
+    hash=ce3f1316217e521947cc4b3047971525
     =====================================
 -->
 
-# runtimepy ([1.1.1](https://pypi.org/project/runtimepy/))
+# runtimepy ([1.2.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
@@ -64,28 +64,63 @@
 # Introduction
 
 # Command-line Options
 
 ```
 $ ./venv3.8/bin/runtimepy -h
 
-usage: runtimepy [-h] [--version] [-v] [-C DIR] {tui,noop} ...
+usage: runtimepy [-h] [--version] [-v] [-C DIR] {arbiter,tui,noop} ...
 
 A framework for implementing Python services.
 
 optional arguments:
-  -h, --help         show this help message and exit
-  --version          show program's version number and exit
-  -v, --verbose      set to increase logging verbosity
-  -C DIR, --dir DIR  execute from a specific directory
+  -h, --help          show this help message and exit
+  --version           show program's version number and exit
+  -v, --verbose       set to increase logging verbosity
+  -C DIR, --dir DIR   execute from a specific directory
 
 commands:
-  {tui,noop}         set of available commands
-    tui              run a terminal interface for the channel environment
-    noop             command stub (does nothing)
+  {arbiter,tui,noop}  set of available commands
+    arbiter           run a connection-arbiter application from a config
+    tui               run a terminal interface for the channel environment
+    noop              command stub (does nothing)
+
+```
+
+## Sub-command Options
+
+### `arbiter`
+
+```
+$ ./venv3.8/bin/runtimepy arbiter -h
+
+usage: runtimepy arbiter [-h] config
+
+positional arguments:
+  config      the configuration to load
+
+optional arguments:
+  -h, --help  show this help message and exit
+
+```
+
+### `tui`
+
+```
+$ ./venv3.8/bin/runtimepy tui -h
+
+usage: runtimepy tui [-h] [-i ITERATIONS] [-r RATE]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i ITERATIONS, --iterations ITERATIONS
+                        maximum number of program iterations (if greater than
+                        zero, default: 0)
+  -r RATE, --rate RATE  frequency (in Hz) to run the interface (default: 60.0
+                        Hz)
 
 ```
 
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `runtimepy`'s source.
```

### Comparing `runtimepy-1.1.1/runtimepy.egg-info/SOURCES.txt` & `runtimepy-1.2.0/runtimepy.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -28,33 +28,39 @@
 runtimepy/channel/environment/names.py
 runtimepy/codec/__init__.py
 runtimepy/codec/protocol/__init__.py
 runtimepy/codec/protocol/base.py
 runtimepy/codec/protocol/json.py
 runtimepy/commands/__init__.py
 runtimepy/commands/all.py
+runtimepy/commands/arbiter.py
 runtimepy/commands/tui.py
 runtimepy/data/schemas/BitFields.yaml
 runtimepy/data/schemas/Channel.yaml
 runtimepy/data/schemas/ChannelRegistry.yaml
+runtimepy/data/schemas/ClientConnectionConfig.yaml
+runtimepy/data/schemas/ConnectionArbiterConfig.yaml
 runtimepy/data/schemas/EnumRegistry.yaml
 runtimepy/data/schemas/RuntimeEnum.yaml
+runtimepy/data/schemas/ServerConnectionConfig.yaml
 runtimepy/enum/__init__.py
 runtimepy/enum/registry.py
 runtimepy/enum/type.py
 runtimepy/mixins/__init__.py
 runtimepy/mixins/enum.py
 runtimepy/mixins/regex.py
 runtimepy/net/__init__.py
 runtimepy/net/connection.py
 runtimepy/net/manager.py
 runtimepy/net/mixin.py
 runtimepy/net/arbiter/__init__.py
 runtimepy/net/arbiter/base.py
+runtimepy/net/arbiter/config.py
 runtimepy/net/arbiter/factory.py
+runtimepy/net/arbiter/imports.py
 runtimepy/net/arbiter/tcp.py
 runtimepy/net/arbiter/udp.py
 runtimepy/net/arbiter/websocket.py
 runtimepy/net/tcp/__init__.py
 runtimepy/net/tcp/connection.py
 runtimepy/net/tcp/telnet/__init__.py
 runtimepy/net/tcp/telnet/codes.py
```

### Comparing `runtimepy-1.1.1/setup.py` & `runtimepy-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/tests/test_entry.py` & `runtimepy-1.2.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-1.1.1/tests/test_mapping.py` & `runtimepy-1.2.0/tests/test_mapping.py`

 * *Files identical despite different names*

