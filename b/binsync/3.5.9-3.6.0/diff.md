# Comparing `tmp/binsync-3.5.9.tar.gz` & `tmp/binsync-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binsync-3.5.9.tar", last modified: Mon Mar 27 22:13:07 2023, max compression
+gzip compressed data, was "binsync-3.6.0.tar", last modified: Sat Apr  8 23:09:33 2023, max compression
```

## Comparing `binsync-3.5.9.tar` & `binsync-3.6.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.957314 binsync-3.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-27 22:12:56.000000 binsync-3.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-27 22:12:56.000000 binsync-3.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-03-27 22:13:07.957314 binsync-3.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-03-27 22:12:56.000000 binsync-3.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.945314 binsync-3.5.9/binsync/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.945314 binsync-3.5.9/binsync/common/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)    37358 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.949314 binsync-3.5.9/binsync/common/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/control_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.949314 binsync-3.5.9/binsync/common/ui/force_push/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/force_push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/force_push/force_push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.949314 binsync-3.5.9/binsync/common/ui/force_push/panels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/force_push/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/force_push/panels/functions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/force_push/panels/global_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/magic_sync_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.949314 binsync-3.5.9/binsync/common/ui/panel_tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/panel_tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/panel_tabs/activity_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/panel_tabs/ctx_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/panel_tabs/functions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/panel_tabs/globals_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/panel_tabs/table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/panel_tabs/util_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/common/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.949314 binsync-3.5.9/binsync/core/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/core/cache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24708 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/core/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/core/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.949314 binsync-3.5.9/binsync/data/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/stack_variable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20455 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/data/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/binsync/decompilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/binsync/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/angr/control_panel_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/angr/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/angr/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/binsync/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/binja/binja_binsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/binja/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/binja/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/binsync/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ghidra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/binsync/decompilers/ghidra/server/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ghidra/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ghidra/server/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ghidra/server/control_panel_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ghidra/server/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ghidra/server/ghidra_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/binsync/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22352 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ida/compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10336 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ida/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ida/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ida/oneliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/decompilers/ida/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-27 22:12:56.000000 binsync-3.5.9/binsync/loggercfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.945314 binsync-3.5.9/binsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-03-27 22:13:07.000000 binsync-3.5.9/binsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-27 22:13:07.000000 binsync-3.5.9/binsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 22:13:07.000000 binsync-3.5.9/binsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 22:13:07.000000 binsync-3.5.9/binsync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-27 22:13:07.000000 binsync-3.5.9/binsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 22:13:07.000000 binsync-3.5.9/binsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/decompiler_stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/decompiler_stubs/angr_binsync/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-27 22:12:56.000000 binsync-3.5.9/decompiler_stubs/angr_binsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-27 22:12:56.000000 binsync-3.5.9/decompiler_stubs/angr_binsync/plugin.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.953314 binsync-3.5.9/decompiler_stubs/binja_binsync/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-27 22:12:56.000000 binsync-3.5.9/decompiler_stubs/binja_binsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-27 22:12:56.000000 binsync-3.5.9/decompiler_stubs/binja_binsync/plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-27 22:12:56.000000 binsync-3.5.9/decompiler_stubs/ghidra_binsync.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-27 22:12:56.000000 binsync-3.5.9/decompiler_stubs/ida_binsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-27 22:13:07.957314 binsync-3.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-27 22:12:56.000000 binsync-3.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:13:07.957314 binsync-3.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-03-27 22:12:56.000000 binsync-3.5.9/tests/test_angr_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-27 22:12:56.000000 binsync-3.5.9/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-03-27 22:12:56.000000 binsync-3.5.9/tests/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-08 23:09:21.000000 binsync-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-08 23:09:21.000000 binsync-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-04-08 23:09:33.022079 binsync-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-04-08 23:09:21.000000 binsync-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.006079 binsync-3.6.0/binsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.006079 binsync-3.6.0/binsync/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37358 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.010079 binsync-3.6.0/binsync/common/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/control_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.010079 binsync-3.6.0/binsync/common/ui/force_push/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/force_push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.010079 binsync-3.6.0/binsync/common/ui/force_push/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/panels/functions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/panels/global_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/magic_sync_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.010079 binsync-3.6.0/binsync/common/ui/panel_tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/activity_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/ctx_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/functions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/globals_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/util_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.014079 binsync-3.6.0/binsync/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24708 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.014079 binsync-3.6.0/binsync/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/stack_variable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20455 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.014079 binsync-3.6.0/binsync/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.018079 binsync-3.6.0/binsync/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/control_panel_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.018079 binsync-3.6.0/binsync/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/binja_binsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.018079 binsync-3.6.0/binsync/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.018079 binsync-3.6.0/binsync/decompilers/ghidra/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/control_panel_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/ghidra_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/binsync/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22352 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10336 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/oneliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/loggercfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.006079 binsync-3.6.0/binsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/decompiler_stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/decompiler_stubs/angr_binsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/angr_binsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/angr_binsync/plugin.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/decompiler_stubs/binja_binsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/binja_binsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/binja_binsync/plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/ghidra_binsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/ida_binsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-08 23:09:33.022079 binsync-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-08 23:09:21.000000 binsync-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-08 23:09:21.000000 binsync-3.6.0/tests/test_angr_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-08 23:09:21.000000 binsync-3.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-08 23:09:21.000000 binsync-3.6.0/tests/test_state.py
```

### Comparing `binsync-3.5.9/LICENSE` & `binsync-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/__main__.py` & `binsync-3.6.0/binsync/__main__.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/artifact_lifter.py` & `binsync-3.6.0/binsync/common/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/controller.py` & `binsync-3.6.0/binsync/common/controller.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/config_dialog.py` & `binsync-3.6.0/binsync/common/ui/config_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,16 @@
         super()._on_ok_clicked()
 
 
 class ConfigureBSDialog(QDialog):
     def __init__(self, controller, open_magic_sync=True, load_config=True, parent=None):
         super().__init__(parent)
         self.controller = controller
