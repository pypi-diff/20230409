# Comparing `tmp/secimport-0.6.4.tar.gz` & `tmp/secimport-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secimport-0.6.4.tar", max compression
+gzip compressed data, was "secimport-0.7.0.tar", max compression
```

## Comparing `secimport-0.6.4.tar` & `secimport-0.7.0.tar`

### file list

```diff
@@ -1,56 +1,51 @@
--rw-r--r--   0        0        0     1069 2022-07-09 18:11:47.562704 secimport-0.6.4/LICENSE
--rw-r--r--   0        0        0     6848 2022-12-25 07:30:26.367226 secimport-0.6.4/README.md
--rw-r--r--   0        0        0      610 2022-12-25 08:21:21.153429 secimport-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      458 2022-12-11 13:46:57.036860 secimport-0.6.4/src/secimport/__init__.py
--rw-r--r--   0        0        0        0 2022-11-13 12:23:42.304794 secimport-0.6.4/src/secimport/backends/bpftrace_backend/__init__.py
--rw-r--r--   0        0        0      361 2022-11-27 18:12:00.029446 secimport-0.6.4/src/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
--rw-r--r--   0        0        0      373 2022-11-27 18:37:43.118960 secimport-0.6.4/src/secimport/backends/bpftrace_backend/actions/kill_process.bt
--rw-r--r--   0        0        0      124 2022-11-20 15:06:52.887438 secimport-0.6.4/src/secimport/backends/bpftrace_backend/actions/log_file_system.bt
--rw-r--r--   0        0        0      109 2022-11-20 15:06:54.735428 secimport-0.6.4/src/secimport/backends/bpftrace_backend/actions/log_network.bt
--rw-r--r--   0        0        0       71 2022-11-20 15:06:56.608430 secimport-0.6.4/src/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
--rw-r--r--   0        0        0       70 2022-11-20 15:06:58.373383 secimport-0.6.4/src/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
--rw-r--r--   0        0        0      183 2022-11-20 15:09:44.756268 secimport-0.6.4/src/secimport/backends/bpftrace_backend/actions/log_syscall.bt
--rw-r--r--   0        0        0    10257 2022-12-25 08:21:04.919843 secimport-0.6.4/src/secimport/backends/bpftrace_backend/bpftrace_backend.py
--rw-r--r--   0        0        0    22087 2022-12-25 08:20:44.564257 secimport-0.6.4/src/secimport/backends/bpftrace_backend/default.template.bt
--rw-r--r--   0        0        0    21870 2022-12-25 07:24:16.261901 secimport-0.6.4/src/secimport/backends/bpftrace_backend/default.yaml.template.bt
--rw-r--r--   0        0        0       66 2022-11-20 15:02:44.500074 secimport-0.6.4/src/secimport/backends/bpftrace_backend/filters/file_system.bt
--rw-r--r--   0        0        0      175 2022-12-11 12:43:13.751671 secimport-0.6.4/src/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
--rw-r--r--   0        0        0       39 2022-12-23 10:43:24.931362 secimport-0.6.4/src/secimport/backends/bpftrace_backend/filters/networking.bt
--rw-r--r--   0        0        0      557 2022-11-20 15:04:30.742436 secimport-0.6.4/src/secimport/backends/bpftrace_backend/filters/processes.bt
--rwxr-xr-x   0        0        0    22668 2022-12-25 08:23:46.023092 secimport-0.6.4/src/secimport/backends/bpftrace_backend/generate_profile.bt
--rw-r--r--   0        0        0     1334 2022-12-23 10:42:49.339018 secimport-0.6.4/src/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
--rw-r--r--   0        0        0        0 2022-11-13 12:23:42.305630 secimport-0.6.4/src/secimport/backends/common/__init__.py
--rw-r--r--   0        0        0     2899 2022-11-14 00:03:14.413113 secimport-0.6.4/src/secimport/backends/common/abstract_backend.py
--rw-r--r--   0        0        0      112 2022-11-13 23:59:25.241517 secimport-0.6.4/src/secimport/backends/common/instrumentation_backend.py
--rw-r--r--   0        0        0     7184 2022-12-23 10:43:27.807216 secimport-0.6.4/src/secimport/backends/common/utils.py
--rw-r--r--   0        0        0        0 2022-11-13 12:23:42.306522 secimport-0.6.4/src/secimport/backends/dtrace_backend/__init__.py
--rw-r--r--   0        0        0      414 2022-11-13 12:23:42.313376 secimport-0.6.4/src/secimport/backends/dtrace_backend/actions/kill_on_processing.d
--rw-r--r--   0        0        0      661 2022-11-13 12:23:42.313725 secimport-0.6.4/src/secimport/backends/dtrace_backend/actions/kill_process.d
--rw-r--r--   0        0        0      133 2022-11-13 12:23:42.314046 secimport-0.6.4/src/secimport/backends/dtrace_backend/actions/log_file_system.d
--rw-r--r--   0        0        0      123 2022-11-13 12:23:42.314299 secimport-0.6.4/src/secimport/backends/dtrace_backend/actions/log_network.d
--rw-r--r--   0        0        0      187 2022-11-13 12:23:42.314505 secimport-0.6.4/src/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
--rw-r--r--   0        0        0      188 2022-11-13 12:23:42.314711 secimport-0.6.4/src/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
--rw-r--r--   0        0        0       63 2022-11-13 12:23:42.315085 secimport-0.6.4/src/secimport/backends/dtrace_backend/actions/log_syscall.d
--rwxr-xr-x   0        0        0     1616 2022-11-20 15:26:33.285758 secimport-0.6.4/src/secimport/backends/dtrace_backend/default.allowlist.template.d
--rwxr-xr-x   0        0        0     1084 2022-11-20 14:49:36.655475 secimport-0.6.4/src/secimport/backends/dtrace_backend/default.blocklist.template.d
--rwxr-xr-x   0        0        0     1757 2022-11-13 23:49:04.546000 secimport-0.6.4/src/secimport/backends/dtrace_backend/default.template.d
--rwxr-xr-x   0        0        0     2598 2022-11-13 23:49:04.569000 secimport-0.6.4/src/secimport/backends/dtrace_backend/default.yaml.template.d
--rw-r--r--   0        0        0    11045 2022-11-20 17:01:52.110569 secimport-0.6.4/src/secimport/backends/dtrace_backend/dtrace_backend.py
--rw-r--r--   0        0        0      171 2022-11-20 15:36:16.457301 secimport-0.6.4/src/secimport/backends/dtrace_backend/filters/file_system.d
--rw-r--r--   0        0        0      176 2022-11-20 15:36:35.684547 secimport-0.6.4/src/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
--rw-r--r--   0        0        0       30 2022-11-13 12:23:42.317579 secimport-0.6.4/src/secimport/backends/dtrace_backend/filters/networking.d
--rw-r--r--   0        0        0      440 2022-11-20 14:52:56.024913 secimport-0.6.4/src/secimport/backends/dtrace_backend/filters/processes.d
--rw-r--r--   0        0        0      974 2022-11-20 14:49:39.808573 secimport-0.6.4/src/secimport/backends/dtrace_backend/generate_profile.d
--rw-r--r--   0        0        0       28 2022-11-13 12:23:42.318284 secimport-0.6.4/src/secimport/backends/dtrace_backend/headers/destructive.d
--rw-r--r--   0        0        0     1240 2022-11-30 19:15:28.183242 secimport-0.6.4/src/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
--rwxr-xr-x   0        0        0     4402 2022-11-20 16:31:43.965736 secimport-0.6.4/src/secimport/backends/dtrace_backend/py_sandbox.d
--rw-r--r--   0        0        0     6744 2022-12-25 08:16:01.684646 secimport-0.6.4/src/secimport/cli.py
--rwxr-xr-x   0        0        0    34087 2022-12-25 08:07:53.328099 secimport-0.6.4/src/secimport/profiles/example.bt
--rwxr-xr-x   0        0        0    12405 2022-12-11 13:56:26.341190 secimport-0.6.4/src/secimport/profiles/example.d
--rw-r--r--   0        0        0     2913 2022-11-13 23:51:00.591764 secimport-0.6.4/src/secimport/profiles/example.yaml
--rwxr-xr-x   0        0        0     1064 2022-12-25 08:07:53.307321 secimport-0.6.4/src/secimport/profiles/processing_sandbox.bt
--rwxr-xr-x   0        0        0    22294 2022-12-23 10:38:56.924695 secimport-0.6.4/src/secimport/profiles/trace.bt
--rw-r--r--   0        0        0     3701 2022-11-20 18:54:50.806478 secimport-0.6.4/src/secimport/sandbox_helper.py
--rwxr-xr-x   0        0        0    28551 2022-12-13 07:47:13.737397 secimport-0.6.4/src/secimport/traced_modules.bt
--rw-r--r--   0        0        0     8329 2022-12-25 08:23:50.780671 secimport-0.6.4/setup.py
--rw-r--r--   0        0        0     7524 2022-12-25 08:23:50.781134 secimport-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-07-09 18:11:47.562704 secimport-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4389 2023-04-09 18:52:50.816277 secimport-0.7.0/README.md
+-rw-r--r--   0        0        0     1715 2023-04-09 18:52:50.838075 secimport-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      437 2023-04-09 18:52:50.838697 secimport-0.7.0/secimport/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:52:50.838812 secimport-0.7.0/secimport/backends/bpftrace_backend/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-09 18:52:50.839406 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
+-rw-r--r--   0        0        0      373 2023-04-09 18:52:50.839675 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/kill_process.bt
+-rw-r--r--   0        0        0      125 2023-04-09 18:52:50.840067 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_file_system.bt
+-rw-r--r--   0        0        0      110 2023-04-09 18:52:50.840472 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_network.bt
+-rw-r--r--   0        0        0       72 2023-04-09 18:52:50.840884 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
+-rw-r--r--   0        0        0       71 2023-04-09 18:52:50.841620 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
+-rw-r--r--   0        0        0      183 2023-04-09 18:52:50.841872 secimport-0.7.0/secimport/backends/bpftrace_backend/actions/log_syscall.bt
+-rw-r--r--   0        0        0     8797 2023-04-09 18:52:50.842186 secimport-0.7.0/secimport/backends/bpftrace_backend/bpftrace_backend.py
+-rw-r--r--   0        0        0    22157 2023-04-09 18:52:50.843083 secimport-0.7.0/secimport/backends/bpftrace_backend/default.template.bt
+-rw-r--r--   0        0        0    23175 2023-04-09 18:52:50.844075 secimport-0.7.0/secimport/backends/bpftrace_backend/default.yaml.template.bt
+-rw-r--r--   0        0        0       67 2023-04-09 18:52:50.844594 secimport-0.7.0/secimport/backends/bpftrace_backend/filters/file_system.bt
+-rw-r--r--   0        0        0      176 2023-04-09 18:52:50.845002 secimport-0.7.0/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
+-rw-r--r--   0        0        0       40 2023-04-09 18:52:50.845662 secimport-0.7.0/secimport/backends/bpftrace_backend/filters/networking.bt
+-rw-r--r--   0        0        0      553 2023-04-09 18:52:50.846141 secimport-0.7.0/secimport/backends/bpftrace_backend/filters/processes.bt
+-rwxr-xr-x   0        0        0    22668 2023-04-09 18:52:50.846870 secimport-0.7.0/secimport/backends/bpftrace_backend/generate_profile.bt
+-rw-r--r--   0        0        0     1203 2023-04-09 18:52:50.847215 secimport-0.7.0/secimport/backends/bpftrace_backend/new_template.bt
+-rw-r--r--   0        0        0      502 2023-04-09 18:52:50.847539 secimport-0.7.0/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
+-rw-r--r--   0        0        0        0 2023-04-09 18:52:50.847638 secimport-0.7.0/secimport/backends/common/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-09 18:52:50.847941 secimport-0.7.0/secimport/backends/common/instrumentation_backend.py
+-rw-r--r--   0        0        0     7102 2023-04-09 18:52:50.848401 secimport-0.7.0/secimport/backends/common/utils.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:52:50.848529 secimport-0.7.0/secimport/backends/dtrace_backend/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-09 18:52:50.849122 secimport-0.7.0/secimport/backends/dtrace_backend/actions/kill_on_processing.d
+-rw-r--r--   0        0        0      662 2023-04-09 18:52:50.850407 secimport-0.7.0/secimport/backends/dtrace_backend/actions/kill_process.d
+-rw-r--r--   0        0        0      134 2023-04-09 18:52:50.850975 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_file_system.d
+-rw-r--r--   0        0        0      124 2023-04-09 18:52:50.851498 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_network.d
+-rw-r--r--   0        0        0      187 2023-04-09 18:52:50.852004 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
+-rw-r--r--   0        0        0      188 2023-04-09 18:52:50.852531 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
+-rw-r--r--   0        0        0       64 2023-04-09 18:52:50.853048 secimport-0.7.0/secimport/backends/dtrace_backend/actions/log_syscall.d
+-rwxr-xr-x   0        0        0     1606 2023-04-09 18:52:50.853621 secimport-0.7.0/secimport/backends/dtrace_backend/default.allowlist.template.d
+-rwxr-xr-x   0        0        0     1081 2023-04-09 18:52:50.854185 secimport-0.7.0/secimport/backends/dtrace_backend/default.blocklist.template.d
+-rwxr-xr-x   0        0        0     1753 2023-04-09 18:52:50.854734 secimport-0.7.0/secimport/backends/dtrace_backend/default.template.d
+-rwxr-xr-x   0        0        0     2587 2023-04-09 18:52:50.855314 secimport-0.7.0/secimport/backends/dtrace_backend/default.yaml.template.d
+-rw-r--r--   0        0        0     8813 2023-04-09 18:52:50.856136 secimport-0.7.0/secimport/backends/dtrace_backend/dtrace_backend.py
+-rw-r--r--   0        0        0      172 2023-04-09 18:52:50.857008 secimport-0.7.0/secimport/backends/dtrace_backend/filters/file_system.d
+-rw-r--r--   0        0        0      177 2023-04-09 18:52:50.857464 secimport-0.7.0/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
+-rw-r--r--   0        0        0       31 2023-04-09 18:52:50.857889 secimport-0.7.0/secimport/backends/dtrace_backend/filters/networking.d
+-rw-r--r--   0        0        0      436 2023-04-09 18:52:50.858379 secimport-0.7.0/secimport/backends/dtrace_backend/filters/processes.d
+-rw-r--r--   0        0        0      969 2023-04-09 18:52:50.858858 secimport-0.7.0/secimport/backends/dtrace_backend/generate_profile.d
+-rw-r--r--   0        0        0       30 2023-04-09 18:52:50.859176 secimport-0.7.0/secimport/backends/dtrace_backend/headers/destructive.d
+-rw-r--r--   0        0        0     1238 2023-04-09 18:52:50.859698 secimport-0.7.0/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
+-rwxr-xr-x   0        0        0     4389 2023-04-09 18:52:50.860203 secimport-0.7.0/secimport/backends/dtrace_backend/py_sandbox.d
+-rw-r--r--   0        0        0    13365 2023-04-09 18:52:50.860554 secimport-0.7.0/secimport/cli.py
+-rwxr-xr-x   0        0        0    22294 2023-04-09 18:52:50.860987 secimport-0.7.0/secimport/profiles/trace.bt
+-rw-r--r--   0        0        0     3048 2023-04-09 18:52:50.861289 secimport-0.7.0/secimport/sandbox_helper.py
+-rw-r--r--   0        0        0     5705 2023-04-09 18:53:17.178027 secimport-0.7.0/setup.py
+-rw-r--r--   0        0        0     5065 2023-04-09 18:53:17.178415 secimport-0.7.0/PKG-INFO
```

### Comparing `secimport-0.6.4/LICENSE` & `secimport-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secimport-0.6.4/src/secimport/backends/bpftrace_backend/bpftrace_backend.py` & `secimport-0.7.0/secimport/backends/dtrace_backend/dtrace_backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,192 +1,148 @@
 """
-Import python modules with bpftrace supervision.
+Import python modules with dtrace supervision.
+
 Copyright (c) 2022 Avi Lumelsky
 """
