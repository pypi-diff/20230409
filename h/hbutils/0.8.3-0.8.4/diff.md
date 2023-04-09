# Comparing `tmp/hbutils-0.8.3.tar.gz` & `tmp/hbutils-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbutils-0.8.3.tar", last modified: Sat Apr  8 02:23:43 2023, max compression
+gzip compressed data, was "hbutils-0.8.4.tar", last modified: Sun Apr  9 03:35:48 2023, max compression
```

## Comparing `hbutils-0.8.3.tar` & `hbutils-0.8.4.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.673721 hbutils-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 02:21:33.000000 hbutils-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-08 02:23:43.673721 hbutils-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-08 02:21:33.000000 hbutils-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.641721 hbutils-0.8.3/hbutils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.641721 hbutils-0.8.3/hbutils/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/algorithm/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/algorithm/topological.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.645721 hbutils-0.8.3/hbutils/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/binary/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/binary/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/binary/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/binary/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/binary/str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/binary/uint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.645721 hbutils-0.8.3/hbutils/collection/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/collection/dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/collection/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/collection/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/collection/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/collection/stacked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/collection/structural.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.649721 hbutils-0.8.3/hbutils/color/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/color/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22809 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/color/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/color/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.649721 hbutils-0.8.3/hbutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.649721 hbutils-0.8.3/hbutils/design/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/design/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/design/final.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/design/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/design/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.649721 hbutils-0.8.3/hbutils/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/encoding/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/encoding/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/encoding/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/encoding/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.653721 hbutils-0.8.3/hbutils/expression/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/expression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.653721 hbutils-0.8.3/hbutils/expression/native/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/expression/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/expression/native/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/expression/native/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/expression/native/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.653721 hbutils-0.8.3/hbutils/file/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/file/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.653721 hbutils-0.8.3/hbutils/model/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/model/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/model/clazz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/model/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/model/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/model/repr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.657721 hbutils-0.8.3/hbutils/random/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/random/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/random/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/random/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/random/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.657721 hbutils-0.8.3/hbutils/reflection/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/reflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/reflection/clazz.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/reflection/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/reflection/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/reflection/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/reflection/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/reflection/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/reflection/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.661721 hbutils-0.8.3/hbutils/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/scale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/scale/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/scale/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.661721 hbutils-0.8.3/hbutils/string/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/string/inflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/string/plural.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/string/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/string/trunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.661721 hbutils-0.8.3/hbutils/system/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.661721 hbutils-0.8.3/hbutils/system/filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/filesystem/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/filesystem/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/filesystem/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.661721 hbutils-0.8.3/hbutils/system/network/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/network/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/network/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/network/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.665721 hbutils-0.8.3/hbutils/system/os/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/os/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/os/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.665721 hbutils-0.8.3/hbutils/system/python/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/python/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/python/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/system/python/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.665721 hbutils-0.8.3/hbutils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.665721 hbutils-0.8.3/hbutils/testing/capture/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/capture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/capture/exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/capture/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.665721 hbutils-0.8.3/hbutils/testing/compare/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/compare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/compare/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.669721 hbutils-0.8.3/hbutils/testing/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/generator/aetg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/generator/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/generator/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.669721 hbutils-0.8.3/hbutils/testing/isolated/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/isolated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/isolated/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/isolated/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/isolated/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/isolated/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.669721 hbutils-0.8.3/hbutils/testing/requires/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/requires/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/requires/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/requires/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.673721 hbutils-0.8.3/hbutils/testing/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-08 02:21:33.000000 hbutils-0.8.3/hbutils/testing/simulate/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 02:23:43.641721 hbutils-0.8.3/hbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-08 02:23:43.000000 hbutils-0.8.3/hbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-08 02:23:43.000000 hbutils-0.8.3/hbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 02:23:43.000000 hbutils-0.8.3/hbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-08 02:23:43.000000 hbutils-0.8.3/hbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 02:23:43.000000 hbutils-0.8.3/hbutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 02:23:43.673721 hbutils-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-08 02:21:33.000000 hbutils-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.779200 hbutils-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 03:33:37.000000 hbutils-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-09 03:35:48.779200 hbutils-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-09 03:33:37.000000 hbutils-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.731200 hbutils-0.8.4/hbutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.735200 hbutils-0.8.4/hbutils/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/algorithm/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/algorithm/topological.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.739200 hbutils-0.8.4/hbutils/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/binary/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/binary/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/binary/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/binary/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/binary/str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/binary/uint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.743200 hbutils-0.8.4/hbutils/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/collection/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/collection/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/collection/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/collection/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/collection/stacked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/collection/structural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.743200 hbutils-0.8.4/hbutils/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/color/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22809 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/color/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/color/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.743200 hbutils-0.8.4/hbutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.743200 hbutils-0.8.4/hbutils/design/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/design/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/design/final.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/design/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/design/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.747200 hbutils-0.8.4/hbutils/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/encoding/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/encoding/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/encoding/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/encoding/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.747200 hbutils-0.8.4/hbutils/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/expression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.747200 hbutils-0.8.4/hbutils/expression/native/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/expression/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/expression/native/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/expression/native/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/expression/native/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.747200 hbutils-0.8.4/hbutils/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/file/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.751200 hbutils-0.8.4/hbutils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/model/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/model/clazz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/model/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/model/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/model/repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.755200 hbutils-0.8.4/hbutils/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/random/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/random/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/random/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/random/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.759200 hbutils-0.8.4/hbutils/reflection/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/reflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/reflection/clazz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/reflection/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/reflection/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/reflection/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/reflection/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/reflection/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/reflection/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.763200 hbutils-0.8.4/hbutils/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/scale/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/scale/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.763200 hbutils-0.8.4/hbutils/string/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/string/inflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/string/plural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/string/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/string/trunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.763200 hbutils-0.8.4/hbutils/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.767200 hbutils-0.8.4/hbutils/system/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/filesystem/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/filesystem/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/filesystem/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.767200 hbutils-0.8.4/hbutils/system/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/network/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/network/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/network/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.767200 hbutils-0.8.4/hbutils/system/os/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/os/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/os/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.771200 hbutils-0.8.4/hbutils/system/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/python/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/python/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/system/python/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.771200 hbutils-0.8.4/hbutils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.771200 hbutils-0.8.4/hbutils/testing/capture/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/capture/exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/capture/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.775200 hbutils-0.8.4/hbutils/testing/compare/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/compare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/compare/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.775200 hbutils-0.8.4/hbutils/testing/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/generator/aetg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/generator/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/generator/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.779200 hbutils-0.8.4/hbutils/testing/isolated/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/isolated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/isolated/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/isolated/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/isolated/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/isolated/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.779200 hbutils-0.8.4/hbutils/testing/requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/requires/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/requires/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/requires/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.779200 hbutils-0.8.4/hbutils/testing/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-09 03:33:37.000000 hbutils-0.8.4/hbutils/testing/simulate/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:35:48.731200 hbutils-0.8.4/hbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-09 03:35:48.000000 hbutils-0.8.4/hbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-09 03:35:48.000000 hbutils-0.8.4/hbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 03:35:48.000000 hbutils-0.8.4/hbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-09 03:35:48.000000 hbutils-0.8.4/hbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 03:35:48.000000 hbutils-0.8.4/hbutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 03:35:48.779200 hbutils-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-09 03:33:37.000000 hbutils-0.8.4/setup.py
```

### Comparing `hbutils-0.8.3/LICENSE` & `hbutils-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/PKG-INFO` & `hbutils-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbutils
-Version: 0.8.3
+Version: 0.8.4
 Summary: Some useful functions and classes in Python infrastructure development.
 Home-page: https://github.com/hansbug/hbutils
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: Tree-structured Value Management
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hbutils-0.8.3/README.md` & `hbutils-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/algorithm/linear.py` & `hbutils-0.8.4/hbutils/algorithm/linear.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/algorithm/topological.py` & `hbutils-0.8.4/hbutils/algorithm/topological.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/binary/base.py` & `hbutils-0.8.4/hbutils/binary/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/binary/bool.py` & `hbutils-0.8.4/hbutils/binary/bool.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/binary/buffer.py` & `hbutils-0.8.4/hbutils/binary/buffer.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/binary/float.py` & `hbutils-0.8.4/hbutils/binary/float.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/binary/int.py` & `hbutils-0.8.4/hbutils/binary/int.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/binary/str.py` & `hbutils-0.8.4/hbutils/binary/str.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/binary/uint.py` & `hbutils-0.8.4/hbutils/binary/uint.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/collection/dimension.py` & `hbutils-0.8.4/hbutils/collection/dimension.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/collection/functional.py` & `hbutils-0.8.4/hbutils/collection/functional.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/collection/recover.py` & `hbutils-0.8.4/hbutils/collection/recover.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/collection/sequence.py` & `hbutils-0.8.4/hbutils/collection/sequence.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/collection/stacked.py` & `hbutils-0.8.4/hbutils/collection/stacked.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/collection/structural.py` & `hbutils-0.8.4/hbutils/collection/structural.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/color/base.py` & `hbutils-0.8.4/hbutils/color/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/color/model.py` & `hbutils-0.8.4/hbutils/color/model.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/color/utils.py` & `hbutils-0.8.4/hbutils/color/utils.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/design/decorator.py` & `hbutils-0.8.4/hbutils/design/decorator.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/design/final.py` & `hbutils-0.8.4/hbutils/design/final.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/design/observer.py` & `hbutils-0.8.4/hbutils/design/observer.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/design/singleton.py` & `hbutils-0.8.4/hbutils/design/singleton.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/encoding/ansi.py` & `hbutils-0.8.4/hbutils/encoding/ansi.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/encoding/base64.py` & `hbutils-0.8.4/hbutils/encoding/base64.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/encoding/decode.py` & `hbutils-0.8.4/hbutils/encoding/decode.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/encoding/hash.py` & `hbutils-0.8.4/hbutils/encoding/hash.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/expression/native/base.py` & `hbutils-0.8.4/hbutils/expression/native/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/expression/native/feature.py` & `hbutils-0.8.4/hbutils/expression/native/feature.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/expression/native/general.py` & `hbutils-0.8.4/hbutils/expression/native/general.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/file/stream.py` & `hbutils-0.8.4/hbutils/file/stream.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/model/clazz.py` & `hbutils-0.8.4/hbutils/model/clazz.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/model/compare.py` & `hbutils-0.8.4/hbutils/model/compare.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/model/enum.py` & `hbutils-0.8.4/hbutils/model/enum.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/model/raw.py` & `hbutils-0.8.4/hbutils/model/raw.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/model/repr.py` & `hbutils-0.8.4/hbutils/model/repr.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/random/binary.py` & `hbutils-0.8.4/hbutils/random/binary.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/random/sequence.py` & `hbutils-0.8.4/hbutils/random/sequence.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/random/state.py` & `hbutils-0.8.4/hbutils/random/state.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/random/string.py` & `hbutils-0.8.4/hbutils/random/string.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/reflection/clazz.py` & `hbutils-0.8.4/hbutils/reflection/clazz.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/reflection/context.py` & `hbutils-0.8.4/hbutils/reflection/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 """
 import collections.abc
 
 from contextlib import contextmanager
 from functools import wraps
 from multiprocessing import current_process
 from threading import current_thread
-from typing import Tuple, TypeVar, Iterator, Mapping, Optional
+from typing import Tuple, TypeVar, Iterator, Mapping, Optional, ContextManager, Any
 
 __all__ = [
     'context', 'cwrap',
+    'nested_with',
 ]
 
 
 def _get_pid() -> int:
     return current_process().pid
 
 
@@ -256,7 +257,83 @@
     @wraps(func)
     def _new_func(*args, **kwargs):
         with context().inherit(context_):
             with context().vars(**vars_):
                 return func(*args, **kwargs)
 
     return _new_func
+
+
+def _yield_nested_for(contexts, depth, items):
+    if depth >= len(contexts):
+        yield tuple(items)
+    else:
+        with contexts[depth] as current_item:
+            items.append(current_item)
+            yield from _yield_nested_for(contexts, depth + 1, items)
+
+
+@contextmanager
+def nested_with(*contexts) -> ContextManager[Tuple[Any, ...]]:
+    """
+    Overview:
+        Nested with, enter and exit multiple contexts.
+
+    :param contexts: Contexts to manage.
+
+    Examples::
+        >>> import os.path
+        >>> import pathlib
+        >>> import tempfile
+        >>> from contextlib import contextmanager
+        >>> from hbutils.reflection import nested_with
+        >>>
+        >>> # allocate a temporary directory, and put one file inside
+        >>> @contextmanager
+        ... def opent(x):
+        ...     with tempfile.TemporaryDirectory() as td:
+        ...         pathlib.Path(os.path.join(td, f'{x}.txt')).write_text(f'this is {x}!')
+        ...         yield td
+        >>>
+        >>> # let's try it
+        >>> with opent(1) as d:
+        ...     print(os.listdir(d))
+        ...     print(pathlib.Path(f'{d}/1.txt').read_text())
+        ['1.txt']
+        this is 1!
+        >>> # open 5 temporary directories at one time
+        >>> with nested_with(*map(opent, range(5))) as ds:
+        ...     for d in ds:
+        ...         print(d)
+        ...         print(os.path.exists(d), os.listdir(d))
+        ...         print(pathlib.Path(f'{d}/{os.listdir(d)[0]}').read_text())
+        /tmp/tmp3u1984br
+        True ['0.txt']
+        this is 0!
+        /tmp/tmp0yx56hv0
+        True ['1.txt']
+        this is 1!
+        /tmp/tmpu_33drm3
+        True ['2.txt']
+        this is 2!
+        /tmp/tmpqal_vzgi
+        True ['3.txt']
+        this is 3!
+        /tmp/tmpy99_wwtt
+        True ['4.txt']
+        this is 4!
+        >>> # these directories are released now
+        >>> for d in ds:
+        ...     print(d)
+        ...     print(os.path.exists(d))  # not exist anymore
+        /tmp/tmp3u1984br
+        False
+        /tmp/tmp0yx56hv0
+        False
+        /tmp/tmpu_33drm3
+        False
+        /tmp/tmpqal_vzgi
+        False
+        /tmp/tmpy99_wwtt
+        False
+    """
+    yield from _yield_nested_for(contexts, 0, [])
```

### Comparing `hbutils-0.8.3/hbutils/reflection/exception.py` & `hbutils-0.8.4/hbutils/reflection/exception.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/reflection/func.py` & `hbutils-0.8.4/hbutils/reflection/func.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/reflection/imports.py` & `hbutils-0.8.4/hbutils/reflection/imports.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/reflection/iter.py` & `hbutils-0.8.4/hbutils/reflection/iter.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/reflection/module.py` & `hbutils-0.8.4/hbutils/reflection/module.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/scale/size.py` & `hbutils-0.8.4/hbutils/scale/size.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/scale/time.py` & `hbutils-0.8.4/hbutils/scale/time.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/string/inflection.py` & `hbutils-0.8.4/hbutils/string/inflection.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/string/plural.py` & `hbutils-0.8.4/hbutils/string/plural.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/string/template.py` & `hbutils-0.8.4/hbutils/string/template.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/string/trunc.py` & `hbutils-0.8.4/hbutils/string/trunc.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/filesystem/binary.py` & `hbutils-0.8.4/hbutils/system/filesystem/binary.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/filesystem/directory.py` & `hbutils-0.8.4/hbutils/system/filesystem/directory.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/filesystem/file.py` & `hbutils-0.8.4/hbutils/system/filesystem/file.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/network/hosts.py` & `hbutils-0.8.4/hbutils/system/network/hosts.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/network/port.py` & `hbutils-0.8.4/hbutils/system/network/port.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/network/url.py` & `hbutils-0.8.4/hbutils/system/network/url.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/os/executable.py` & `hbutils-0.8.4/hbutils/system/os/executable.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/os/type.py` & `hbutils-0.8.4/hbutils/system/os/type.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/python/implementation.py` & `hbutils-0.8.4/hbutils/system/python/implementation.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/system/python/package.py` & `hbutils-0.8.4/hbutils/system/python/package.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/_base.py` & `hbutils-0.8.4/hbutils/testing/_base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/capture/exit.py` & `hbutils-0.8.4/hbutils/testing/capture/exit.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/capture/output.py` & `hbutils-0.8.4/hbutils/testing/capture/output.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/compare/text.py` & `hbutils-0.8.4/hbutils/testing/compare/text.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/generator/aetg.py` & `hbutils-0.8.4/hbutils/testing/generator/aetg.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/generator/base.py` & `hbutils-0.8.4/hbutils/testing/generator/base.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/generator/func.py` & `hbutils-0.8.4/hbutils/testing/generator/func.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/generator/matrix.py` & `hbutils-0.8.4/hbutils/testing/generator/matrix.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/isolated/directory.py` & `hbutils-0.8.4/hbutils/testing/isolated/directory.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/isolated/entry_point.py` & `hbutils-0.8.4/hbutils/testing/isolated/entry_point.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/isolated/input.py` & `hbutils-0.8.4/hbutils/testing/isolated/input.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/isolated/logging.py` & `hbutils-0.8.4/hbutils/testing/isolated/logging.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/requires/cmd.py` & `hbutils-0.8.4/hbutils/testing/requires/cmd.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/requires/expr.py` & `hbutils-0.8.4/hbutils/testing/requires/expr.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/requires/version.py` & `hbutils-0.8.4/hbutils/testing/requires/version.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils/testing/simulate/entry.py` & `hbutils-0.8.4/hbutils/testing/simulate/entry.py`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils.egg-info/PKG-INFO` & `hbutils-0.8.4/hbutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbutils
-Version: 0.8.3
+Version: 0.8.4
 Summary: Some useful functions and classes in Python infrastructure development.
 Home-page: https://github.com/hansbug/hbutils
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: Tree-structured Value Management
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hbutils-0.8.3/hbutils.egg-info/SOURCES.txt` & `hbutils-0.8.4/hbutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/hbutils.egg-info/requires.txt` & `hbutils-0.8.4/hbutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hbutils-0.8.3/setup.py` & `hbutils-0.8.4/setup.py`

 * *Files identical despite different names*