+        self.open_magic_sync = open_magic_sync
+        self.load_config = load_config
 
         self.setWindowTitle("Start BinSync")
         self._main_layout = QVBoxLayout()
 
         self._init_widgets()
         self.setLayout(self._main_layout)
         self.show()
```

### Comparing `binsync-3.5.9/binsync/common/ui/control_panel.py` & `binsync-3.6.0/binsync/common/ui/control_panel.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/force_push/force_push.py` & `binsync-3.6.0/binsync/common/ui/force_push/force_push.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/force_push/panels/functions_table.py` & `binsync-3.6.0/binsync/common/ui/force_push/panels/functions_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,19 +281,28 @@
             mappedIndex = self.proxymodel.mapToSource(proxyIndex)
             if not self.model.data(mappedIndex, Qt.CheckStateRole):
                 break
         else:
             self.select_all.setChecked(True)
 
     def push(self):
+        # In higher QT versions, like those used in Binja, the way states are described in
+        # a checkbox changed, so we must find out if .value can be used or not
+        first_state_obj = self.model.checkState(
+            self.proxymodel.mapToSource(self.proxymodel.index(0, 0, QModelIndex()))
+        )
+        check_has_value = hasattr(first_state_obj, "value")
+
         self.proxymodel.setFilterFixedString("")
         for i in range(self.proxymodel.rowCount()):
             proxyIndex = self.proxymodel.index(i, 0, QModelIndex())
             mappedIndex = self.proxymodel.mapToSource(proxyIndex)
-            if self.model.checkState(mappedIndex):
+            model_state = self.model.checkState(mappedIndex)
+            is_checked = model_state.value if check_has_value else model_state
+            if is_checked:
                 func_addr = int(self.model.data(mappedIndex), 16)
                 self.controller.force_push_function(func_addr)
 
     def connect_select_all(self, checkbox):
         self.select_all = checkbox
 
     def check_all(self):
```

### Comparing `binsync-3.5.9/binsync/common/ui/force_push/panels/global_panel.py` & `binsync-3.6.0/binsync/common/ui/force_push/panels/global_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -267,19 +267,28 @@
         self.proxymodel.setFilterFixedString(text)
         self.select_all.setChecked(False)
 
     def _lookup_addr_for_gvar(self, name):
         return self.model.gvar_name_to_addr_map[name]
 
     def push(self):