-
 import importlib
+import importlib.machinery  # important for importlib to work for our use case
 import os
-from sys import executable as PYTHON_EXECUTABLE
 import stat
 import time
 from pathlib import Path
 from typing import List
 
+
 from secimport.backends.common.instrumentation_backend import InstrumentationBackend
 from secimport.backends.common.utils import (
     BASE_DIR_NAME,
     SECIMPORT_ROOT,
     render_syscalls_filter,
 )
 
-TEMPLATES_DIR_NAME = SECIMPORT_ROOT / "backends" / "bpftrace_backend"
+TEMPLATES_DIR_NAME = SECIMPORT_ROOT / "backends" / "dtrace_backend"
+DEFAULT_BACKEND = InstrumentationBackend.DTRACE
+PROFILES_DIR_NAME = SECIMPORT_ROOT / "profiles"
 
 
-def create_bpftrace_script_for_module(
+def run_dtrace_script_for_module(
     module_name: str,
     allow_shells: bool,
     allow_networking: bool,
+    use_sudo: bool,
     log_python_calls: bool,
     log_syscalls: bool,
     log_network: bool,
     log_file_system: bool,
     destructive: bool,
-    syscalls_allowlist: List[str] = None,
-    syscalls_blocklist: List[str] = None,
     templates_dir: Path = TEMPLATES_DIR_NAME,
-) -> Path:
-    """
-    # Template components available at the moment:
-    # ###DESTRUCTIVE###
-    # ###FUNCTION_ENTRY###
-    # ###FUNCTION_EXIT###
-    # ###SYSCALL_ENTRY###
-    # ###MODULE_NAME###
-    """
-
-    module = importlib.machinery.PathFinder().find_spec(module_name)
-    if module is None:
-        raise ModuleNotFoundError(module_name)
-    module_traced_name = module.origin  # e.g this.py
-
-    assert not (
-        syscalls_allowlist is not None and syscalls_blocklist is not None
-    ), "Please specify either syscalls_allowlist OR syscalls_blocklist."
-
-    # If we have an allowlist
-    if syscalls_allowlist is not None:
-        script_template = render_bpftrace_probe_for_module(
-            module_name=module_name,
-            destructive=destructive,
-            templates_dir=templates_dir,
-        )
-        syscalls_filter = render_syscalls_filter(
-            syscalls_list=syscalls_allowlist,
-            allow=True,
-            instrumentation_backend=InstrumentationBackend.EBPF,
-            module_name=module_traced_name,
-        )
-        script_template = script_template.replace(
-            "###SYSCALL_FILTER###", syscalls_filter
-        )
-
-    elif syscalls_blocklist is not None:
-        # If we have a blocklist
-        script_template = render_bpftrace_probe_for_module(
-            module_name=module_name,
-            destructive=destructive,
-            templates_dir=templates_dir,
-        )
-        syscalls_filter = render_syscalls_filter(
-            syscalls_list=syscalls_allowlist,
-            allow=True,
-            instrumentation_backend=InstrumentationBackend.EBPF,
-            module_name=module_traced_name,
-        )
-        script_template = script_template.replace(
-            "###SYSCALL_FILTER###", syscalls_filter
-        )
-
-    else:
-        script_template = render_bpftrace_template(
-            module_traced_name=module_traced_name,
-            allow_shells=allow_shells,
-            allow_networking=allow_networking,
-            log_python_calls=log_python_calls,
-            log_syscalls=log_syscalls,
-            log_network=log_network,
-            log_file_system=log_file_system,
-            destructive=destructive,
-            templates_dir=templates_dir,
-        )
-
-    # Creating a dscript file with the modified template
-    if not os.path.exists(BASE_DIR_NAME):
-        os.mkdir(BASE_DIR_NAME)
-
-    module_file_name = os.path.join(BASE_DIR_NAME, f"bpftrace_sandbox_{module_name}.bt")
-    with open(module_file_name, "w") as module_file:
-        module_file.write(script_template)
+):
+    module_file_path = create_dtrace_script_for_module(
+        module_name=module_name,
+        allow_shells=allow_shells,
+        allow_networking=allow_networking,
+        log_python_calls=log_python_calls,
+        log_syscalls=log_syscalls,
+        log_network=log_network,
+        log_file_system=log_file_system,
+        destructive=destructive,
+        templates_dir=templates_dir,
+    )
+    output_file = BASE_DIR_NAME / f"dtrace_sandbox_{module_name}.log"
+    current_pid = os.getpid()
+    dtrace_command = f'{"sudo " if use_sudo else ""} dtrace -q -s {module_file_path} -p {current_pid} -o {output_file} &2>/dev/null'
+    print("(running dtrace supervisor): ", dtrace_command)
+    st = os.stat(module_file_path)
+    os.chmod(module_file_path, st.st_mode | stat.S_IEXEC)
+    os.system(dtrace_command)
 