+        # In higher QT versions, like those used in Binja, the way states are described in
+        # a checkbox changed, so we must find out if .value can be used or not
+        first_state_obj = self.model.checkState(
+            self.proxymodel.mapToSource(self.proxymodel.index(0, 0, QModelIndex()))
+        )
+        check_has_value = hasattr(first_state_obj, "value")
+
         self.proxymodel.setFilterFixedString("")
         for i in range(self.proxymodel.rowCount()):
             proxyIndex = self.proxymodel.index(i, 0, QModelIndex())
             mappedIndex = self.proxymodel.mapToSource(proxyIndex)
-            if self.model.checkState(mappedIndex):
+            model_state = self.model.checkState(mappedIndex)
+            is_checked = model_state.value if check_has_value else model_state
+            if is_checked:
                 type_ = self.model.data(mappedIndex)
                 name = self.model.data(mappedIndex.sibling(mappedIndex.row(), 1))
                 lookup_item = self._lookup_addr_for_gvar(name) if type_ == "Variable" else name
                 print(f"\npushing {lookup_item}\n")
                 self.controller.force_push_global_artifact(lookup_item)
 
     def connect_select_all(self, checkbox):
```

### Comparing `binsync-3.5.9/binsync/common/ui/magic_sync_dialog.py` & `binsync-3.6.0/binsync/common/ui/magic_sync_dialog.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/panel_tabs/activity_table.py` & `binsync-3.6.0/binsync/common/ui/panel_tabs/activity_table.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/panel_tabs/ctx_table.py` & `binsync-3.6.0/binsync/common/ui/panel_tabs/ctx_table.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/panel_tabs/functions_table.py` & `binsync-3.6.0/binsync/common/ui/panel_tabs/functions_table.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/panel_tabs/globals_table.py` & `binsync-3.6.0/binsync/common/ui/panel_tabs/globals_table.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/panel_tabs/table_model.py` & `binsync-3.6.0/binsync/common/ui/panel_tabs/table_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         self.update_signal.emit(list(row_data.values()), row_colors)
 
         # ask for in-row updates (in UI) to any single row changed
         for update_idx in row_update_idxs:
             self.dataChanged.emit(self.index(0, update_idx), self.index(self.rowCount() - 1, update_idx))
 
     def _compute_row_color(self, artifact_update_time: datetime.datetime):
-        duration = (datetime.datetime.now(tz=datetime.timezone.utc) - artifact_update_time).seconds  # table coloring
+        duration = int(datetime.datetime.now(tz=datetime.timezone.utc).timestamp() - artifact_update_time.timestamp())
         if 0 <= duration <= self.controller.table_coloring_window:
             opacity = (self.controller.table_coloring_window - duration) / self.controller.table_coloring_window
             return QColor(
                 BinsyncTableModel.ACTIVE_FUNCTION_COLOR[0],
                 BinsyncTableModel.ACTIVE_FUNCTION_COLOR[1],
                 BinsyncTableModel.ACTIVE_FUNCTION_COLOR[2],
                 int(BinsyncTableModel.ACTIVE_FUNCTION_COLOR[3] * opacity)
```

### Comparing `binsync-3.5.9/binsync/common/ui/panel_tabs/util_panel.py` & `binsync-3.6.0/binsync/common/ui/panel_tabs/util_panel.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/qt_objects.py` & `binsync-3.6.0/binsync/common/ui/qt_objects.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/common/ui/utils.py` & `binsync-3.6.0/binsync/common/ui/utils.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/core/cache.py` & `binsync-3.6.0/binsync/core/cache.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/core/client.py` & `binsync-3.6.0/binsync/core/client.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/core/scheduler.py` & `binsync-3.6.0/binsync/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/__init__.py` & `binsync-3.6.0/binsync/data/__init__.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/artifact.py` & `binsync-3.6.0/binsync/data/artifact.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/comment.py` & `binsync-3.6.0/binsync/data/comment.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/configuration.py` & `binsync-3.6.0/binsync/data/configuration.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/enum.py` & `binsync-3.6.0/binsync/data/enum.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/func.py` & `binsync-3.6.0/binsync/data/func.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/global_variable.py` & `binsync-3.6.0/binsync/data/global_variable.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/patch.py` & `binsync-3.6.0/binsync/data/patch.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/stack_variable.py` & `binsync-3.6.0/binsync/data/stack_variable.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/state.py` & `binsync-3.6.0/binsync/data/state.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/struct.py` & `binsync-3.6.0/binsync/data/struct.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/type_parser.py` & `binsync-3.6.0/binsync/data/type_parser.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/data/user.py` & `binsync-3.6.0/binsync/data/user.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/angr/artifact_lifter.py` & `binsync-3.6.0/binsync/decompilers/angr/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/angr/control_panel_view.py` & `binsync-3.6.0/binsync/decompilers/angr/control_panel_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class ControlPanelView(BaseView):
     """
     The class for the window that shows changes/info to BinSync data. This includes things like
     changes to functions or structs.
     """
 
     def __init__(self, instance, default_docking_position, controller, *args, **kwargs):
-        super().__init__('sync', instance, default_docking_position, *args, **kwargs)
+        super().__init__('sync', instance, instance.workspace, default_docking_position, *args, **kwargs)
 
         self.base_caption = "BinSync: Control Panel"
 
         self.controller: AngrBinSyncController = controller
         self.control_panel = ControlPanel(self.controller)
         self._init_widgets()
```

### Comparing `binsync-3.5.9/binsync/decompilers/angr/controller.py` & `binsync-3.6.0/binsync/decompilers/angr/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
     #
     #   Utils
     #
 
     def refresh_decompilation(self, func_addr):
         self._main_instance.workspace.jump_to(func_addr)
-        view = self._main_instance.workspace._get_or_create_pseudocode_view()
+        view = self._main_instance.workspace._get_or_create_view("pseudocode", CodeView)
         view.codegen.am_event()
         view.focus()
 
     def decompile_function(self, func, refresh_gui=False):
         # check for known decompilation
         available = self._main_instance.kb.structured_code.available_flavors(func.addr)
         should_decompile = False
```

### Comparing `binsync-3.5.9/binsync/decompilers/angr/plugin.py` & `binsync-3.6.0/binsync/decompilers/angr/plugin.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/binja/artifact_lifter.py` & `binsync-3.6.0/binsync/decompilers/binja/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/binja/binja_binsync.py` & `binsync-3.6.0/binsync/decompilers/binja/binja_binsync.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from collections import defaultdict
 import logging
 
 from binsync.common.ui.version import set_ui_version
 set_ui_version("PySide6")
 from binsync.common.ui.config_dialog import ConfigureBSDialog
 from binsync.common.ui.control_panel import ControlPanel
-from .compat import find_main_window, BinjaDockWidget, create_widget, bn_struct_to_bs, bn_func_to_bs
+from .compat import bn_enum_to_bs, find_main_window, BinjaDockWidget, create_widget, bn_struct_to_bs, bn_func_to_bs
 from .controller import BinjaBinSyncController
 from binsync.data import (
     State, User, Artifact,
     Function, FunctionHeader, FunctionArgument, StackVariable,
     Comment, GlobalVariable, Patch,
     Enum, Struct, StructMember
 )
@@ -142,18 +142,22 @@
             l.debug(f"   -> Function Symbol")
             func = view.get_function_at(sym.address)
             bs_func = bn_func_to_bs(func)
             self._controller.schedule_job(
                 self._controller.push_artifact,
                 FunctionHeader(sym.name, sym.address, type_=bs_func.header.type, args=bs_func.header.args)
             )
-
         elif sym.type == SymbolType.DataSymbol:
             l.debug(f"   -> Data Symbol")
-            pass
+            var: binaryninja.DataVariable = view.get_data_var_at(sym.address)
+            
+            self._controller.schedule_job(
+                self._controller.push_artifact,
+                GlobalVariable(var.address, var.name, type_=str(var.type), size=var.type.width)
+            )
         else:
             l.debug(f"   -> Other Symbol: {sym.type}")
             pass
 
     def type_defined(self, view, name, type_):
         l.debug(f"Type Defined: {name} {type_}")
         if self._controller.sync_lock.locked():
@@ -163,15 +167,16 @@
             bs_struct = bn_struct_to_bs(name, type_)
             self._controller.schedule_job(
                 self._controller.push_artifact,
                 bs_struct
             )
 
         elif isinstance(type_, EnumerationType):
-            pass
+            bs_enum = bn_enum_to_bs(type_)
+            self._controller.schedule_job(self._controller.push_artifact, bs_enum)
 
 
 def start_data_monitor(view, controller):
     notification = DataMonitor(view, controller)
     view.register_notification(notification)
```

### Comparing `binsync-3.5.9/binsync/decompilers/binja/compat.py` & `binsync-3.6.0/binsync/decompilers/binja/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,7 +227,16 @@
             bn_func.start
         )
         for off, var in binja_stack_vars.items()
     }
 
     size = bn_func.address_ranges[0].end - bn_func.address_ranges[0].start
     return Function(bn_func.start, size, header=sync_header, stack_vars=bs_stack_vars)