-    # TODO: FIGURE OUT A WAY TO COMPILE WITHOUT EXECUTING - MSKING SURE THE GENERATION WORKED SYNTAX-WISE.
-    return module_file_name
+    # TODO: wait for dtrace to start explicitly using an event/fd, not time based - although 2 seconds is more than enough.
+    # TODO: add startup logs for dropped packets without python modules (until the first python enter takes place in the syscalls probe, the python module is null).
+    time.sleep(5)
+    return True
 
 
-def run_bpftrace_script_for_module(
+def create_dtrace_script_for_module(
     module_name: str,
     allow_shells: bool,
     allow_networking: bool,
     log_python_calls: bool,
     log_syscalls: bool,
     log_network: bool,
     log_file_system: bool,
     destructive: bool,
-    syscalls_allowlist: List[str],
-    syscalls_blocklist: List[str],
-    use_sudo: bool = False,
     templates_dir: Path = TEMPLATES_DIR_NAME,
-):
-    module_file_path = create_bpftrace_script_for_module(
-        module_name=module_name,
+) -> str:
+    module = importlib.machinery.PathFinder().find_spec(module_name)
+    if module is None:
+        raise ModuleNotFoundError(module_name)
+    module_traced_name = module.origin  # e.g this.py
+
+    script_template = render_dscript_template(
+        module_traced_name=module_traced_name,
         allow_shells=allow_shells,
         allow_networking=allow_networking,
         log_python_calls=log_python_calls,
         log_syscalls=log_syscalls,
         log_network=log_network,
         log_file_system=log_file_system,
         destructive=destructive,
-        syscalls_allowlist=syscalls_allowlist,
-        syscalls_blocklist=syscalls_blocklist,
         templates_dir=templates_dir,
     )
-    output_file = BASE_DIR_NAME / f"bpftrace_sandbox_{module_name}.log"
-    current_pid = os.getpid()
-    bpftrace_command = f'{"sudo " if use_sudo else ""} {module_file_path} --unsafe -q -p {current_pid} -o {output_file} &2>/dev/null'
-    st = os.stat(module_file_path)
-    os.chmod(module_file_path, st.st_mode | stat.S_IEXEC)
-    print("(sandbox command): ", bpftrace_command)
-    print()
-    print("Waiting for bpftrace.... ")
-    os.system(bpftrace_command)
-    time.sleep(10)  # TODO: change to fd creation (event)
-    return True
+
+    # Creating a dscript file with the modified template
+    if not os.path.exists(BASE_DIR_NAME):
+        os.mkdir(BASE_DIR_NAME)
+
+    module_file_name = os.path.join(BASE_DIR_NAME, f"dtrace_sandbox_{module_name}.d")
+    with open(module_file_name, "w") as module_file:
+        module_file.write(script_template)
+
+    # Making sure the script compiles
+    dtrace_compile_command = f"dtrace -s {module_file_name} -e"
+    compile_exit_code = os.system(dtrace_compile_command)
+    assert (
+        compile_exit_code == 0
+    ), f"Failed to compile the dtrace script at {module_file_name}"
+    print("Successfully compiled dtrace profile: ", module_file_name)
+    return module_file_name
 
 
-def render_bpftrace_template(
+def render_dscript_template(
     module_traced_name: str,
     allow_shells: bool,
     allow_networking: bool,
     log_python_calls: bool,
     log_syscalls: bool,
     log_network: bool,
     log_file_system: bool,
     destructive: bool,
     templates_dir: Path = TEMPLATES_DIR_NAME,
-    default_template_filename: str = "default.template.bt",
-    interpreter_path: str = PYTHON_EXECUTABLE,
+    default_template_filename: str = "default.template.d",
 ):
     script_template = open(
         templates_dir / default_template_filename,
         "r",
     ).read()
 
-    # Updating the right binary to be probed by bpftrace
-    script_template = script_template.replace(
-        "###INTERPRETER_PATH###", interpreter_path
-    )
+    if destructive is True:
+        destructive = open(templates_dir / "headers/destructive.d", "r").read()
+        script_template = script_template.replace("###DESTRUCTIVE###", destructive)
+    else:
+        script_template = script_template.replace("###DESTRUCTIVE###", "")
 
     # PYTHON instrumentations
     code_syscall_entry = ""
     if log_python_calls is True:
         code_function_entry = open(
-            templates_dir / "actions/log_python_module_entry.bt",
+            templates_dir / "actions/log_python_module_entry.d",
             "r",
         ).read()
         code_function_exit = open(
-            templates_dir / "actions/log_python_module_exit.bt",
+            templates_dir / "actions/log_python_module_exit.d",
             "r",
         ).read()
         script_template = script_template.replace(
             "###FUNCTION_ENTRY###", code_function_entry
         )
         script_template = script_template.replace(
             "###FUNCTION_EXIT###", code_function_exit
@@ -194,117 +150,113 @@
     else:
         script_template = script_template.replace("###FUNCTION_ENTRY###", "")
         script_template = script_template.replace("###FUNCTION_EXIT###", "")
 
     # SYSCALLS instrumentations
     if log_syscalls is True:
         _code = open(
-            templates_dir / "actions/log_syscall.bt",
+            templates_dir / "actions/log_syscall.d",
             "r",
         ).read()
         code_syscall_entry += f"{_code};\n"
 
     if log_file_system is True:
         filter_fs_code = open(
-            templates_dir / "filters/file_system.bt",
+            templates_dir / "filters/file_system.d",
             "r",
         ).read()
         code_syscall_entry += f"{filter_fs_code}\n{{"
         action_log_file_system = open(
-            templates_dir / "actions/log_file_system.bt",
+            templates_dir / "actions/log_file_system.d",
             "r",
         ).read()
         code_syscall_entry += f"{action_log_file_system}}}\n"
 
     if allow_networking is False or log_network is True:
         filter_networking_code = open(
-            templates_dir / "filters/networking.bt",
+            templates_dir / "filters/networking.d",
             "r",
         ).read()
         code_syscall_entry += f"{filter_networking_code}{{\n"
 
         if log_network is True:
             action_log_network = open(
-                templates_dir / "actions/log_network.bt",
+                templates_dir / "actions/log_network.d",
                 "r",
             ).read()
             code_syscall_entry += f"{action_log_network}\n"
 
         if allow_networking is False:
             action_kill = open(
-                templates_dir / "actions/kill_process.bt",
+                templates_dir / "actions/kill_process.d",
                 "r",
             ).read()
             code_syscall_entry += f"{action_kill}\n"
         code_syscall_entry += "}\n"
 
     if allow_shells is False:
         filter_processes_code = open(
-            templates_dir / "filters/processes.bt",
+            templates_dir / "filters/processes.d",
             "r",
         ).read()
         code_syscall_entry += f"{filter_processes_code}{{\n"
         action_kill_on_processing = open(
-            templates_dir / "actions/kill_on_processing.bt",
+            templates_dir / "actions/kill_on_processing.d",
             "r",
         ).read()
         code_syscall_entry += f"{action_kill_on_processing}}}\n"
 
     script_template = script_template.replace("###SYSCALL_ENTRY###", code_syscall_entry)
     script_template = script_template.replace("###MODULE_NAME###", module_traced_name)
-
-    # Updating the destructive behavior
-    script_template = script_template.replace(
-        "###DESTRUCTIVE###", "1" if destructive else "0"
-    )
     return script_template
 
 
-def render_bpftrace_probe_for_module(
+def render_dtrace_probe_for_module(
     module_name: str,
     destructive: bool,
+    syscalls_allowlist: List[str],
     templates_dir: Path = TEMPLATES_DIR_NAME,
-    interpreter_path: str = PYTHON_EXECUTABLE,
 ) -> str:
     # Loading the probe allowlist template
     probe_template = open(
-        templates_dir / "probes/module_syscalls_allowlist_template.bt",
+        templates_dir / "probes/module_syscalls_allowlist_template.d",
         "r",
     ).read()
 
+    # Adding a syscalls filter
+    syscalls_filter = render_syscalls_filter(
+        syscalls_list=syscalls_allowlist,
+        allow=True,
+        instrumentation_backend=InstrumentationBackend.DTRACE,
+    )
+    probe_template = probe_template.replace("###SYSCALL_FILTER###", syscalls_filter)
+
     # Adding a probe filter for the specified python module
     supervision_filter = open(
-        templates_dir / "filters/is_current_module_under_supervision.bt",
+        templates_dir / "filters/is_current_module_under_supervision.d",
         "r",
     ).read()
 
     # Adding the action according to the 'destructive' flag:  kill if destructive, log otherwise
     supervision_action = ""
     if destructive is True:
         action_kill_process = open(
-            templates_dir / "actions/kill_process.bt",
+            templates_dir / "actions/kill_process.d",
             "r",
         ).read()
         supervision_action = f"{{{action_kill_process}}}\n"
     else:
         action_log_syscall = open(
-            templates_dir / "actions/log_syscall.bt",
+            templates_dir / "actions/log_syscall.d",
             "r",
         ).read()
         supervision_action = f"{{{action_log_syscall}}}\n"
 
-    # Updating the template with the filters, their actions, and module name
+    # Updating the template
     probe_template = probe_template.replace(
         "###SUPERVISED_MODULES_FILTER###", supervision_filter
     )
     probe_template = probe_template.replace(
         "###SUPERVISED_MODULES_ACTION###", supervision_action
     )
     probe_template = probe_template.replace("###MODULE_NAME###", module_name)
-
-    # Updating the destructive behavior
-    probe_template = probe_template.replace(
-        "###DESTRUCTIVE###", "1" if destructive else "0"
-    )
-
-    probe_template = probe_template.replace("###INTERPRETER_PATH###", interpreter_path)
     return probe_template
```

### Comparing `secimport-0.6.4/src/secimport/backends/bpftrace_backend/default.template.bt` & `secimport-0.7.0/secimport/backends/bpftrace_backend/default.template.bt`

 * *Files 0% similar despite different names*

```diff
@@ -705,23 +705,24 @@
     ###SYSCALL_ENTRY###
 }
 
 
 // Invoked before importlib imports a module
 // import__find__load__start(str modulename)
 usdt:###INTERPRETER_PATH###:import__find__load__start {
+    // TODO: verify that the module is allowed in the syscall filter.
     // @imports[arg0] = count();
     // printf('importing %s', arg0);
 }
 
-// Invoked after importlib imports a module 
+// Invoked after importlib imports a module
 // import__find__load__done(str modulename, int found)
 usdt:###INTERPRETER_PATH###:import__find__load__done{
     // printf('imported %s with result %d', arg0, arg1);
 }
 
 END {
     clear(@sysname);
     clear(@sysnum);
     clear(@entrypoints);
     clear(@syscalls_filters);
-}
+}
```

### Comparing `secimport-0.6.4/src/secimport/backends/bpftrace_backend/default.yaml.template.bt` & `secimport-0.7.0/secimport/profiles/trace.bt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 #!/usr/bin/env bpftrace
 