+
+def bn_enum_to_bs(name: str, bn_enum: binaryninja.EnumerationType):
+    members = {}
+    
+    for enum_member in bn_enum.members:
+        if isinstance(enum_member, binaryninja.EnumerationMember) and isinstance(enum_member.value, int):
+            members[enum_member.name] = enum_member.value
+    
+    return Enum(name, members)
```

### Comparing `binsync-3.5.9/binsync/decompilers/binja/controller.py` & `binsync-3.6.0/binsync/decompilers/binja/controller.py`

 * *Files 21% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Function, FunctionHeader, FunctionArgument, StackVariable,
     Comment, GlobalVariable, Patch,
     Enum, Struct
 )
 import binsync
 
 from .artifact_lifter import BinjaArtifactLifter
-from .compat import bn_func_to_bs, bn_struct_to_bs
+from .compat import bn_enum_to_bs, bn_func_to_bs, bn_struct_to_bs
 
 
 l = logging.getLogger(__name__)
 
 #
 # Helpers
 #
@@ -78,15 +78,15 @@
 #
 # Controller
 #
 
 class BinjaBinSyncController(BinSyncController):
     def __init__(self):
         super(BinjaBinSyncController, self).__init__(artifact_lifter=BinjaArtifactLifter(self))
-        self.bv = None
+        self.bv: binaryninja.BinaryView = None
 
     def binary_hash(self) -> str:
         hash_ = ""
         try:
             hash_ = hashlib.md5(self.bv.file.raw[:]).hexdigest()
         except Exception:
             pass
@@ -161,16 +161,31 @@
                     members.append((bn_type, bs_memb.name))
 
                 s.members = members
 
         return True
 
     @init_checker
+    @fill_event
     def fill_global_var(self, var_addr, user=None, artifact=None, **kwargs):
-        return False
+        changed = False
+        bs_global_var: GlobalVariable = artifact
+        bn_global_var: binaryninja.DataVariable = self.bv.get_data_var_at(var_addr)
+        global_type = self.bv.parse_type_string(bs_global_var.type)
+        
+        if bs_global_var and bs_global_var.name:
+            if bn_global_var is None:
+                bn_global_var = self.bv.define_user_data_var(bs_global_var.addr, global_type, bs_global_var.name)
+                changed = True
+        
+            if bn_global_var.name != bs_global_var.name or bn_global_var.type != global_type:
+                bn_global_var = self.bv.define_user_data_var(bs_global_var.addr, global_type, bs_global_var.name)
+                changed = True
+
+        return changed
 
     @init_checker
     @background_and_wait
     @fill_event
     def fill_function(self, func_addr, user=None, artifact=None, **kwargs):
         """
         Grab all relevant information from the specified user and fill the @bn_func.
@@ -231,15 +246,15 @@
                 try:
                     bn_prototype, _ = self.bv.parse_type_string(prototype_str)
                     valid_type = True
                 except Exception:
                     pass
 
                 if valid_type:
-                    bn_func.function_type = bn_prototype
+                    bn_func.type = bn_prototype
                     updates |= True
 
         return updates
 
     @init_checker
     @fill_event
     def fill_stack_variable(self, func_addr, offset, user=None, artifact=None, bn_func=None, **kwargs):
@@ -280,14 +295,31 @@
     @fill_event
     def fill_comment(self, addr, user=None, artifact=None, bn_func=None, **kwargs):
         # TODO: check if the comment changed when set!
         comment: Comment = artifact
         bn_func.set_comment_at(comment.addr, comment.comment)
 
         return True
+    
+    @init_checker
+    @fill_event
+    def fill_enum(self, name, user=None, artifact=None, ida_code_view=None, **kwargs):
+        bs_enum: Enum = artifact
+        bn_enum: binaryninja.EnumerationType = self.bv.types.get(name)
+        
+        bn_members = []
+        
+        for member_name, value in bs_enum.members.items():
+            bn_members.append({ "name": member_name, "value": value })
+        
+        new_type = binaryninja.TypeBuilder.enumeration(self.bv.arch, bn_members)
+        
+        self.bv.define_user_type(name, new_type)
+            
+        return True
 
     #
     # Artifact API
     #
 
     def function(self, addr, **kwargs) -> Optional[Function]:
         bn_func = self.bv.get_function_at(addr)
@@ -302,37 +334,54 @@
             if bn_func.symbol.type != SymbolType.FunctionSymbol:
                 continue
 
             funcs[bn_func.start] = Function(bn_func.start, bn_func.total_bytes)
             funcs[bn_func.start].name = bn_func.name
 
         return funcs
+    
+
+    def enum(self, name) -> Optional[Enum]:
+        bn_enum = self.bv.types.get(name, None)
+        if bn_enum is None:
+            return None
+        
+        if isinstance(bn_enum, EnumerationType):
+            return bn_enum_to_bs(name, bn_enum)
+        
+        return None
+    
+    def enums(self) -> Dict[str, Enum]:                        
+        return {
+            name: bn_enum_to_bs(''.join(name.name), t) for name, t in self.bv.types.items()
+            if isinstance(t, EnumerationType)
+        }
 
     def struct(self, name) -> Optional[Struct]:
         bn_struct = self.bv.types.get(name, None)
-        if bn_struct is None:
+        if bn_struct is None or not isinstance(bn_struct, StructureType):
             return None
 
         return bn_struct_to_bs(name, bn_struct)
 
     def structs(self) -> Dict[str, Struct]:
         return {
-            name: Struct(name, t.width, {}) for name, t in self.bv.types.items()
+            name: Struct(''.join(name.name), t.width, {}) for name, t in self.bv.types.items()
             if isinstance(t, StructureType)
         }
 
     def global_vars(self) -> Dict[int, GlobalVariable]:
         return {
-            addr: GlobalVariable(addr, self.bv.get_symbol_at(addr) or f"data_{addr:x}")
+            addr: GlobalVariable(addr, var.name or f"data_{addr:x}")
             for addr, var in self.bv.data_vars.items()
         }
     
     def global_var(self, addr) -> Optional[GlobalVariable]:
         try:
             var = self.bv.data_vars[addr]
         except KeyError:
             return None 
             
         gvar = GlobalVariable(
-            addr, self.bv.get_symbol_at(addr) or f"data_{addr:x}", type_=str(var.type), size=var.type.width
+            addr, self.bv.get_symbol_at(addr) or f"data_{addr:x}", type_=str(var.type) if var.type is not None else None, size=var.type.width
         )
-        return gvar
+        return gvar
```

### Comparing `binsync-3.5.9/binsync/decompilers/ghidra/server/artifact_lifter.py` & `binsync-3.6.0/binsync/decompilers/ghidra/server/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ghidra/server/control_panel_window.py` & `binsync-3.6.0/binsync/decompilers/ghidra/server/control_panel_window.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ghidra/server/controller.py` & `binsync-3.6.0/binsync/decompilers/ghidra/server/controller.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ghidra/server/ghidra_client.py` & `binsync-3.6.0/binsync/decompilers/ghidra/server/ghidra_client.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ida/artifact_lifter.py` & `binsync-3.6.0/binsync/decompilers/ida/artifact_lifter.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ida/compat.py` & `binsync-3.6.0/binsync/decompilers/ida/compat.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ida/controller.py` & `binsync-3.6.0/binsync/decompilers/ida/controller.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ida/hooks.py` & `binsync-3.6.0/binsync/decompilers/ida/hooks.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ida/oneliner.py` & `binsync-3.6.0/binsync/decompilers/ida/oneliner.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/decompilers/ida/plugin.py` & `binsync-3.6.0/binsync/decompilers/ida/plugin.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/installer.py` & `binsync-3.6.0/binsync/installer.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync/loggercfg.py` & `binsync-3.6.0/binsync/loggercfg.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/binsync.egg-info/SOURCES.txt` & `binsync-3.6.0/binsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/decompiler_stubs/binja_binsync/plugin.json` & `binsync-3.6.0/decompiler_stubs/binja_binsync/plugin.json`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/setup.cfg` & `binsync-3.6.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 	sortedcontainers
 	toml
 	GitPython
 	filelock
 	pycparser
 	setuptools
 	prompt_toolkit