+// A profiling script that logs all the syscalls, per python module.
+// It can be attached to a running process using -p or can be used to trace a python shell interactively.
+//
+// Usage:
+// ./trace.bt -c Python-3.10.0/python
+
 BEGIN {
     // Mapping all syscalls both ways, based on https://github.com/iovisor/bpftrace/blob/2c7a7a598dbe1aa790db2dfe2db242aa69137d5b/tools/syscount.bt
     // Generates using bash:
     //   $ apt-get install auditd
     //   $ ausyscall --dump | awk 'NR > 1 { printf("\t@sysname[%d] = \"%s\";\n", $1, $2); }';
     printf("REGISTERING SYSCALLS...\n");
     @sysname[0] = "read";
@@ -675,52 +681,46 @@
 	@sysnum["pwritev2"] = 328;
 	@sysnum["pkey_mprotect"] = 329;
 	@sysnum["pkey_alloc"] = 330;
 	@sysnum["pkey_free"] = 331;
 	@sysnum["statx"] = 332;
 	@sysnum["io_pgetevents"] = 333;
 	@sysnum["rseq"] = 334;
-    
-    ###SYSCALL_FILTER###
-    printf("STARTED\n");
+    printf("Tracing Modules - Exit gracefully with Ctrl+D\n")
 }
 