+	pyside2
 python_requires = >= 3.6
 include_package_data = True
 packages = find:
 
 [options.package_data]
 binsync = 
 	decompiler_stubs/*.py
@@ -35,15 +36,15 @@
 
 [options.entry_points]
 console_scripts = 
 	binsync = binsync.__main__:main
 
 [options.extras_require]
 test = 
-	angr-management>=9.2.40
+	angr-management
 	pytest-qt
 	pyside6
 	flake8
 	pytest
 
 [egg_info]
 tag_build =
```

### Comparing `binsync-3.5.9/setup.py` & `binsync-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/tests/test_angr_gui.py` & `binsync-3.6.0/tests/test_angr_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from PySide6 import QtWidgets
 from PySide6.QtCore import Qt, QPoint
 from PySide6.QtGui import QContextMenuEvent
 from PySide6.QtTest import QTest
 from PySide6.QtCore import Qt, QPoint, QTimer
 from PySide6.QtWidgets import QApplication, QMenu
+from angrmanagement.ui.views import CodeView, DisassemblyView
 from pytestqt.qtbot import QtBot
 import pytest
 
 import angr
 from angrmanagement.ui.dialogs.rename_node import RenameNode
 from angrmanagement.ui.main_window import MainWindow
 
@@ -95,20 +96,21 @@
     assert (context_menu.objectName() == obj_name)
     sync_action = next(filter(lambda x: "Sync" == x.text(), context_menu.actions()))
     sync_action.trigger()
     context_menu.close()
 
 
 def rename_function(qtbot: QtBot, main, func, new_func_name):
-    disasm_view = main.workspace._get_or_create_disassembly_view()
+    disasm_view = main.workspace._get_or_create_view("disassembly", DisassemblyView)
     disasm_view._t_flow_graph_visible = True
     disasm_view.display_function(func)
     disasm_view.decompile_current_function()
     main.workspace.main_instance.join_all_jobs()
-    pseudocode_view = main.workspace._get_or_create_pseudocode_view()
+
+    pseudocode_view = main.workspace._get_or_create_view("pseudocode", CodeView)
     for _, item in pseudocode_view.codegen.map_pos_to_node.items():
         if isinstance(item.obj, angr.analyses.decompiler.structured_codegen.c.CFunction):
             func_node = item.obj
             break
     else:
         raise Exception("The CFunction _instance is not found.")
     rnode = RenameNode(code_view=pseudocode_view, node=func_node)
@@ -116,20 +118,20 @@
     rnode._name_box.setText("")
     qtbot.keyClicks(rnode._name_box, new_func_name)
     qtbot.mouseClick(rnode._ok_button, Qt.MouseButton.LeftButton)
     assert func.name == new_func_name
 
 
 def rename_stack_variable(qtbot:QtBot, main, func, new_var_name, var_offset):
-    disasm_view = main.workspace._get_or_create_disassembly_view()
+    disasm_view = main.workspace._get_or_create_view("disassembly", DisassemblyView)
     disasm_view._t_flow_graph_visible = True
     disasm_view.display_function(func)
     disasm_view.decompile_current_function()
     main.workspace.main_instance.join_all_jobs()
-    pseudocode_view = main.workspace._get_or_create_pseudocode_view()
+    pseudocode_view = main.workspace._get_or_create_view("pseudocode", CodeView)
     for _, item in pseudocode_view.codegen.map_pos_to_node.items():
         if isinstance(item.obj, angr.analyses.decompiler.structured_codegen.c.CVariable) and \
                 isinstance(item.obj.variable, angr.sim_variable.SimStackVariable) and \
                 item.obj.variable.offset == var_offset:
             var_node = item.obj
             break
     else:
```

### Comparing `binsync-3.5.9/tests/test_client.py` & `binsync-3.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `binsync-3.5.9/tests/test_state.py` & `binsync-3.6.0/tests/test_state.py`

 * *Files identical despite different names*