-
-usdt:###INTERPRETER_PATH###:function__entry {
+usdt:/workspace/Python-3.10.0/python:function__entry {
         @["depth"]++;
         @entrypoints[str(arg0)] = @["depth"];
         @globals["previous_module"] = @globals["current_module"];
         @globals["current_module"] = str(arg0);
-        @latest_supervised_module =  str(arg0);
-        // printf("%s, %s, depth=%d\n", str(arg0), str(arg1), @["depth"]);
-}
 
-usdt:###INTERPRETER_PATH###:function__return {
-    @["depth"]--;
-}
-
-tracepoint:raw_syscalls:sys_enter /comm == "python"/ {
-    ###SUPERVISED_MODULES_PROBES###
+        // To trace python calls in the console, uncomment:
+        // printf("%s, %s, depth=%d\n", str(arg0), str(arg1), @["depth"]) ;
 }
 
-// Invoked before importlib imports a module ('__import__()' or 'import')
-usdt:###INTERPRETER_PATH###:import__find__load__start {
-    
+usdt:/workspace/Python-3.10.0/python:function__return {
+        @["depth"]--;
 }
 
-// Invoked after importlib imports a module 
-usdt:###INTERPRETER_PATH###:import__find__load__done{
-
+tracepoint:raw_syscalls:sys_enter /comm == "python"/ {
+    // @modules_syscalls[@globals["current_module"], @sysname[args->id], @["depth"]] = count();
+    @modules_syscalls[@globals["current_module"], @sysname[args->id]] = count();
+    @syscalls[@sysname[args->id]] = count();
 }
 
-// Invoked when a new line is entered
-usdt:###INTERPRETER_PATH###:line {
-
-}
 
 END {
+    printf("Summary:");
+	printf(" %-32s %-10s %-22s %8s\r\n", "FILE", "TYPE", "NAME", "COUNT");
+	printf("\r\nAll syscalls (count):\r\n");
+	print(@syscalls);
+    printf("\r\nSyscalls Per Python Module:\r\n");
+    print(@modules_syscalls);
+	printf("\r\nDone.\r\n");
     clear(@sysname);
     clear(@sysnum);
+    clear(@syscalls);
+    clear(@modules_syscalls);
     clear(@entrypoints);
-    clear(@syscalls_filters);
-    clear(@globals);
-}
+    clear(@globals)
+}
```

### Comparing `secimport-0.6.4/src/secimport/backends/bpftrace_backend/filters/processes.bt` & `secimport-0.7.0/secimport/backends/bpftrace_backend/filters/processes.bt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
     if (@sysname[args->id] == "posix_spawn" ||
         @sysname[args->id] == "posix_spawnp" ||
         @sysname[args->id] == "clone" ||
         @sysname[args->id] == "__clone2" ||
         @sysname[args->id] == "clone3" ||
         @sysname[args->id] == "fork" ||
         @sysname[args->id] == "vfork" ||
-        @sysname[args->id] == "forkexec" || 
-        @sysname[args->id] == "execl" || 
-        @sysname[args->id] == "execlp" || 
-        @sysname[args->id] == "execle" || 
-        @sysname[args->id] == "execv" || 
-        @sysname[args->id] == "execvp")
+        @sysname[args->id] == "forkexec" ||
+        @sysname[args->id] == "execl" ||
+        @sysname[args->id] == "execlp" ||
+        @sysname[args->id] == "execle" ||
+        @sysname[args->id] == "execv" ||
+        @sysname[args->id] == "execvp")
```

### Comparing `secimport-0.6.4/src/secimport/backends/bpftrace_backend/generate_profile.bt` & `secimport-0.7.0/secimport/backends/bpftrace_backend/generate_profile.bt`

 * *Files 0% similar despite different names*

```diff
@@ -711,15 +711,15 @@
 // Invoked before importlib imports a module
 // import__find__load__start(str modulename)
 usdt:###INTERPRETER_PATH###:import__find__load__start {
     // @imports[arg0] = count();
     // printf('importing %s', arg0);
 }
 
-// Invoked after importlib imports a module 
+// Invoked after importlib imports a module
 // import__find__load__done(str modulename, int found)
 usdt:###INTERPRETER_PATH###:import__find__load__done{
     // printf('imported %s with result %d', arg0, arg1);
 }
 
 END {
     printf("Summary:");
@@ -731,8 +731,8 @@
 	printf("\r\nDone.\r\n");
     clear(@sysname);
     clear(@sysnum);
     clear(@syscalls);
     clear(@modules_syscalls);
     clear(@entrypoints);
     clear(@globals);
-}
+}
```

### Comparing `secimport-0.6.4/src/secimport/backends/common/utils.py` & `secimport-0.7.0/secimport/backends/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     module_name=None,
 ):
     assert isinstance(allow, bool), '"allow" must be a bool value'
     # "=="" means the syscall matches (blocklist), while "!="" means allow only the following.
     match_sign = "!=" if allow else "=="
     syscalls_filter = ""
     for i, _syscall in enumerate(syscalls_list):
+        _syscall = _syscall.strip()
         if i > 0:
             if instrumentation_backend == InstrumentationBackend.DTRACE:
                 syscalls_filter += " && "
         assert isinstance(
             _syscall, str
         ), f"The provided syscall it not a syscall string name: {_syscall}"
 
@@ -59,23 +60,25 @@
             # strncmp returns 0 if it is a match
             # syscalls_filter += f'(strncmp(@sysname[args->id],  "{_syscall}", 24) {expected_output_value})'
             _module_name = (
                 f'"{module_name}"'
                 if module_name is not None
                 else '@globals["current_module"]'
             )
-            syscalls_filter += f"@syscalls_filters[{_module_name}, \"{_syscall}\"] = {expected_output_value};"
+            syscalls_filter += f'@syscalls_filters[{_module_name}, "{_syscall}"] = {expected_output_value};'
             syscalls_filter += "\n\t"
         else:
             raise NotImplementedError(
                 f"backend '{instrumentation_backend}' is not supported"
             )
 
         filter_name = "allowlist" if allow else "blocklist"
-        print(f"Adding syscall {_syscall} to {filter_name} for module {module_name}")
+        print(
+            f"[debug] adding syscall {_syscall} to {filter_name} for module {module_name}"
+        )
     return syscalls_filter
 
 
 def build_module_sandbox_from_yaml_template(
     template_path: Path,
     backend: InstrumentationBackend = DEFAULT_BACKEND,
 ):
@@ -99,15 +102,15 @@
     safe_yaml = yaml.safe_load(open(template_path, "r").read())
     parsed_probes = []
     syscalls_filter = ""
     for module_name, module_config in safe_yaml.get("modules", {}).items():
         # Finding the module without loading
         module = importlib.machinery.PathFinder().find_spec(module_name)
         if module is None:
-            msg = f"Warning: {module_name} is not present in the current environment. It is required in order to generate a sandbox with correct a import name."
+            pass
             # raise ModuleNotFoundError(msg)
 
         # Tracing module entrypoint
         module_traced_name = module.origin if module is not None else module_name
         # module_traced_name = os.path.split(module_traced_name)[:-1][0]
 
         _destructive = module_config.get("destructive")
@@ -130,15 +133,15 @@
             )
 
             module_sandbox_probe = render_dtrace_probe_for_module(
                 module_name=module_traced_name,
                 destructive=_destructive,
                 syscalls_allowlist=_syscall_allowlist,
             )
-            sandbox_file_name = f"default.yaml.template.d"
+            sandbox_file_name = "default.yaml.template.d"
             script_template = open(
                 DTRACE_TEMPLATES_DIR_NAME / sandbox_file_name,
                 "r",
             ).read()
         elif backend == InstrumentationBackend.EBPF:
             from secimport.backends.bpftrace_backend.bpftrace_backend import (
                 render_bpftrace_probe_for_module,
@@ -151,15 +154,15 @@
             # Adding a syscalls filter
             syscalls_filter += render_syscalls_filter(
                 syscalls_list=_syscall_allowlist,
                 allow=True,
                 instrumentation_backend=InstrumentationBackend.EBPF,
                 module_name=module_traced_name,
             )
-            sandbox_file_name = f"default.yaml.template.bt"
+            sandbox_file_name = "default.yaml.template.bt"
             script_template = open(
                 BPFTRACE_TEMPLATES_DIR_NAME / sandbox_file_name,
                 "r",
             ).read()
         assert module_sandbox_probe, ValueError(
             f"Failed to create a probe for module {module_name}"
         )
```

### Comparing `secimport-0.6.4/src/secimport/backends/dtrace_backend/actions/kill_process.d` & `secimport-0.7.0/secimport/backends/dtrace_backend/actions/kill_process.d`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,8 +3,8 @@
                 printf("\t\tKilling process; depth=%d sandboxed_depth=%d module=%s\r\n", self->depth, depth_matrix[_current_module_str], _current_module_str);
                 printf("\t\tIf this behavior is unexpected, add the syscall '%s' to your list. The policy that blocked this syscall is logged above the stackstrace.\r\n", probefunc);
                 stop();
                 printf("\t\tKILLING...\r\n");
                 system("\t\tkill -9 %d", pid);
                 printf("\t\tKILLED.\r\n");
                 printf("\t####################\r\n");
-                exit(-1);
+                exit(-1);
```

### Comparing `secimport-0.6.4/src/secimport/backends/dtrace_backend/default.allowlist.template.d` & `secimport-0.7.0/secimport/backends/dtrace_backend/default.allowlist.template.d`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 #!/usr/sbin/dtrace -Zs
 /*
 	This script generates a list of syscalls for a given program.
 	It generates a filter for dscript.
 	The first probe can be replaced with the output of the following usage.
 
-	USAGE:	sudo dtrace -s src/secimport/templates/default.allowlist.template.d -c "python -m http.server" # then CTRL+C
+	USAGE:	sudo dtrace -s secimport/templates/default.allowlist.template.d -c "python -m http.server" # then CTRL+C
 */
 
 #pragma D option destructive
 #pragma D option quiet
 #pragma D option switchrate=1
 
 /* Non-Allowed syscalls probe - Kills the process */
 /* Replace line 17 with the output of this script; */
 /* syscall:::entry
 /pid == $target
  && (###SYSCALL_FILTER###)
  /
-{	
+{
 	printf("\t\tDetected invalid syscall %s, terminating process %d...\r\n", probefunc, pid);
 	ustack();
 	stop();
 	printf("\t\tKILLING...\r\n");
 	system("\t\tkill -9 %d", pid);
 	printf("\t\tKILLED.\r\n");
 	exit(-1);
 } */
 
 
 /* Allowed syscalls probe */
 syscall:::entry
 /pid == $target/
-{	
+{
 	@calls[basename(execname), "syscall", probefunc] = count();
 	@syscalls[probefunc, "syscall"] = count();
 }
 
 dtrace:::END
 {
 	printf("\r\nsyscalls for %d:\r\n\r\n", $target);
@@ -44,10 +44,10 @@
 	printf("\r\nAll syscalls:\r\n");
 	printa("- %s\r\n", @syscalls);
 	printf("\r\n Generated syscalls (yaml profile):\r\n");
 	printf("    destructive: true\r\n    syscall_allowlist:\r\n");
 	printa("        - %s\r\n", @syscalls);
 	printf("\r\nAllowlist for you module:\r\n\r\n");
 	printa("probefunc != \"%s\" && ", @syscalls);
-	printf("\r\n\r\nGo to src/secimport/templates/default.allowlist.template.d and modify your probe.\r\n\r\n");
+	printf("\r\n\r\nGo to secimport/templates/default.allowlist.template.d and modify your probe.\r\n\r\n");
 	printf("\r\nDone.\r\n")
 }
```

### Comparing `secimport-0.6.4/src/secimport/backends/dtrace_backend/default.blocklist.template.d` & `secimport-0.7.0/secimport/backends/dtrace_backend/default.blocklist.template.d`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 /* Non-Allowed syscalls probe - Kills the process */
 /* Replace line 17 with the output of this script; */
 /* syscall:::entry
 /pid == $target
  && (###SYSCALL_FILTER###)
  /
-{	
+{
 	printf("\t\tDetected invalid syscall %s, terminating process %d...\r\n", probefunc, pid);
 	ustack();
 	stop();
 	printf("\t\tKILLING...\r\n");
 	system("\t\tkill -9 %d", pid);
 	printf("\t\tKILLED.\r\n");
 	exit(-1);
 } */
 
 /* Allowed syscalls probe */
 syscall:::entry
 /pid == $target/
-{	
+{
 	@calls[basename(execname), "syscall", probefunc] = count();
 	@syscalls[probefunc, "syscall"] = count();
 }
 
 dtrace:::END
 {
 	printf("\r\nsyscalls for %d:\r\n\r\n", $target);
@@ -35,8 +35,7 @@
 	printf("\r\nAll syscalls:\r\n");
 	printa("- %s\r\n", @syscalls);
 	printf("\r\n Generated syscalls (yaml profile):\r\n");
 	printf("    destructive: true\r\n    syscall_allowlist:\r\n");
 	printa("        - %s\r\n", @syscalls);
 	printf("\r\nDone.\r\n")
 }
-
```

### Comparing `secimport-0.6.4/src/secimport/backends/dtrace_backend/default.template.d` & `secimport-0.7.0/secimport/backends/dtrace_backend/default.template.d`

 * *Files 1% similar despite different names*

```diff
@@ -37,34 +37,34 @@
 	/* Saving the stack depth for each module, assuming interpreter with GIL will run line-by-line. */
 	if (depth_matrix[current_module_str] > self->depth){
 		depth_matrix["###MODULE_NAME###"] = 0;
 	}
 	if (depth_matrix[current_module_str] == 0){
 		depth_matrix[current_module_str] = self->depth;
 	}
-	
+
 	###FUNCTION_ENTRY###
 	self->last = timestamp;
 }
 
 python*:::function-return
-{	
-	
+{
+
 	this->delta = (timestamp - self->last) / 1000;
 	self->depth -= self->depth > 0 ? 1 : 0;
 	if (depth_matrix["###MODULE_NAME###"] > self->depth){
 		depth_matrix["###MODULE_NAME###"] = 0;
 	}
 	###FUNCTION_EXIT###
 	self->last = timestamp;
 }
 
 syscall:::entry
 /pid == $target/
-{	
+{
 	@calls[basename(execname), "syscall", probefunc] = count();
 	###SYSCALL_ENTRY###
 }
 
 dtrace:::END
 {
 	printf("System Calls (%d):\r\n\r\n", $target);
```

### Comparing `secimport-0.6.4/src/secimport/backends/dtrace_backend/default.yaml.template.d` & `secimport-0.7.0/secimport/backends/dtrace_backend/default.yaml.template.d`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     10 Hz -> ~15k
     20 Hz -> ~10k
     30 Hz -> ~2k
     40 Hz -> ~1k
     50 Hz (max) -> < 200
 */
 
-#pragma D option dynvarsize=400000     
+#pragma D option dynvarsize=400000
 /*
      10,000 @ 50 Hz -> ~25k+
-    100,000 @ 50 Hz -> ~20k  
+    100,000 @ 50 Hz -> ~20k
     200,000 @ 50 Hz -> ~3k
     300,000 @ 50 Hz -> ~1k
     400,000 @ 50 Hz -> 0
     400,000 @ 25 Hz -> ~2k
     500,000 @ 25 Hz -> ~1k
 */
 
@@ -51,24 +51,24 @@
 	this->delta = (timestamp - self->last) / 1000;
 	self->depth++;
 
 	/* Memoizing the previous module and current module */
 	_current_module_str = stringof(copyinstr(arg0));
 	previous_module_str = stringof(current_module_str);
 	current_module_str =  _current_module_str;
-	
+
 	/* if (strstr(_current_module_str, "###MODULE_NAME###") != 0){
 		printf("---! in module %s \r\n", "###MODULE_NAME###");
 	} */
 
 	/* Saving the stack depth for each module, assuming interpreter with GIL will run line-by-line. */
 	if (depth_matrix[current_module_str] > self->depth){
 		depth_matrix[current_module_str] = 0;
 	}
-	if (depth_matrix[current_module_str] == 0){ 
+	if (depth_matrix[current_module_str] == 0){
 		/* printf("---> (%d) %s\r\n", self->depth,  _current_module_str); */
 		depth_matrix[current_module_str] = self->depth;
 	}
 	/* depth_matrix[current_module_str] = self->depth; */
 }
 
 python*:::function-return
@@ -85,18 +85,18 @@
 /pid == $target/
 {
 	@calls[basename(execname), "syscall", probefunc] = count();
 	/* printf("\n@%s", probefunc); */
 	###SUPERVISED_MODULES_PROBES###
 }
 
-/* 
+/*
 syscall:::return
 /pid == $target/
-{	
+{
 	printf("\n");
 } */
 
 
 dtrace:::END
 {
 	printf("System Calls (%d)\r\n\r\n", $target);
```

### Comparing `secimport-0.6.4/src/secimport/backends/dtrace_backend/generate_profile.d` & `secimport-0.7.0/secimport/backends/dtrace_backend/generate_profile.d`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/sbin/dtrace -Zs
 /*
 	This script generates a list of syscalls for a given program.
 	It generates a filter for dscript.
 	The first probe can be replaced with the output of the following usage.
 
-	USAGE:	sudo dtrace -s src/secimport/templates/generate_profile.d -c "python -m http.server" # then CTRL+C
+	USAGE:	sudo dtrace -s secimport/templates/generate_profile.d -c "python -m http.server" # then CTRL+C
 */
 
 #pragma D option quiet
 #pragma D option switchrate=1
 
 /* Trace syscalls probe */
 syscall:::entry
 /pid == $target/
-{	
+{
 	@calls[basename(execname), "syscall", probefunc] = count();
 	@syscalls[probefunc, "syscall"] = count();
 }
 
 dtrace:::END
 {
 	printf("\r\nsyscalls for %d:\r\n\r\n", $target);
```

### Comparing `secimport-0.6.4/src/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d` & `secimport-0.7.0/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 if ((depth_matrix["###MODULE_NAME###"] != 0) && (self->depth >= depth_matrix["###MODULE_NAME###"])){
 	    if (latest_supervised_module == ""){
 			latest_supervised_module = "###MODULE_NAME###"
 		}
 		else{
 			if (depth_matrix["###MODULE_NAME###"] > depth_matrix[latest_supervised_module]){
 				latest_supervised_module = "###MODULE_NAME###"
-			}	
+			}
 		}
-		
+
 /* printf("GOT %s %s %d", _current_module_str,  dirname("###MODULE_NAME###"), strstr(_current_module_str,  dirname("###MODULE_NAME###")) */
 		if (depth_matrix["###MODULE_NAME###"] == depth_matrix[latest_supervised_module])
 		{
 			if (###SYSCALL_FILTER###){
 				printf("\n*SUPERVISED FLOW: syscall '%s' called in '%s' from '%s'; which entered at depth %d;\nThe supervised module is %s which entered the stack in depth %d;\r\n", probefunc, _current_module_str, "###MODULE_NAME###", depth_matrix["###MODULE_NAME###"],  latest_supervised_module, depth_matrix[latest_supervised_module]);
 				###SUPERVISED_MODULES_FILTER###
 				###SUPERVISED_MODULES_ACTION###
 			}
 		}
 }
-/* ###MODULE_NAME### END */
+/* ###MODULE_NAME### END */
```

### Comparing `secimport-0.6.4/src/secimport/backends/dtrace_backend/py_sandbox.d` & `secimport-0.7.0/secimport/backends/dtrace_backend/py_sandbox.d`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/sbin/dtrace -Zs
 
 /*
-Examples based on: 
+Examples based on:
 	https://docs.oracle.com/cd/E18752_01/html/819-5488/gcfpz.html
 	https://opensource.apple.com/source/dtrace/dtrace-147/DTTk/dtruss.auto.html
 	https://www.brendangregg.com/Articles/FreeBSDwiki_DTrace_Tutorial_2014.pdf
 	https://docs.oracle.com/en/operating-systems/solaris/oracle-solaris/11.4/dtrace-guide/arrays-dtrace.html
 */
 
 #pragma D option destructive
@@ -15,15 +15,15 @@
 /* A depth matrix for modules by name, maps each module (string) to the stack depth (int) at which it entered. */
 int depth_matrix[string];
 self int depth;
 self int sandbox_module_reached;
 
 string current_module_str;
 string previous_module_str;
-/* 
+/*
 inline string RED       = "33[31;1m";
 inline string BLUE      = "33[34;1m";
 inline string GREEN     = "33[32;1m";
 inline string VIOLET    = "33[35;1m";
 inline string OFF       = "33[0m";
 */
 
@@ -50,37 +50,37 @@
 	current_module_str =  _current_module_str;
 
 	/* Saving the stack depth for each module, assuming interpreter with GIL will run line-by-line. */
 	if (depth_matrix[current_module_str] == 0){
 		depth_matrix[current_module_str] = self->depth;
 	}
 
-	printf("\r\n%d %6d %10d  %16s:%-4d %-8s %*s-> %s", cpu, pid, this->delta, 
+	printf("\r\n%d %6d %10d  %16s:%-4d %-8s %*s-> %s", cpu, pid, this->delta,
 	    current_module_str, arg2, "func", self->depth * 4, "",
 	    copyinstr(arg1));
 	self->depth++;
 	self->last = timestamp;
 }
 
 python*:::function-return
-{	
+{
 	this->delta = (timestamp - self->last) / 1000;
 	self->depth -= self->depth > 0 ? 1 : 0;
-	printf("\r\n%d %6d %10d  %16s:%-4d %-8s %*s<- %s", cpu, pid, this->delta, 
+	printf("\r\n%d %6d %10d  %16s:%-4d %-8s %*s<- %s", cpu, pid, this->delta,
 	    current_module_str, arg2, "func", self->depth * 4, "",
 	    copyinstr(arg1));
 	if (depth_matrix[current_module_str] >= self->depth){
 		depth_matrix[current_module_str] = 0;
 	}
 	self->last = timestamp;
 }
 
 syscall:::entry
 /pid == $target/
-{	
+{
 	printf("\t%*s#%s",self->depth * 4, "",probefunc);
 	@calls[basename(execname), "syscall", probefunc] = count();
 	if (probefunc == "open"){
 		printf("(OPENING FILE): %s from thread %d in python module %s\r\n", probefunc, tid, current_module_str);
 	}
 	if (probefunc == "write"){
 		printf("(TOUCHING FILESYSTEM): %s(%d) from thread %d in python module %s\r\n", probefunc, arg1, tid, current_module_str);
@@ -103,22 +103,22 @@
 	}
 	if (probefunc == "posix_spawnp" ||
 		probefunc == "clone" ||
 		probefunc == "__clone2" ||
 		probefunc == "clone3" ||
 		probefunc == "fork" ||
 		probefunc == "vfork" ||
-		probefunc == "forkexec" || 
-		probefunc == "execl" || 
-		probefunc == "execlp" || 
-		probefunc == "execle" || 
-		probefunc == "execv" || 
+		probefunc == "forkexec" ||
+		probefunc == "execl" ||
+		probefunc == "execlp" ||
+		probefunc == "execle" ||
+		probefunc == "execv" ||
 		probefunc == "execvp")
-			{ 
-				/* printf("\t\t(ALLOWING SHELL using %s):%60s %16s %20d\r\n", probefunc, copyinstr(arg0), copyinstr(arg1), arg2); */ 
+			{
+				/* printf("\t\t(ALLOWING SHELL using %s):%60s %16s %20d\r\n", probefunc, copyinstr(arg0), copyinstr(arg1), arg2); */
 				if(depth_matrix["malicious.py"] != 0 && self->depth >= depth_matrix["malicious.py"]){
 					printf("\t\TERMINATING shell...\r\n");
 					ustack();
 					stop();
 					printf("\t\tkilling...\r\n");
 					system("\t\tkill -9 %d", pid);
 					printf("\t\tkilled.\r\n");
```

### Comparing `secimport-0.6.4/src/secimport/profiles/trace.bt` & `secimport-0.7.0/secimport/backends/bpftrace_backend/default.yaml.template.bt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 #!/usr/bin/env bpftrace
 
-// A profiling script that logs all the syscalls, per python module.
-// It can be attached to a running process using -p or can be used to trace a python shell interactively.
-// 
-// Usage:
-// ./trace.bt -c Python-3.10.0/python
-
 BEGIN {
     // Mapping all syscalls both ways, based on https://github.com/iovisor/bpftrace/blob/2c7a7a598dbe1aa790db2dfe2db242aa69137d5b/tools/syscount.bt
     // Generates using bash:
     //   $ apt-get install auditd
     //   $ ausyscall --dump | awk 'NR > 1 { printf("\t@sysname[%d] = \"%s\";\n", $1, $2); }';
     printf("REGISTERING SYSCALLS...\n");
     @sysname[0] = "read";
@@ -681,46 +675,75 @@
 	@sysnum["pwritev2"] = 328;
 	@sysnum["pkey_mprotect"] = 329;
 	@sysnum["pkey_alloc"] = 330;
 	@sysnum["pkey_free"] = 331;
 	@sysnum["statx"] = 332;
 	@sysnum["io_pgetevents"] = 333;
 	@sysnum["rseq"] = 334;
-    printf("Tracing Modules - Exit gracefully with Ctrl+D\n")
+
+    ###SYSCALL_FILTER###
+    printf("STARTED\n");
 }
 
-usdt:/workspace/Python-3.10.0/python:function__entry {
+
+usdt:###INTERPRETER_PATH###:function__entry {
         @["depth"]++;
         @entrypoints[str(arg0)] = @["depth"];
         @globals["previous_module"] = @globals["current_module"];
         @globals["current_module"] = str(arg0);
-
-        // To trace python calls in the console, uncomment:
-        // printf("%s, %s, depth=%d\n", str(arg0), str(arg1), @["depth"]) ;
+        @latest_supervised_module =  str(arg0);
+        // printf("%s, %s, depth=%d\n", str(arg0), str(arg1), @["depth"]);
 }
 
-usdt:/workspace/Python-3.10.0/python:function__return {
-        @["depth"]--;
+usdt:###INTERPRETER_PATH###:function__return {
+    @["depth"]--;
 }
 
 tracepoint:raw_syscalls:sys_enter /comm == "python"/ {
-    // @modules_syscalls[@globals["current_module"], @sysname[args->id], @["depth"]] = count();
-    @modules_syscalls[@globals["current_module"], @sysname[args->id]] = count();
-    @syscalls[@sysname[args->id]] = count();
+    // Allowing global requirements ("general requirements") to be used by all syscalls.
+    if (@syscalls_filters["general_requirements", @sysname[args->id]] != 1){
+        // Logging every syscall that was not confirmed by the user at compile time.
+        if (@syscalls_filters[@latest_supervised_module, @sysname[args->id]] != 1){
+            printf("\033[91m[SECURITY PROFILE VIOLATED]: %s called syscall %s at depth %d\033[0m\r\n", @latest_supervised_module, @sysname[args->id], @["depth"]);
+
+            if (str($1) == "STOP") {
+                printf("\n^^^ STOPPING PROCESS %d DUE TO SYSCALL VIOLATION ^^^\n", pid);
+                signal("SIGSTOP");
+                printf("\t\tPROCESS %d STOPPED.\r\n", pid);
+            }
+
+            if (str($1) == "KILL") {
+                printf("\n^^^ KILLING PROCESS %d DUE TO SYSCALL VIOLATION ^^^\n", pid);
+                signal("SIGKILL");
+                // system("pkill -9 python"); // optional. Please use "bpftrace --unsafe" or remove this line.
+                printf("\t\tKILLED.\r\n");
+                exit(); // optional
+            }
+        }
+    }
 }
 
 
+// Invoked before importlib imports a module
+// import__find__load__start(str modulename)
+// usdt:###INTERPRETER_PATH###:import__find__load__start {
+    // TODO: verify that the module is allowed in the syscall filter.
+    // @imports[arg0] = count();
+    // printf("importing %d", arg0);
+// }
+
+// Invoked after importlib imports a module
+// import__find__load__done(str modulename, int found)
+// usdt:###INTERPRETER_PATH###:import__find__load__done{
+    // printf("imported %d", arg0);
+// }
+
+
 END {
-    printf("Summary:");
-	printf(" %-32s %-10s %-22s %8s\r\n", "FILE", "TYPE", "NAME", "COUNT");
-	printf("\r\nAll syscalls (count):\r\n");
-	print(@syscalls);
-    printf("\r\nSyscalls Per Python Module:\r\n");
-    print(@modules_syscalls);
-	printf("\r\nDone.\r\n");
     clear(@sysname);
     clear(@sysnum);
-    clear(@syscalls);
-    clear(@modules_syscalls);
     clear(@entrypoints);
-    clear(@globals)
-}
+    clear(@syscalls_filters);
+    clear(@globals);
+    clear(@latest_supervised_module);
+    clear(@);
+}
```

### Comparing `secimport-0.6.4/src/secimport/sandbox_helper.py` & `secimport-0.7.0/secimport/sandbox_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Import python modules with syscalls supervision.
 
 Copyright (c) 2022 Avi Lumelsky
 """
 
-from typing import List
 from secimport.backends.common.instrumentation_backend import InstrumentationBackend
 from secimport.backends.common.utils import DEFAULT_BACKEND
 from secimport.backends.bpftrace_backend.bpftrace_backend import (
     run_bpftrace_script_for_module,
 )
 from secimport.backends.dtrace_backend.dtrace_backend import (
     run_dtrace_script_for_module,
@@ -21,31 +20,28 @@
     allow_networking: bool = False,
     use_sudo: bool = False,
     log_python_calls: bool = False,  # When True, the log file might reach GB in seconds.
     log_syscalls: bool = False,
     log_network: bool = False,
     log_file_system: bool = False,
     destructive: bool = True,
-    syscalls_allowlist: List[str] = None,
-    syscalls_blocklist: List[str] = None,
     backend=DEFAULT_BACKEND,
+    **kwargs,
 ):
     """Import a python module in confined settings.
 
     Args:
         module_name (str): The name of the module to import. The same way you would have used an 'import' statement.
         allow_shells (bool, optional): Whether to allow forking/spwning shells and execute commands.
         allow_networking (bool, optional): Whether to allow socket syscalls.
         use_sudo (bool, optional): Whether to run dtrace with sudo. Can be turned off if sudo is not installed.
         log_python_calls (bool, optional): Whether to log the call tree of the python stack - function entry and exit events.
         log_network (bool, optional): Whether to log network successful connections - e.g socket syscalls.
         log_file_system (bool, optional): Whether to log filesystem calls - e.g read, open, write, etc.
         destructive (bool, optional): Whether to kill the process with -9 sigkill upon violation of any of the configurations above.
-        syscalls_allowlist (list, optional): A list of allowed syscalls for the module. Any other syscall will result in destructive behavior (see description above).
-        syscalls_blocklist (list, optional): A list of syscalls to block for the module. Any of the specified syscalls under this module will result in destructive behavior (see description above).
     Returns:
         _type_: A Python Module. The module is supervised by a dtrace process with destructive capabilities unless the 'destructive' argument is set to False.
     """
 
     if backend == InstrumentationBackend.EBPF:
         assert run_bpftrace_script_for_module(
             module_name=module_name,
@@ -53,29 +49,25 @@
             allow_networking=allow_networking,
             use_sudo=use_sudo,
             log_python_calls=log_python_calls,
             log_syscalls=log_syscalls,
             log_network=log_network,
             log_file_system=log_file_system,
             destructive=destructive,
-            syscalls_allowlist=syscalls_allowlist,
-            syscalls_blocklist=syscalls_blocklist,
         )
     elif backend == InstrumentationBackend.DTRACE:
         assert run_dtrace_script_for_module(
             module_name=module_name,
             allow_shells=allow_shells,
             allow_networking=allow_networking,
             use_sudo=use_sudo,
             log_python_calls=log_python_calls,
             log_syscalls=log_syscalls,
             log_network=log_network,
             log_file_system=log_file_system,
             destructive=destructive,
-            syscalls_allowlist=syscalls_allowlist,
-            syscalls_blocklist=syscalls_blocklist,
         )
     else:
         raise NotImplementedError(f"backend '{backend}' is not implemented.")
 
-    _module = __import__(module_name)
+    _module = __import__(module_name, **kwargs)
     return _module
```

