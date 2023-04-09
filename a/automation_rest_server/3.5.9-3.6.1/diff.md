# Comparing `tmp/automation_rest_server-3.5.9.tar.gz` & `tmp/automation_rest_server-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\automation_rest_server-3.5.9.tar", last modified: Fri Mar  3 03:42:31 2023, max compression
+gzip compressed data, was "dist\automation_rest_server-3.6.1.tar", last modified: Sun Apr  9 03:04:17 2023, max compression
```

## Comparing `automation_rest_server-3.5.9.tar` & `automation_rest_server-3.6.1.tar`

### file list

```diff
@@ -1,154 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/
--rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0      551 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/configuration/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/configuration/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/configuration/config.yaml
--rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.5.9/automation_rest_server/configuration/firmware_build.yaml
--rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/configuration/pci.ids
--rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/configuration/version.yaml
--rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.5.9/automation_rest_server/configuration/web_server.yaml
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/
--rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/models/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/models/__init__.py
--rw-rw-rw-   0        0        0     4264 2022-08-12 01:44:10.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/models/helper.py
--rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/node_resource.py
--rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/test_resource.py
--rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/web_resource.py
--rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.5.9/automation_rest_server/rest_client/web_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/__init__.py
--rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/reset_server.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/__init__.py
--rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/benchmark_resource.py
--rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/build_firmware_resource.py
--rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/git_resource.py
--rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/models/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/models/__init__.py
--rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/models/ftp_server.py
--rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/models/helper.py
--rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/oakgate_resource.py
--rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/operation_resource.py
--rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/state_resource.py
--rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/stop_flag_resource.py
--rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/test_resource.py
--rw-rw-rw-   0        0        0     1244 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/upgrade_resource.py
--rw-rw-rw-   0        0        0     5946 2023-03-03 03:40:52.000000 automation_rest_server-3.5.9/automation_rest_server/run.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/__init__.py
--rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/database.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/
--rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/__init__.py
--rw-rw-rw-   0        0        0     3039 2022-09-15 07:43:45.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/slot.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/
--rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/__init__.py
--rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
--rw-rw-rw-   0        0        0     3383 2022-12-14 01:26:41.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
--rw-rw-rw-   0        0        0      608 2023-02-28 09:02:51.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
--rw-rw-rw-   0        0        0     8892 2022-09-27 01:01:15.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/
--rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/__init__.py
--rw-rw-rw-   0        0        0     2067 2022-12-13 09:26:23.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/nose_engine.py
--rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/oakgate_engine.py
--rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/perses_engine.py
--rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
--rw-rw-rw-   0        0        0     8717 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/perses_power_cycle_engine_old.py
--rw-rw-rw-   0        0        0     4174 2022-09-20 05:33:53.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/special_parameter.py
--rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/sse_engine.py
--rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_build.py
--rw-rw-rw-   0        0        0     2724 2022-12-14 00:39:53.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_download.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/__init__.py
--rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
--rw-rw-rw-   0        0        0     2892 2022-12-14 01:11:11.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
--rw-rw-rw-   0        0        0     1637 2022-09-27 01:01:15.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
--rw-rw-rw-   0        0        0     1581 2022-09-27 01:01:15.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
--rw-rw-rw-   0        0        0     4180 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
--rw-rw-rw-   0        0        0     5467 2022-08-12 02:31:49.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/node_database.py
--rw-rw-rw-   0        0        0    10709 2023-03-01 01:30:29.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/performance_database.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/reboot_engine/
--rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/reboot_engine/__init__.py
--rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
--rw-rw-rw-   0        0        0     1946 2022-08-15 02:37:21.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/state.py
--rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/status_file.py
--rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_base.py
--rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_benchmark.py
--rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_benchmark_group.py
--rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_case.py
--rw-rw-rw-   0        0        0    21775 2022-12-03 07:40:32.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_pool.py
--rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_reboot_handle.py
--rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_result.py
--rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_runner.py
--rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/test_framework/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/
--rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/dll/
--rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/dll/__init__.py
--rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/dll/buf.dll
--rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/dll/buf.so
--rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/dll/build.py
--rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/linux_nvme.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/
--rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/__init__.py
--rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/buf.py
--rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/ctype.py
--rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/get_feature.py
--rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/ioctl.py
--rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/nvme.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/
--rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/__init__.py
--rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/command.py
--rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/features.py
--rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/hmb.py
--rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/identify.py
--rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/log_page.py
--rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/memory.py
--rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/pcie.py
--rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/registers.py
--rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/utility_vu.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/diskpart/
--rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/diskpart/__init__.py
--rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/diskpart/diskpart.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/fio/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/fio/__init__.py
--rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/fio/fio.py
--rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/fio/fio_linux.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/fio/tool/
--rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/fio/tool/fio
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/git/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/git/__init__.py
--rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.5.9/automation_rest_server/tool/git/git_operator.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/tool/iometer/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/tool/iometer/__init__.py
--rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.5.9/automation_rest_server/tool/iometer/iometer.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server/utils/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/utils/__init__.py
--rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/utils/buf.py
--rw-rw-rw-   0        0        0     5716 2022-11-15 03:39:09.000000 automation_rest_server-3.5.9/automation_rest_server/utils/firmware_path.py
--rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/utils/log.py
--rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.5.9/automation_rest_server/utils/message.py
--rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/utils/nose_xml.py
--rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.5.9/automation_rest_server/utils/pip_operation.py
--rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/utils/process.py
--rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.5.9/automation_rest_server/utils/ssh.py
--rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.5.9/automation_rest_server/utils/system.py
-drwxrwxrwx   0        0        0        0 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server.egg-info/
--rw-rw-rw-   0        0        0      551 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6700 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/automation_rest_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-03-03 03:42:31.000000 automation_rest_server-3.5.9/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-03-03 03:42:23.000000 automation_rest_server-3.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/
+-rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      551 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:16.000000 automation_rest_server-3.6.1/automation_rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/configuration/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/configuration/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/configuration/config.yaml
+-rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.1/automation_rest_server/configuration/firmware_build.yaml
+-rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/configuration/pci.ids
+-rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/configuration/version.yaml
+-rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.1/automation_rest_server/configuration/web_server.yaml
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/
+-rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     4264 2022-08-12 01:44:10.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/models/helper.py
+-rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/node_resource.py
+-rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/test_resource.py
+-rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/web_resource.py
+-rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.1/automation_rest_server/rest_client/web_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/__init__.py
+-rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/reset_server.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/__init__.py
+-rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/benchmark_resource.py
+-rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/build_firmware_resource.py
+-rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/git_resource.py
+-rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/models/ftp_server.py
+-rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/models/helper.py
+-rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/oakgate_resource.py
+-rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/operation_resource.py
+-rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/state_resource.py
+-rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/stop_flag_resource.py
+-rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/test_resource.py
+-rw-rw-rw-   0        0        0     1244 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/upgrade_resource.py
+-rw-rw-rw-   0        0        0     5980 2023-03-06 02:10:37.000000 automation_rest_server-3.6.1/automation_rest_server/run.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/__init__.py
+-rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/database.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/
+-rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/__init__.py
+-rw-rw-rw-   0        0        0     3039 2022-09-15 07:43:45.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/slot.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/
+-rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/__init__.py
+-rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
+-rw-rw-rw-   0        0        0     3383 2022-12-14 01:26:41.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
+-rw-rw-rw-   0        0        0      608 2023-02-28 09:02:51.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
+-rw-rw-rw-   0        0        0     8892 2022-09-27 01:01:15.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/
+-rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/__init__.py
+-rw-rw-rw-   0        0        0     2067 2022-12-13 09:26:23.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/nose_engine.py
+-rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/oakgate_engine.py
+-rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/perses_engine.py
+-rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/special_parameter.py
+-rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/sse_engine.py
+-rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_build.py
+-rw-rw-rw-   0        0        0     2724 2022-12-14 00:39:53.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_download.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/__init__.py
+-rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
+-rw-rw-rw-   0        0        0     3909 2023-04-07 02:24:48.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
+-rw-rw-rw-   0        0        0     1987 2023-04-09 02:31:46.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
+-rw-rw-rw-   0        0        0     1581 2022-09-27 01:01:15.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
+-rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
+-rw-rw-rw-   0        0        0     5467 2022-08-12 02:31:49.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/node_database.py
+-rw-rw-rw-   0        0        0    10711 2023-03-31 07:34:14.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/performance_database.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/reboot_engine/
+-rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/reboot_engine/__init__.py
+-rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
+-rw-rw-rw-   0        0        0     2052 2023-04-04 09:26:41.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/state.py
+-rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/status_file.py
+-rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_base.py
+-rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_benchmark.py
+-rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_benchmark_group.py
+-rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_case.py
+-rw-rw-rw-   0        0        0    21722 2023-04-04 09:26:41.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_pool.py
+-rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_reboot_handle.py
+-rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_result.py
+-rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_runner.py
+-rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/test_framework/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/
+-rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/dll/
+-rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/dll/__init__.py
+-rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/dll/buf.dll
+-rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/dll/buf.so
+-rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/dll/build.py
+-rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/linux_nvme.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/
+-rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/__init__.py
+-rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/buf.py
+-rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/ctype.py
+-rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/get_feature.py
+-rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/ioctl.py
+-rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/nvme.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/
+-rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/__init__.py
+-rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/command.py
+-rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/features.py
+-rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/hmb.py
+-rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/identify.py
+-rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/log_page.py
+-rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/memory.py
+-rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/pcie.py
+-rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/registers.py
+-rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/utility_vu.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/diskpart/
+-rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/diskpart/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/diskpart/diskpart.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/fio/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/fio/__init__.py
+-rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/fio/fio.py
+-rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/fio/fio_linux.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/fio/tool/
+-rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/fio/tool/fio
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/git/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/git/__init__.py
+-rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.1/automation_rest_server/tool/git/git_operator.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/tool/iometer/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/tool/iometer/__init__.py
+-rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.1/automation_rest_server/tool/iometer/iometer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/automation_rest_server/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/utils/__init__.py
+-rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/utils/buf.py
+-rw-rw-rw-   0        0        0     5547 2023-04-07 03:23:26.000000 automation_rest_server-3.6.1/automation_rest_server/utils/firmware_path.py
+-rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/utils/log.py
+-rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.1/automation_rest_server/utils/message.py
+-rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/utils/nose_xml.py
+-rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.1/automation_rest_server/utils/pip_operation.py
+-rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/utils/process.py
+-rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.1/automation_rest_server/utils/ssh.py
+-rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.1/automation_rest_server/utils/system.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:16.000000 automation_rest_server-3.6.1/automation_rest_server.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-04-09 03:04:16.000000 automation_rest_server-3.6.1/automation_rest_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6622 2023-04-09 03:04:16.000000 automation_rest_server-3.6.1/automation_rest_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 03:04:16.000000 automation_rest_server-3.6.1/automation_rest_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-09 03:04:16.000000 automation_rest_server-3.6.1/automation_rest_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-04-09 03:04:16.000000 automation_rest_server-3.6.1/automation_rest_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-09 03:04:16.000000 automation_rest_server-3.6.1/automation_rest_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-04-09 03:04:17.000000 automation_rest_server-3.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-04-09 03:02:42.000000 automation_rest_server-3.6.1/setup.py
```

### Comparing `automation_rest_server-3.5.9/LICENSE.txt` & `automation_rest_server-3.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/MANIFEST.in` & `automation_rest_server-3.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/PKG-INFO` & `automation_rest_server-3.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation_rest_server
-Version: 3.5.9
+Version: 3.6.1
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/configuration/config.yaml` & `automation_rest_server-3.6.1/automation_rest_server/configuration/config.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/configuration/firmware_build.yaml` & `automation_rest_server-3.6.1/automation_rest_server/configuration/firmware_build.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/configuration/pci.ids` & `automation_rest_server-3.6.1/automation_rest_server/configuration/pci.ids`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/models/helper.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/node_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/node_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_client/resource/test_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_client/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_client/web_rest_client.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_client/web_rest_client.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/reset_server.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/reset_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/benchmark_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/build_firmware_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/build_firmware_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/git_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/git_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/models/ftp_server.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/models/ftp_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/models/helper.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/oakgate_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/oakgate_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/operation_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/operation_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/state_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/state_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/stop_flag_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/stop_flag_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/test_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/rest_server/resource/upgrade_resource.py` & `automation_rest_server-3.6.1/automation_rest_server/rest_server/resource/upgrade_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/run.py` & `automation_rest_server-3.6.1/automation_rest_server/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import sys
 import re
 import yaml
 import argparse
 import signal
 import platform
 if "-s" not in sys.argv:
-    print("Start to upgrade prun")
-    ret_code = os.system("pip3 install -U automation_rest_server -i https://pypi.org/project")
+    cmd_line = "pip3 install -U automation_rest_server -i https://pypi.org/project"
+    print(f"Start to upgrade prun{cmd_line}")
+    ret_code = os.system(cmd_line)
     print(f"upgrade result {ret_code}")
-
 sys.path.append(os.path.join(os.path.dirname(__file__)))
 from test_framework.test_pool import TestPool
 from test_framework.test_suite import TestSuite
 from test_framework.test_case import TestCase
 from rest_server.reset_server import *
 from rest_server.resource.models.ftp_server import thread_start_ftp_server
 from test_framework.database import update_abnormal_end_tests
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/database.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/slot.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/nose_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/nose_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/oakgate_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/oakgate_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/perses_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/perses_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/perses_power_cycle_engine_old.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,205 +1,173 @@
 import os
 import re
+import yaml
+import shutil
 import time
-import checksumdir
-from nose.tools import assert_equal
-from utils.ssh import SSH
+from tool.git.git_operator import GitOperator
 from utils import log
-from utils.message import Message
-from test_framework.test_base import TestBase
-from test_framework.state import State
+from utils.system import execute, get_time_stamp
 
 
-class PowerCycleEngine(TestBase):
+class FirmwareBuildEngine(object):
 
     def __init__(self):
-        super(PowerCycleEngine, self).__init__()
+        self.commit = ""
+        self.root_path = None
+        self.remote_path = None
+        self.build_paras = None
+        self.log_path = None
+
+    def get_log_path(self):
+        log_path = os.path.join(self.root_path, "log")
+        if os.path.exists(log_path) is False:
+            os.mkdir(log_path)
+        return log_path
+
+    def save_msg(self, msg):
+        log_file = "Build_fw_{}_{}.log".format(self.commit, time.time())
+        log_path = os.path.join(self.log_path, log_file)
+        with open(log_path, "w", encoding='utf-8') as file_:
+            file_.write(msg)
+        return log_path
+
+    def get_public_paras(self, project):
+        ret = False
+        git_config = os.path.join(os.path.dirname(__file__), "..", "..", "configuration", "firmware_build.yaml")
+        with open(git_config, "r", encoding='utf-8') as f_:
+            cont = f_.read()
+            configs = yaml.load(cont)
+            if project in configs.keys():
+                self.root_path = configs["root_path"]
+                self.remote_path = os.path.join(configs["remote_firmware"], project, "nightly")
+                self.build_paras = configs[project]
+                ret = True
+        return ret
+
+    def check_root_path(self):
+        if os.path.exists(self.root_path) is False:
+            os.makedirs(self.root_path)
+
+    def precondition(self, project):
+        ret = self.get_public_paras(project)
+        if ret is True:
+            self.check_root_path()
+            self.log_path = self.get_log_path()
+        return ret
+
+    def run(self, para):
+        print("build parameter", para)
+        if self.precondition(para["project"]):
+            ret, update_msg = self.update_code(para["rep_user"], para["rep_password"], para["rep_url"], para["rep_branch"])
+            if ret == 0:
+                commit_path = self.is_commit_exist()
+                if commit_path is None:
+                    ret, fw_bin_path, build_msg = self.build_firmware()
+                else:
+                    ret, fw_bin_path, build_msg = 0, commit_path, "Find exist commit path"
+            else:
+                fw_bin_path, build_msg = "",  "Update code failed, skip build firmware"
+            log_path = self.save_msg("{}\n{}".format(update_msg.message, build_msg))
+        else:
+            log_path = self.save_msg("Not found Project build config: {}".format(para["project"]))
+            ret, fw_bin_path = -1, ""
+        return ret, fw_bin_path, log_path, self.commit
+
+    def is_commit_exist(self):
+        if self.remote_path is not None and self.commit != "":
+            for item in os.listdir(self.remote_path):
+                if self.commit in item:
+                    find_build_path = os.path.join(self.remote_path, item)
+                    if self.is_folder_empty(find_build_path) is False:
+                        log.INFO("Find exist commit folder {} in {}".format(item, self.remote_path))
+                        return find_build_path
+                    else:
+                        shutil.rmtree(find_build_path)
+                        log.INFO("Remove emtpy build path: {}".format(find_build_path))
+        return None
+
+    @staticmethod
+    def is_folder_empty(remote_path):
+        dirs = os.listdir(remote_path)
+        result = False if dirs else True
+        return result
+
+    def build_firmware(self):
+        ret = None
+        msg = ""
+        remote_path = os.path.join(self.remote_path, "{}_{}".format(get_time_stamp(), self.commit))
+        if os.path.exists(remote_path) is False:
+            log.INFO("Create folder: {}".format(remote_path))
+            os.mkdir(remote_path)
+        for build in self.build_paras:
+            if build["output"] is not None:
+                output_path = os.path.join(self.root_path, build["output"])
+                self.clear_output(output_path, build["artifact"])
+            ret, output = self.execute_build_command(build["cmd"])
+            msg = "{}\n{}".format(msg, output)
+            log.INFO("{}, result: {}".format(build["cmd"], ret))
+            if ret == 0:
+                if build["output"] is not None:
+                    self.archiving_artifacts(build, remote_path)
+        return ret, remote_path, msg
+
+    def archiving_artifacts(self, build, remote_path):
+        log.INFO("archiving_artifacts")
+        if self.commit is not None:
+            for item in os.listdir(os.path.join(self.root_path, build["output"])):
+                if self.check_file_type(item, build["artifact"]):
+                    new_file_name = self.get_new_artifact_name(item, self.commit)
+                    scr_file = os.path.join(self.root_path, build["output"], item)
+                    dest_file = os.path.join(remote_path, new_file_name)
+                    log.INFO("Copy file: {} to {}".format(scr_file, dest_file))
+                    shutil.copyfile(scr_file, dest_file)
 
-    def initialization(self, parameters):
-        self.target_ip = os.environ["target_ip"]
-        self.user = os.environ.get('user', 'root')
-        self.password = os.environ.get('password', 'nvme')
-        self.adapter = os.environ.get('adapter', 'usbrelay')
-        self.fw_path = os.environ.get('fw_path', 'not_set')
-        self.commit = os.environ.get('commit', 'not_set')
-        self.ssh = SSH(self.target_ip, username=self.user, password=self.password)
-        self.ssh.open()
-        self.ssh.command("mount -a")
-        self.remote_env_path = self.get_remote_path()
-        self.remote_env_perses_path = "{}/{}".format(self.remote_env_path, "perses")
-        self.local_env_perses_path = os.environ["working_path"]
-        self.setup_target_environment()
-
-    def get_remote_path(self):
-        network_path = r"/home/share/sqa/powercycle"
-        if self.ssh.is_exist(network_path):
-            remote_path = r"/home/share/sqa/powercycle/{}".format(self.target_ip)
+    @staticmethod
+    def get_new_artifact_name(file_name, commit):
+        items = file_name.split(".")
+        if len(items) == 2:
+            new_name = "{}_{}.{}".format(items[0], commit, items[1])
         else:
-            remote_path = r"/home/powercycle"
-        return remote_path
+            new_name = file_name
+        return new_name
 
-    def remote_install(self, remote_path):
-        command = "cd {} && python install.py".format(remote_path)
-        status, output = self.ssh.command(command)
-        if status != 0:
-            print("remotes install failed")
-        print(output)
+    def execute_build_command(self, command_line):
+        cmd = "cd {} && {}".format(self.root_path, command_line)
+        status, output = execute(cmd, interrupt=False)
         return status, output
 
-    def dos2unit(self, remote_path):
-        paths = ["{}/tools/fio".format(remote_path),
-                 "{}/tools/vdbench504".format(remote_path),
-                 "{}/tools/usbrelay".format(remote_path)]
-        for item in paths:
-            command = "cd {} && dos2unix *".format(item)
-            status, output = self.ssh.command(command)
-            if status != 0:
-                print("dos2unit {} install failed".format(item))
-            print(output)
-
-    def chmod_files(self, remote_path):
-        paths = ["{}/tools/fio/fio".format(remote_path),
-                 "{}/tools/vdbench504/vdbench".format(remote_path),
-                 "{}/tools/usbrelay/usbrelay".format(remote_path)]
-        for item in paths:
-            command = "chmod 777 {}".format(item)
-            status, output = self.ssh.command(command)
-            if status != 0:
-                print("chmod  {}  failed".format(item))
-            print(output)
-
-    def upload_and_init_perses_2_target(self):
-        if self.ssh.is_exist(self.remote_env_path) is False:
-            self.ssh.make_dir(self.remote_env_path)
-        if self.ssh.is_exist(self.remote_env_perses_path) is False:
-            self.ssh.make_dir(self.remote_env_perses_path)
-        self.ssh.sftp_put_dir(self.local_env_perses_path, self.remote_env_perses_path)
-        self.remote_install(self.remote_env_perses_path)
-        self.dos2unit(self.remote_env_perses_path)
-        self.chmod_files(self.remote_env_perses_path)
-
-    def update_modified_perses_2_target(self):
-        compare_folder = ["configuration", "lib", "testcase", "testsuite", "testfile"]
-        for folder in compare_folder:
-            local_path = os.path.join(self.local_env_perses_path, folder)
-            remote_path = r"{}/{}".format(self.remote_env_perses_path, folder)
-            local_md5 = self.get_folder_md5(local_path)
-            remote_md5 = self.get_folder_md5_by_ssh(remote_path)
-            if local_md5 != remote_md5:
-                temp_path = "{}/{}".format(self.remote_env_perses_path, folder)
-                self.ssh.command("rm -r {}".format(temp_path))
-                self.ssh.make_dir(temp_path)
-                self.ssh.sftp_put_dir(local_path, temp_path)
-
-    def update_run_file(self):
-        local_path = os.path.join(self.local_env_perses_path, "run.py")
-        remote_path = r"{}/{}".format(self.remote_env_perses_path,  "run.py")
-        self.ssh.command("rm -r {}".format(remote_path))
-        self.ssh.sftp_put(local_path, remote_path)
-
-    def setup_target_environment(self):
-        ret = self.ssh.is_exist(self.remote_env_perses_path)
-        if ret is False:
-            self.upload_and_init_perses_2_target()
-        else:
-            self.update_modified_perses_2_target()
-            self.update_run_file()
+    def clear_output(self, path, file_types):
+        for item in os.listdir(path):
+            if os.path.isfile(os.path.join(path, item)):
+                if self.check_file_type(item, file_types) is True:
+                    os.remove(os.path.join(path, item))
+                    log.INFO("Firmware build delete file: {}".format(item))
 
     @staticmethod
-    def get_folder_md5(path):
-        md5hash = None
-        if os.path.exists(path):
-            md5hash = checksumdir.dirhash(path, 'md5', excluded_extensions=['pyc'])
-        return md5hash
-
-    def get_folder_md5_by_ssh(self, path):
-        md5 = None
-        cmd = "checksumdir -a md5 {}".format(path)
-        status, output = self.ssh.command(cmd)
-        if status == 0:
-            md5 = output.replace("\n", "")
-        return md5
-
-    def get_loop(self, test):
-        loop = 1
-        test_path = re.findall("(.*):", test)[0]
-        function_name = re.findall("\w*\:\w*\.(\w*)", test)
-        file_ = open(test_path)
-        content = file_.read()
-        loops = re.findall(".*attr\(loop\=(\d+)\).*\n\s+def\s+{}\(self\)".format(function_name[0]), content)
-        loop = loops[0]if loops else loop
-        return loop
-
-    def remote_run_test(self, test, loop=1, before_reboot=True):
-        before_reboot = "true" if before_reboot is True else "false"
-        parameter = "loop:{},before_reboot:{},adapter:{},fw_path:{},commit:{}".format(loop, before_reboot, self.adapter,
-                                                                                   self.fw_path, self.commit)
-        run_command = "cd {} && python run.py testcase -n {} -v {}".format(self.remote_env_perses_path, test, parameter)
-        status, output = self.ssh.command(run_command)
-        # log.INFO("Remote_run_test command: %s, status: %s, output:\n %s", run_command, status, output)
-        return status, output
+    def check_file_type(file_name, file_types):
+        for item in file_types:
+            if file_name.endswith(item) is True:
+                return True
+        return False
 
-    def reboot(self):
-        log.INFO("reboot......")
-        self.ssh.command_without_result("reboot -nf", timeout=10)
-        time.sleep(10)
-        self.ssh.close()
-
-    def wait_reboot_complete(self, time_out=600):
-        result = False
-        start_time = time.time()
-        current_time = start_time
-        duration = current_time - start_time
-        while duration < time_out:
-            log.INFO("try to connect target compute: time %s", duration)
-            try:
-                self.ssh.open(timeout=10)
-            except RuntimeError:
-                pass
-            if self.ssh.is_active():
-                self.ssh.command("mount -a")
-                log.INFO("reboot succeed")
-                result = True
-                break
-            duration = time.time() - start_time
-        return result
+    @staticmethod
+    def get_url_folder(url):
+        rets = re.findall("/(\w*)\.git", url)
+        if rets:
+            folder_name = rets[0]
+        else:
+            folder_name = ""
+        return folder_name
 
-    def save_log(self, out_put, test_case):
-        log_file = os.path.join(self.get_log_path(), "power_cycle_%s_%s.xml" % (test_case, time.time()))
-        file_ = open(os.path.join(log_file), "w")
-        file_.write(out_put)
-        file_.close()
-        return log_file
-
-    def run(self, test_case, test_path, parameters, queue):
-
-        print("Test parameters", parameters)
-        self.initialization(parameters)
-
-        loop = self.get_loop(test_path)
-        result = State.PASS
-        test_message = Message()
-        for index in range(int(loop)):
-            test_message.add_message("Run Power Cycle test: {}, loop: {}".format(test_case, index))
-            status, output1 = self.remote_run_test(test_case, loop=index, before_reboot=True)
-            test_message.add_message(output1)
-            if status != 0:
-                result = State.FAIL
-                break
-            self.reboot()
-            reboot_result = self.wait_reboot_complete()
-            if reboot_result is False:
-                test_message.add_message("Reboot failed at loop {}".format(index))
-                result = State.FAIL
-                break
-            else:
-                test_message.add_message("Reboot succeed at loop {}".format(index))
-            status, output2 = self.remote_run_test(test_case, loop=index, before_reboot=False)
-            test_message.add_message(output2)
-            if status != 0:
-                result = State.FAIL
-                break
-        log_path = self.save_log(test_message.message, test_case)
-        result = {"name": test_case, "result": result, "log": log_path}
-        queue.put(result)
-        return result
+    def update_code(self, rep_user, rep_pwd, rep_url, rep_branch):
+        rep_folder = os.path.join(self.root_path, self.get_url_folder(rep_url))
+        if os.path.exists(rep_folder):
+            git_operator = GitOperator(rep_user, rep_pwd, rep_folder)
+            result = git_operator.update_code(rep_branch)
+        else:
+            git_operator = GitOperator(rep_user, rep_pwd, self.root_path)
+            result = git_operator.clone(rep_url, rep_branch)
+        self.commit = git_operator.commit
+        if self.commit == "":
+            result = -1
+            log.ERR("Do not find commit, please check input branch or commit")
+        return result, git_operator.message
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/engine/sse_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/engine/sse_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_build.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_download.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,60 @@
 
 import subprocess
 import os
 import time
 from utils.system import decorate_exception_result
 from utils.firmware_path import FirmwareBinPath
 from utils import log
-from test_framework.state import State
-from utils.system import get_test_platform_version
 
 
-class OakgateDownload(object):
+class PersesSerialDownloader(object):
 
     def __init__(self):
-        super(OakgateDownload, self).__init__()
+        self.fw_path_manage = FirmwareBinPath()
         self.root_path = os.getcwd()
         self.script_path = os.path.join(self.root_path, "Utility")
-        self.logs_path = os.path.join(self.root_path, "Logs")
+        self.logs_path = os.path.join(self.root_path, "Logs", "Two_step")
         self.orig_log_folders = list()
         self.latest_log_folders = list()
-        self.fw_path_manage = FirmwareBinPath()
-
-    def get_fw_path(self, parameters):
-        volume = parameters.get("volume", "ALL")
-        nand = parameters.get("nand", "BICS4")
-        commit = parameters.get("commit", "")
-        fw_path = parameters.get("fw_path", "")
-        if os.path.isfile(fw_path):
-            win_fw_bin = fw_path
-        else:
-            win_fw_bin = self.fw_path_manage.get_image_path(fw_path, volume, commit, nand)
-        return win_fw_bin
-
-    def gen_cmd_line(self, fw_path, ogt):
-        version = get_test_platform_version()
-        if version == 1:
-            cmd = "cd /d {} && python cnex_auto_dl_fw.py --oakgate={} --image2={}".format(self.script_path, ogt, fw_path)
-        else:
-            cmd = "cd /d {} && python cnex_auto_dl_fw.py --oakgate={} --target_image={}".format(self.script_path, ogt, fw_path)
-        log.INFO("oakgate download: {}".format(cmd))
-        return cmd
+        self.log_file = None
+        self.log_path = None
+        # self.init_log_path()
+
+    def init_log_path(self):
+        if os.path.exists(self.logs_path) is False:
+            os.mkdir(self.logs_path)
 
     def get_orig_logs(self):
         log_dirs = os.listdir(self.logs_path)
         for item in log_dirs:
-            if os.path.isdir(os.path.join(self.logs_path, item)):
+            if os.path.isfile(os.path.join(self.logs_path, item)):
                 self.orig_log_folders.append(os.path.join(self.logs_path, item))
 
-    def get_new_log(self, oakgate):
-        new_logs = list()
+    def gen_cmd_line(self, target_ip, com, cap, spi):
+        command_line = f"cd /d {self.script_path} && python two_step_download.py --iroc={target_ip} " \
+                       f"--firmwarePath={cap} --preBinPath={spi} --serialPort={com}"
+        log.INFO(f"Perses two step: {command_line}")
+        return command_line
+
+    def get_new_log(self):
         self.latest_log_folders = os.listdir(self.logs_path)
+        new_logs = list()
         for item in self.latest_log_folders:
             log_item = os.path.join(self.logs_path, item)
-            if os.path.isdir(log_item):
+            if os.path.isfile(log_item):
                 if log_item not in self.orig_log_folders:
-                    for new_log_item in os.listdir(log_item):
-                        if os.path.isfile(os.path.join(log_item, new_log_item)):
-                            if oakgate in new_log_item:    # check if this log belong to correct oagkate
-                                new_logs.append(os.path.join(log_item, new_log_item))
+                    new_logs.append(log_item)
         return new_logs
 
     @decorate_exception_result
     def run(self, parameters):
-        fw_path = self.fw_path_manage.get_fw_path_from_parameter(parameters)
-        oakgate = parameters["oakgate"]
-        self.get_orig_logs()
-        cmd = self.gen_cmd_line(fw_path, oakgate)
-        ret = os.system(cmd)
-        logs = self.get_new_log(oakgate)
+        ret = -1
+        com_port = parameters["com"]
+        target_ip = parameters.get("target_ip", None)
+        spi_path = self.fw_path_manage.get_spi_path(parameters)
+        cap_path = self.fw_path_manage.get_cap(parameters)
+        if spi_path is not None and cap_path is not None and target_ip is not None:
+            command_line = self.gen_cmd_line(target_ip, com_port, cap_path, spi_path)
+            ret = os.system(command_line)
+        logs = "pass" if ret == 0 else "fail"
         return ret, logs
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 
 import os
 import platform
 from multiprocessing import Queue
 from utils.system import decorate_exception_result
 from test_framework.engine.perses_engine import PersesEngine
-from test_framework.engine.perses_power_cycle_engine import PersesPowerEngine
+from test_framework.firmware_engine.serial_download_engine import PersesSerialDownloader
 from test_framework.test_base import TestBase
 from utils import log
-from test_framework.state import State
+from test_framework.state import State, UpgradeType
+
 
 class PersesDownload(TestBase):
 
     def __init__(self):
         super(PersesDownload, self).__init__()
         self.root_path = os.getcwd()
-        if "win" in platform.system().lower():
-            self.perses_engine = PersesPowerEngine()
-        else:
-            self.perses_engine = PersesEngine()
         self.download_testcase = "test_debug:TestPowerCycleDebug.test_auto_fw_upgrade"
 
-    @decorate_exception_result
-    def run(self, parameters):
+    def nvme_download(self, parameters):
         queue = Queue()
+        ret, logs = -1, ""
         test_path = self.get_all_script_path(self.download_testcase)
         if test_path:
             for index in range(1):
                 log.INFO("########Perses Download test path: {}, loop: {}".format(test_path[0], index))
-                self.perses_engine.run(self.download_testcase, test_path[0], parameters, queue)
+                perses_engine = PersesEngine()
+                perses_engine.run(self.download_testcase, test_path[0], parameters, queue)
                 result = queue.get(True)
                 logs = result["log"]
                 if result["result"] == State.PASS:
                     log.INFO("########test passed: {}".format(index))
                     ret = 0
                     break
-                ret = -1
         else:
             ret = State.ERROR_NOT_FOUND
             logs = "NOT find test case: {}".format(self.download_testcase)
         return ret, logs
 
+    @staticmethod
+    def two_step_download(parameters):
+        engine = PersesSerialDownloader()
+        ret, logs = engine.run(parameters)
+        return ret, logs
+
+    @decorate_exception_result
+    def run(self, parameters):
+        if parameters.get("upgrade_type", 1) == UpgradeType.NVMe[0]:
+            ret, logs = self.nvme_download(parameters)
+        else:
+            ret, logs = self.two_step_download(parameters)
+        return ret, logs
+
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,90 @@
 
 import subprocess
 import os
 import time
 from utils.system import decorate_exception_result
+from utils.firmware_path import FirmwareBinPath
+from utils import log
+from test_framework.state import State, UpgradeType
+from utils.system import get_test_platform_version
 
 
-class SerialDownloader(object):
+class OakgateDownload(object):
 
     def __init__(self):
+        super(OakgateDownload, self).__init__()
         self.root_path = os.getcwd()
         self.script_path = os.path.join(self.root_path, "Utility")
-        self.logs_path = os.path.join(self.root_path, "Logs", "Two_step")
+        self.logs_path = os.path.join(self.root_path, "Logs")
         self.orig_log_folders = list()
         self.latest_log_folders = list()
-        self.log_file = None
-        self.log_path = None
-        self.init_log_path()
-
-    def init_log_path(self):
-        if os.path.exists(self.logs_path) is False:
-            os.mkdir(self.logs_path)
+        self.fw_path_manage = FirmwareBinPath()
+
+    def get_fw_path(self, parameters):
+        nand = parameters.get("nand", "BICS5")
+        commit = parameters.get("commit", "")
+        fw_path = parameters.get("fw_path", "")
+        if os.path.isfile(fw_path):
+            win_fw_bin = fw_path
+        else:
+            win_fw_bin = self.fw_path_manage.get_image_path(fw_path, commit, nand)
+        return win_fw_bin
+
+    def gen_nvme_cmd_line(self, fw_path, ogt):
+        version = get_test_platform_version()
+        if version == 1:
+            cmd = "cd /d {} && python cnex_auto_dl_fw.py --oakgate={} --image2={}".format(self.script_path, ogt, fw_path)
+        else:
+            cmd = "cd /d {} && python cnex_auto_dl_fw.py --oakgate={} --target_image={}".format(self.script_path, ogt, fw_path)
+        log.INFO("oakgate download: {}".format(cmd))
+        return cmd
+
+    def gen_two_step_cmd_line(self, fw_path, spi_fw, ogt, com):
+
+        cmd = f"cd /d {self.script_path} && python two_step_download.py --oakgate {ogt} --firmwarePath {fw_path} " \
+              f"--serialPort {com} --preBinPath {spi_fw}"
+        log.INFO("oakgate two step download: {}".format(cmd))
+        return cmd
 
     def get_orig_logs(self):
         log_dirs = os.listdir(self.logs_path)
         for item in log_dirs:
-            if os.path.isfile(os.path.join(self.logs_path, item)):
+            if os.path.isdir(os.path.join(self.logs_path, item)):
                 self.orig_log_folders.append(os.path.join(self.logs_path, item))
 
-    def gen_cmd_line(self, com_port, fw_path, oakgate, pre_bin_path):
-        command_line = "cd /d {} && python two_step_download.py --oakgate={} --firmwarePath={} --preBinPath={} --serialPort={}"\
-            .format(self.script_path, oakgate, fw_path, pre_bin_path, com_port)
-        return command_line
-
-    def execute_command(self, cmd):
-        ret = os.system(cmd)
-        unused_err = ""
-        return ret, unused_err
-
-    def get_bin_path(self, fw_path, vol, commit):
-        if os.path.isfile(fw_path):
-            bin_path = fw_path
-        else:
-            bin_path = self.get_fw_path(fw_path, vol, commit)
-        return bin_path
-
-    def get_spi_bin(self, fw_path):
-        spi_bin_path = None
-        if os.path.isdir(fw_path):
-            spi_bin_path = self.get_spi_path(fw_path)
-        return spi_bin_path
-
-    def get_fw_path(self, fw_path, vol, commit):
-        for file_name in os.listdir(fw_path):
-            if os.path.isfile(os.path.join(fw_path, file_name)):
-                if "_{}_".format(vol) in file_name and commit in file_name and file_name.endswith(".cap"):
-                    return os.path.join(fw_path, file_name)
-        return None
-
-    def get_spi_path(self, fw_path):
-        for file_name in os.listdir(fw_path):
-            if os.path.isfile(os.path.join(fw_path, file_name)):
-                if "spi" in file_name.lower() and file_name.endswith(".cap"):
-                    return os.path.join(fw_path, file_name)
-        return None
-
-    def get_new_log(self):
-        self.latest_log_folders = os.listdir(self.logs_path)
+    def get_new_log(self, oakgate):
         new_logs = list()
+        self.latest_log_folders = os.listdir(self.logs_path)
         for item in self.latest_log_folders:
             log_item = os.path.join(self.logs_path, item)
-            if os.path.isfile(log_item):
+            if os.path.isdir(log_item):
                 if log_item not in self.orig_log_folders:
-                    new_logs.append(log_item)
+                    for new_log_item in os.listdir(log_item):
+                        if os.path.isfile(os.path.join(log_item, new_log_item)):
+                            if oakgate in new_log_item:    # check if this log belong to correct oagkate
+                                new_logs.append(os.path.join(log_item, new_log_item))
         return new_logs
 
-    def create_error_log(self, content):
-        error_log = os.path.join(self.logs_path, "error_{}.log".format(time.time()))
-        err_file = open(error_log, "w")
-        try:
-            if type(content) is bytes:
-                err_file.write(content.decode('utf-8', 'ignore'))
-            else:
-                err_file.write(str(content))
-        except Exception as e:
-            print("Write error failed", e)
-        err_file.close()
-        return error_log
-
     @decorate_exception_result
     def run(self, parameters):
-        com_port = parameters["com"]
-        fw_path = parameters["fw_path"]
-        oakgate = parameters["oakgate"]
-        vol = parameters["volume"]
-        commit = parameters["commit"]
+        cmd = None
+        oakgate = parameters.get("oakgate", None)
+        com = parameters.get("com", None)
         self.get_orig_logs()
-        bin_path = self.get_bin_path(fw_path, vol, commit)
-        pre_bin_path = self.get_spi_bin(fw_path)
-        if bin_path is not None:
-            command_line = self.gen_cmd_line(com_port, bin_path, oakgate, pre_bin_path)
-            print(command_line)
-            ret, unused_err = self.execute_command(command_line)
+        if parameters.get("upgrade_type", 1) == UpgradeType.NVMe[0]:
+            fw_path = self.fw_path_manage.get_fw_path_from_parameter(parameters)
+            if oakgate is not None and fw_path is not None:
+                cmd = self.gen_nvme_cmd_line(fw_path, oakgate)
+        else:
+            spi_path = self.fw_path_manage.get_spi_path(parameters)
+            cap_path = self.fw_path_manage.get_cap(parameters)
+            print(spi_path, cap_path, oakgate)
+            if spi_path is not None and cap_path is not None and oakgate is not None:
+                cmd = self.gen_two_step_cmd_line(cap_path, spi_path, oakgate, com)
+        if cmd is not None:
+            ret = os.system(cmd)
+            logs = self.get_new_log(oakgate)
         else:
-            ret = 1
-            unused_err = ("Did not find fw bin at: {}".format(fw_path))
-        error_log = self.create_error_log(unused_err)
-        logs = self.get_new_log()
-        logs.append(error_log)
+            ret = -1
+            logs = f"OGT upgrade fail: com: {com},ogt:{oakgate}"
         return ret, logs
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/node_database.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/node_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/performance_database.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/performance_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         time_list = list()
         for item in [read_bws, write_bws]:
             for item_ in item:
                 if item_["time"] not in time_list:
                     time_list.append(item_["time"])
         value_lists = list()
         for index in time_list:
-            write_value =  [item["value"] for item in write_bws if item["time"]==index]
-            read_value =  [item["value"] for item in read_bws if item["time"]==index]
+            write_value = [item["value"] for item in write_bws if item["time"] == index]
+            read_value = [item["value"] for item in read_bws if item["time"] == index]
             if write_value or read_value:
                 rw_item = dict()
                 rw_item["time"] = index
                 rw_item["write"] = write_value[0] if write_value else 0
                 rw_item["read"] = read_value[0] if read_value else 0
                 value_lists.append(rw_item)
         for index in value_lists:
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/state.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,7 +89,13 @@
         Standby: "Standby",
         Build: "Build",
         Download: "Download",
         Testing: "Testing",
         Lost: "Lost",
     }
 
+
+class UpgradeType(object):
+
+    NVMe = (0, "nvme")
+    TwoStepDownload = (1, "two step download")
+
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/status_file.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/status_file.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_base.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_base.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_benchmark.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_benchmark_group.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_benchmark_group.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_case.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_case.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_pool.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from test_framework.test_benchmark_group import TestBenchmarkGroup
 from test_framework.firmware_download import FirmwareDownloader
 from test_framework.firmware_build import FirmwareBuild
 from test_framework.test_reboot_handle import RebootHandle
 from rest_server.resource.models.helper import MyThread
 from test_framework.state import State
 from test_framework.state import TestType
-from test_framework.database import decorate_add_tests, decorate_update_test_state
-from test_framework.node_database import update_node_state, node_heart_beat
+from test_framework.node_database import node_heart_beat
 from test_framework.state import NodeState
 from test_framework.status_file import StatusFile
 from test_framework.dut.slot import Slot
 from rest_client.web_rest_client import decorate_api_update_test_result, decorate_api_update_node_status
 from utils import log
 
 
@@ -516,20 +515,21 @@
         """
         if type(parameters) is dict:
             if "TARGETIP" in parameters.keys():
                 os.environ["TARGETIP"] = parameters["TARGETIP"]
 
     @staticmethod
     def set_test_parameters(parameters):
-        if type(parameters) is dict:
-            for key in parameters.keys():
-                os.environ[key] = parameters[key]
+        if isinstance(parameters, dict):
+            for key, value in parameters.items():
+                if isinstance(value, str):
+                    os.environ[key] = value
 
     def test_set_parameters(self, parameters):
         print("Custom global parameters: ")
         if type(parameters) is dict:
             for key in parameters.keys():
-                print("parametesr: ", key, os.environ[key])
+                print("parameters: ", key, os.environ[key])
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_reboot_handle.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_reboot_handle.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_result.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_result.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_runner.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_runner.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/test_framework/test_suite.py` & `automation_rest_server-3.6.1/automation_rest_server/test_framework/test_suite.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/dll/buf.dll` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/dll/buf.dll`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/dll/buf.so` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/dll/buf.so`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/dll/build.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/dll/build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/linux_nvme.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/linux_nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/buf.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/ctype.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/ctype.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/get_feature.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/get_feature.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/ioctl.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/ioctl.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/nvme.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/command.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/command.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/features.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/features.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/hmb.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/hmb.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/identify.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/identify.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/log_page.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/log_page.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/memory.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/memory.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/pcie.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/pcie.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/struct/registers.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/struct/registers.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/device/nvme/utility_vu.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/device/nvme/utility_vu.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/diskpart/diskpart.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/diskpart/diskpart.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/fio/fio.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/fio/fio.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/fio/fio_linux.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/fio/fio_linux.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/fio/tool/fio` & `automation_rest_server-3.6.1/automation_rest_server/tool/fio/tool/fio`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/git/git_operator.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/git/git_operator.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/tool/iometer/iometer.py` & `automation_rest_server-3.6.1/automation_rest_server/tool/iometer/iometer.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/utils/buf.py` & `automation_rest_server-3.6.1/automation_rest_server/utils/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/utils/firmware_path.py` & `automation_rest_server-3.6.1/automation_rest_server/utils/firmware_path.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,355 +4,344 @@
 00000030: 7469 6c73 2069 6d70 6f72 7420 6c6f 670d  tils import log.
 00000040: 0a0d 0a0d 0a63 6c61 7373 2046 6972 6d77  .....class Firmw
 00000050: 6172 6542 696e 5061 7468 286f 626a 6563  areBinPath(objec
 00000060: 7429 3a0d 0a0d 0a20 2020 2064 6566 205f  t):....    def _
 00000070: 5f69 6e69 745f 5f28 7365 6c66 293a 0d0a  _init__(self):..
 00000080: 2020 2020 2020 2020 7365 6c66 2e6c 696e          self.lin
 00000090: 7578 5f70 6174 6820 3d20 222f 686f 6d65  ux_path = "/home
-000000a0: 2f73 6861 7265 2f72 656c 6561 7365 2f72  /share/release/r
-000000b0: 6564 7461 696c 220d 0a20 2020 2020 2020  edtail"..       
-000000c0: 2073 656c 662e 7769 6e64 6f77 735f 7061   self.windows_pa
-000000d0: 7468 203d 2072 225c 5c31 3732 2e32 392e  th = r"\\172.29.
-000000e0: 3139 302e 345c 7368 6172 655c 7265 6c65  190.4\share\rele
-000000f0: 6173 655c 7265 6474 6169 6c22 0d0a 2020  ase\redtail"..  
-00000100: 2020 2020 2020 7365 6c66 2e61 7574 6f5f        self.auto_
-00000110: 6275 696c 645f 666f 6c64 6572 203d 2022  build_folder = "
-00000120: 6e69 6768 746c 7922 0d0a 0d0a 2020 2020  nightly"....    
-00000130: 6465 6620 6765 745f 6465 6661 756c 745f  def get_default_
-00000140: 6261 7365 5f70 6174 6828 7365 6c66 293a  base_path(self):
-00000150: 0d0a 2020 2020 2020 2020 6966 2022 7769  ..        if "wi
-00000160: 6e22 2069 6e20 7379 732e 706c 6174 666f  n" in sys.platfo
-00000170: 726d 2e6c 6f77 6572 2829 3a0d 0a20 2020  rm.lower():..   
-00000180: 2020 2020 2020 2020 2062 6173 655f 7061           base_pa
-00000190: 7468 203d 2073 656c 662e 7769 6e64 6f77  th = self.window
-000001a0: 735f 7061 7468 0d0a 2020 2020 2020 2020  s_path..        
-000001b0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000001c0: 2020 2062 6173 655f 7061 7468 203d 2073     base_path = s
-000001d0: 656c 662e 6c69 6e75 785f 7061 7468 0d0a  elf.linux_path..
-000001e0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-000001f0: 6173 655f 7061 7468 0d0a 0d0a 2020 2020  ase_path....    
-00000200: 6465 6620 6765 745f 696d 6167 655f 7061  def get_image_pa
-00000210: 7468 2873 656c 662c 2062 6173 655f 7061  th(self, base_pa
-00000220: 7468 2c20 766f 6c75 6d65 2c20 636f 6d6d  th, volume, comm
-00000230: 6974 5f69 642c 206e 616e 6429 3a0d 0a20  it_id, nand):.. 
-00000240: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-00000250: 682e 6578 6973 7473 2862 6173 655f 7061  h.exists(base_pa
-00000260: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
-00000270: 2020 636f 6d6d 6974 5f36 6269 7420 3d20    commit_6bit = 
-00000280: 636f 6d6d 6974 5f69 645b 303a 365d 0d0a  commit_id[0:6]..
-00000290: 2020 2020 2020 2020 2020 2020 6e61 6e64              nand
-000002a0: 203d 2022 414c 4c22 2069 6620 766f 6c75   = "ALL" if volu
-000002b0: 6d65 2e6c 6f77 6572 2829 203d 3d20 2261  me.lower() == "a
-000002c0: 6c6c 2220 656c 7365 206e 616e 640d 0a20  ll" else nand.. 
-000002d0: 2020 2020 2020 2020 2020 206e 616e 6420             nand 
-000002e0: 3d20 6e61 6e64 2e6c 6f77 6572 2829 0d0a  = nand.lower()..
-000002f0: 2020 2020 2020 2020 2020 2020 766f 6c75              volu
-00000300: 6d65 203d 2076 6f6c 756d 652e 6c6f 7765  me = volume.lowe
-00000310: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
-00000320: 205f 6669 6c65 7320 3d20 6f73 2e6c 6973   _files = os.lis
-00000330: 7464 6972 2862 6173 655f 7061 7468 290d  tdir(base_path).
-00000340: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00000350: 2069 7465 6d20 696e 205f 6669 6c65 733a   item in _files:
-00000360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000370: 2020 6974 656d 5f70 6174 6820 3d20 6f73    item_path = os
-00000380: 2e70 6174 682e 6a6f 696e 2862 6173 655f  .path.join(base_
-00000390: 7061 7468 2c20 6974 656d 290d 0a20 2020  path, item)..   
-000003a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000003b0: 6f73 2e70 6174 682e 6973 6469 7228 6974  os.path.isdir(it
-000003c0: 656d 5f70 6174 6829 2061 6e64 2063 6f6d  em_path) and com
-000003d0: 6d69 745f 3662 6974 2069 6e20 6974 656d  mit_6bit in item
-000003e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000003f0: 2020 2020 2020 2072 6574 203d 2073 656c         ret = sel
-00000400: 662e 6765 745f 696d 6167 655f 7061 7468  f.get_image_path
-00000410: 2869 7465 6d5f 7061 7468 2c20 766f 6c75  (item_path, volu
-00000420: 6d65 2c20 636f 6d6d 6974 5f69 642c 206e  me, commit_id, n
-00000430: 616e 6429 0d0a 2020 2020 2020 2020 2020  and)..          
-00000440: 2020 2020 2020 2020 2020 6966 2072 6574            if ret
-00000450: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00000460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000470: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00000480: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-00000490: 2020 2065 6c69 6620 2822 5f7b 7d5f 222e     elif ("_{}_".
-000004a0: 666f 726d 6174 2876 6f6c 756d 6529 2069  format(volume) i
-000004b0: 6e20 6974 656d 2e6c 6f77 6572 2829 2920  n item.lower()) 
-000004c0: 616e 6420 2822 7072 6542 6f6f 746c 6f61  and ("preBootloa
-000004d0: 6465 7222 2e6c 6f77 6572 2829 206e 6f74  der".lower() not
-000004e0: 2069 6e20 6974 656d 2e6c 6f77 6572 2829   in item.lower()
-000004f0: 2920 616e 6420 5c0d 0a20 2020 2020 2020  ) and \..       
-00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000510: 2069 7465 6d2e 656e 6473 7769 7468 2822   item.endswith("
-00000520: 2e62 696e 2229 2061 6e64 2028 225f 7b7d  .bin") and ("_{}
-00000530: 5f22 2e66 6f72 6d61 7428 6e61 6e64 2920  _".format(nand) 
-00000540: 696e 2069 7465 6d2e 6c6f 7765 7228 2929  in item.lower())
-00000550: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000560: 2020 2020 2020 2072 6574 7572 6e20 6f73         return os
-00000570: 2e70 6174 682e 6a6f 696e 2862 6173 655f  .path.join(base_
-00000580: 7061 7468 2c20 6974 656d 290d 0a0d 0a20  path, item).... 
-00000590: 2020 2064 6566 2067 6574 5f66 775f 7061     def get_fw_pa
-000005a0: 7468 5f66 726f 6d5f 7061 7261 6d65 7465  th_from_paramete
-000005b0: 7228 7365 6c66 2c20 7061 7261 6d65 7465  r(self, paramete
-000005c0: 7273 2c20 6261 7365 5f70 6174 683d 2222  rs, base_path=""
-000005d0: 293a 0d0a 2020 2020 2020 2020 766f 6c75  ):..        volu
-000005e0: 6d65 203d 2070 6172 616d 6574 6572 732e  me = parameters.
-000005f0: 6765 7428 2276 6f6c 756d 6522 2c20 2241  get("volume", "A
-00000600: 4c4c 2229 0d0a 2020 2020 2020 2020 6e61  LL")..        na
-00000610: 6e64 203d 2070 6172 616d 6574 6572 732e  nd = parameters.
-00000620: 6765 7428 226e 616e 6422 2c20 2241 4c4c  get("nand", "ALL
-00000630: 2229 0d0a 2020 2020 2020 2020 636f 6d6d  ")..        comm
-00000640: 6974 203d 2070 6172 616d 6574 6572 732e  it = parameters.
-00000650: 6765 7428 2263 6f6d 6d69 7422 2c20 2222  get("commit", ""
-00000660: 290d 0a20 2020 2020 2020 2066 775f 7061  )..        fw_pa
-00000670: 7468 203d 2070 6172 616d 6574 6572 732e  th = parameters.
-00000680: 6765 7428 2266 775f 7061 7468 222c 2062  get("fw_path", b
-00000690: 6173 655f 7061 7468 2920 6966 2062 6173  ase_path) if bas
-000006a0: 655f 7061 7468 203d 3d20 2222 2065 6c73  e_path == "" els
-000006b0: 6520 6261 7365 5f70 6174 680d 0a20 2020  e base_path..   
-000006c0: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-000006d0: 6973 6669 6c65 2866 775f 7061 7468 293a  isfile(fw_path):
-000006e0: 0d0a 2020 2020 2020 2020 2020 2020 6677  ..            fw
-000006f0: 5f62 696e 5f70 6174 6820 3d20 6677 5f70  _bin_path = fw_p
-00000700: 6174 680d 0a20 2020 2020 2020 2065 6c73  ath..        els
-00000710: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000720: 766f 6c75 6d65 203d 2022 414c 4c22 2069  volume = "ALL" i
-00000730: 6620 766f 6c75 6d65 203d 3d20 2222 2065  f volume == "" e
-00000740: 6c73 6520 766f 6c75 6d65 0d0a 2020 2020  lse volume..    
-00000750: 2020 2020 2020 2020 6e61 6e64 203d 2022          nand = "
-00000760: 414c 4c22 2069 6620 6e61 6e64 203d 3d20  ALL" if nand == 
-00000770: 2222 2065 6c73 6520 6e61 6e64 0d0a 2020  "" else nand..  
-00000780: 2020 2020 2020 2020 2020 6c6f 672e 494e            log.IN
-00000790: 464f 2822 6677 2070 6174 6820 7b7d 2076  FO("fw path {} v
-000007a0: 6f6c 756d 6520 7b7d 2063 6f6d 6d69 7420  olume {} commit 
-000007b0: 7b7d 206e 616e 6420 7b7d 222e 666f 726d  {} nand {}".form
-000007c0: 6174 2866 775f 7061 7468 2c20 766f 6c75  at(fw_path, volu
-000007d0: 6d65 2c20 636f 6d6d 6974 2c20 6e61 6e64  me, commit, nand
-000007e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000007f0: 6677 5f62 696e 5f70 6174 6820 3d20 7365  fw_bin_path = se
-00000800: 6c66 2e67 6574 5f69 6d61 6765 5f70 6174  lf.get_image_pat
-00000810: 6828 6677 5f70 6174 682c 2076 6f6c 756d  h(fw_path, volum
-00000820: 652c 2063 6f6d 6d69 742c 206e 616e 6429  e, commit, nand)
-00000830: 0d0a 2020 2020 2020 2020 6c6f 672e 494e  ..        log.IN
-00000840: 464f 2822 4765 7420 7061 7468 2066 726f  FO("Get path fro
-00000850: 6d20 7061 7261 6d65 7465 7273 3a20 7b7d  m parameters: {}
-00000860: 222e 666f 726d 6174 2866 775f 6269 6e5f  ".format(fw_bin_
-00000870: 7061 7468 2929 0d0a 2020 2020 2020 2020  path))..        
-00000880: 7265 7475 726e 2066 775f 6269 6e5f 7061  return fw_bin_pa
-00000890: 7468 0d0a 0d0a 2020 2020 4073 7461 7469  th....    @stati
-000008a0: 636d 6574 686f 640d 0a20 2020 2064 6566  cmethod..    def
-000008b0: 2063 6861 6e67 655f 7061 7468 5f77 696e   change_path_win
-000008c0: 5f32 5f6c 696e 7578 2877 696e 5f70 6174  _2_linux(win_pat
-000008d0: 6829 3a0d 0a20 2020 2020 2020 2069 6620  h):..        if 
-000008e0: 7769 6e5f 7061 7468 2069 7320 6e6f 7420  win_path is not 
-000008f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00000900: 2020 2070 6174 685f 7465 6d70 203d 2077     path_temp = w
-00000910: 696e 5f70 6174 682e 7265 706c 6163 6528  in_path.replace(
-00000920: 225c 5c5c 5c31 3732 2e32 392e 3139 302e  "\\\\172.29.190.
-00000930: 3422 2c20 222f 686f 6d65 2229 0d0a 2020  4", "/home")..  
-00000940: 2020 2020 2020 2020 2020 6c69 6e75 785f            linux_
-00000950: 7061 7468 203d 2070 6174 685f 7465 6d70  path = path_temp
-00000960: 2e72 6570 6c61 6365 2822 5c5c 222c 2022  .replace("\\", "
-00000970: 2f22 290d 0a20 2020 2020 2020 2020 2020  /")..           
-00000980: 206c 6f67 2e49 4e46 4f28 2247 6574 206c   log.INFO("Get l
-00000990: 696e 7578 2070 6174 683a 207b 7d22 2e66  inux path: {}".f
-000009a0: 6f72 6d61 7428 6c69 6e75 785f 7061 7468  ormat(linux_path
-000009b0: 2929 0d0a 2020 2020 2020 2020 656c 7365  ))..        else
-000009c0: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-000009d0: 696e 7578 5f70 6174 6820 3d20 226e 6f74  inux_path = "not
-000009e0: 5f66 696e 645f 6c69 6e75 785f 7061 7468  _find_linux_path
-000009f0: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00000a00: 6e20 6c69 6e75 785f 7061 7468 0d0a 0d0a  n linux_path....
-00000a10: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-00000a20: 640d 0a20 2020 2064 6566 2063 6861 6e67  d..    def chang
-00000a30: 655f 7061 7468 5f6c 696e 7578 5f32 5f77  e_path_linux_2_w
-00000a40: 696e 286c 696e 7578 5f70 6174 6829 3a0d  in(linux_path):.
-00000a50: 0a20 2020 2020 2020 2069 6620 6c69 6e75  .        if linu
-00000a60: 785f 7061 7468 2069 7320 6e6f 7420 4e6f  x_path is not No
-00000a70: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00000a80: 206c 696e 7578 5f70 6174 6820 3d20 6c69   linux_path = li
-00000a90: 6e75 785f 7061 7468 2e72 6570 6c61 6365  nux_path.replace
-00000aa0: 2822 2f2f 222c 2022 2f22 290d 0a20 2020  ("//", "/")..   
-00000ab0: 2020 2020 2020 2020 2070 6174 685f 7465           path_te
-00000ac0: 6d70 203d 206c 696e 7578 5f70 6174 682e  mp = linux_path.
-00000ad0: 7265 706c 6163 6528 222f 686f 6d65 222c  replace("/home",
-00000ae0: 2022 5c5c 5c5c 3137 322e 3239 2e31 3930   "\\\\172.29.190
-00000af0: 2e34 2229 0d0a 2020 2020 2020 2020 2020  .4")..          
-00000b00: 2020 7769 6e5f 7061 7468 203d 2070 6174    win_path = pat
-00000b10: 685f 7465 6d70 2e72 6570 6c61 6365 2822  h_temp.replace("
-00000b20: 2f22 2c20 225c 5c22 290d 0a20 2020 2020  /", "\\")..     
-00000b30: 2020 2020 2020 206c 6f67 2e49 4e46 4f28         log.INFO(
-00000b40: 2247 6574 2077 696e 2070 6174 683a 207b  "Get win path: {
-00000b50: 7d22 2e66 6f72 6d61 7428 7769 6e5f 7061  }".format(win_pa
-00000b60: 7468 2929 0d0a 2020 2020 2020 2020 656c  th))..        el
-00000b70: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00000b80: 2077 696e 5f70 6174 6820 3d20 226e 6f74   win_path = "not
-00000b90: 5f66 696e 645f 7769 6e5f 7061 7468 220d  _find_win_path".
-00000ba0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000bb0: 7769 6e5f 7061 7468 0d0a 0d0a 2020 2020  win_path....    
-00000bc0: 6465 6620 6765 745f 6465 6661 756c 745f  def get_default_
-00000bd0: 6261 7365 5f70 6174 685f 656e 6861 6e63  base_path_enhanc
-00000be0: 6528 7365 6c66 2c20 7061 7261 6d65 7465  e(self, paramete
-00000bf0: 7273 293a 0d0a 2020 2020 2020 2020 6966  rs):..        if
-00000c00: 2022 6261 7365 5f70 6174 6822 2069 6e20   "base_path" in 
-00000c10: 7061 7261 6d65 7465 7273 2e6b 6579 7328  parameters.keys(
-00000c20: 293a 2020 2320 666f 7220 6f61 6b67 6174  ):  # for oakgat
-00000c30: 650d 0a20 2020 2020 2020 2020 2020 2072  e..            r
-00000c40: 6574 7572 6e20 7061 7261 6d65 7465 7273  eturn parameters
-00000c50: 5b22 6261 7365 5f70 6174 6822 5d0d 0a20  ["base_path"].. 
-00000c60: 2020 2020 2020 2069 6620 2266 775f 7061         if "fw_pa
-00000c70: 7468 2220 696e 2070 6172 616d 6574 6572  th" in parameter
-00000c80: 732e 6b65 7973 2829 3a20 2020 2320 666f  s.keys():   # fo
-00000c90: 7220 7065 7273 6573 0d0a 2020 2020 2020  r perses..      
-00000ca0: 2020 2020 2020 7465 6d70 5f70 6174 6820        temp_path 
-00000cb0: 3d20 7061 7261 6d65 7465 7273 5b22 6677  = parameters["fw
-00000cc0: 5f70 6174 6822 5d0d 0a20 2020 2020 2020  _path"]..       
-00000cd0: 2020 2020 2069 6620 2231 3732 2e32 392e       if "172.29.
-00000ce0: 3139 302e 3422 2069 6e20 7465 6d70 5f70  190.4" in temp_p
-00000cf0: 6174 683a 0d0a 2020 2020 2020 2020 2020  ath:..          
-00000d00: 2020 2020 2020 6966 2022 7769 6e22 2069        if "win" i
-00000d10: 6e20 7379 732e 706c 6174 666f 726d 2e6c  n sys.platform.l
-00000d20: 6f77 6572 2829 3a0d 0a20 2020 2020 2020  ower():..       
-00000d30: 2020 2020 2020 2020 2020 2020 2062 6173               bas
-00000d40: 655f 7061 7468 203d 2074 656d 705f 7061  e_path = temp_pa
-00000d50: 7468 0d0a 2020 2020 2020 2020 2020 2020  th..            
-00000d60: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00000d80: 6173 655f 7061 7468 203d 2073 656c 662e  ase_path = self.
-00000d90: 6368 616e 6765 5f70 6174 685f 7769 6e5f  change_path_win_
-00000da0: 325f 6c69 6e75 7828 7465 6d70 5f70 6174  2_linux(temp_pat
-00000db0: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-00000dc0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00000dd0: 2020 2020 2020 2062 6173 655f 7061 7468         base_path
-00000de0: 203d 2074 656d 705f 7061 7468 0d0a 2020   = temp_path..  
-00000df0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00000e00: 2020 2020 2020 2020 2062 6173 655f 7061           base_pa
-00000e10: 7468 203d 2073 656c 662e 6765 745f 6465  th = self.get_de
-00000e20: 6661 756c 745f 6261 7365 5f70 6174 6828  fault_base_path(
-00000e30: 290d 0a20 2020 2020 2020 206c 6f67 2e49  )..        log.I
-00000e40: 4e46 4f28 2247 6574 2062 6173 6520 7061  NFO("Get base pa
-00000e50: 7468 3a20 7b7d 222e 666f 726d 6174 2862  th: {}".format(b
-00000e60: 6173 655f 7061 7468 2929 0d0a 2020 2020  ase_path))..    
-00000e70: 2020 2020 7265 7475 726e 2062 6173 655f      return base_
-00000e80: 7061 7468 0d0a 0d0a 2020 2020 6465 6620  path....    def 
-00000e90: 6765 6e65 7261 7465 5f6f 616b 6761 7465  generate_oakgate
-00000ea0: 5f69 6d61 6765 7328 7365 6c66 2c20 7061  _images(self, pa
-00000eb0: 7261 6d65 7465 7273 293a 0d0a 2020 2020  rameters):..    
-00000ec0: 2020 2020 6f75 7470 7574 5f70 6172 6d20      output_parm 
-00000ed0: 3d20 6469 6374 2829 0d0a 2020 2020 2020  = dict()..      
-00000ee0: 2020 766f 6c75 6d65 203d 2070 6172 616d    volume = param
-00000ef0: 6574 6572 732e 6765 7428 2276 6f6c 756d  eters.get("volum
-00000f00: 6522 2c20 2241 4c4c 2229 0d0a 2020 2020  e", "ALL")..    
-00000f10: 2020 2020 6e61 6e64 203d 2070 6172 616d      nand = param
-00000f20: 6574 6572 732e 6765 7428 226e 616e 6422  eters.get("nand"
-00000f30: 2c20 2241 4c4c 2229 0d0a 2020 2020 2020  , "ALL")..      
-00000f40: 2020 6261 7365 5f70 6174 6820 3d20 7365    base_path = se
-00000f50: 6c66 2e67 6574 5f64 6566 6175 6c74 5f62  lf.get_default_b
-00000f60: 6173 655f 7061 7468 5f65 6e68 616e 6365  ase_path_enhance
-00000f70: 2870 6172 616d 6574 6572 7329 0d0a 2020  (parameters)..  
-00000f80: 2020 2020 2020 6966 2022 696d 6167 6531        if "image1
-00000f90: 2220 6e6f 7420 696e 2070 6172 616d 6574  " not in paramet
-00000fa0: 6572 732e 6b65 7973 2829 2061 6e64 2022  ers.keys() and "
-00000fb0: 6261 7365 5f76 6572 7369 6f6e 2220 696e  base_version" in
-00000fc0: 2070 6172 616d 6574 6572 732e 6b65 7973   parameters.keys
-00000fd0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00000fe0: 2072 6574 203d 2073 656c 662e 6765 745f   ret = self.get_
-00000ff0: 696d 6167 655f 7061 7468 2862 6173 655f  image_path(base_
-00001000: 7061 7468 2c20 766f 6c75 6d65 2c20 7061  path, volume, pa
-00001010: 7261 6d65 7465 7273 5b22 6261 7365 5f76  rameters["base_v
-00001020: 6572 7369 6f6e 225d 2c20 6e61 6e64 290d  ersion"], nand).
-00001030: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00001040: 7265 7420 6973 206e 6f74 204e 6f6e 653a  ret is not None:
-00001050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001060: 2020 6f75 7470 7574 5f70 6172 6d5b 2269    output_parm["i
-00001070: 6d61 6765 3122 5d20 3d20 7265 740d 0a20  mage1"] = ret.. 
-00001080: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00001090: 7574 7075 745f 7061 726d 5b22 6261 7365  utput_parm["base
-000010a0: 5f76 6572 7369 6f6e 225d 203d 2070 6172  _version"] = par
-000010b0: 616d 6574 6572 735b 2262 6173 655f 7665  ameters["base_ve
-000010c0: 7273 696f 6e22 5d0d 0a20 2020 2020 2020  rsion"]..       
-000010d0: 2069 6620 2269 6d61 6765 3222 206e 6f74   if "image2" not
-000010e0: 2069 6e20 7061 7261 6d65 7465 7273 2e6b   in parameters.k
-000010f0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-00001100: 2020 2020 6966 2022 7461 7267 6574 5f76      if "target_v
-00001110: 6572 7369 6f6e 2220 696e 2070 6172 616d  ersion" in param
-00001120: 6574 6572 732e 6b65 7973 2829 3a0d 0a20  eters.keys():.. 
-00001130: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001140: 6574 203d 2073 656c 662e 6765 745f 696d  et = self.get_im
-00001150: 6167 655f 7061 7468 2862 6173 655f 7061  age_path(base_pa
-00001160: 7468 2c20 766f 6c75 6d65 2c20 7061 7261  th, volume, para
-00001170: 6d65 7465 7273 5b22 7461 7267 6574 5f76  meters["target_v
-00001180: 6572 7369 6f6e 225d 2c20 6e61 6e64 290d  ersion"], nand).
-00001190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011a0: 2069 6620 7265 7420 6973 206e 6f74 204e   if ret is not N
-000011b0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000011c0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-000011d0: 5f70 6172 6d5b 2269 6d61 6765 3222 5d20  _parm["image2"] 
-000011e0: 3d20 7265 740d 0a20 2020 2020 2020 2020  = ret..         
-000011f0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00001200: 745f 7061 726d 5b22 7461 7267 6574 5f76  t_parm["target_v
-00001210: 6572 7369 6f6e 225d 203d 2070 6172 616d  ersion"] = param
-00001220: 6574 6572 735b 2274 6172 6765 745f 7665  eters["target_ve
-00001230: 7273 696f 6e22 5d0d 0a20 2020 2020 2020  rsion"]..       
-00001240: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00001250: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-00001260: 696d 6167 6531 2220 696e 206f 7574 7075  image1" in outpu
-00001270: 745f 7061 726d 2e6b 6579 7328 293a 0d0a  t_parm.keys():..
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2020 6f75 7470 7574 5f70 6172 6d5b      output_parm[
-000012a0: 2269 6d61 6765 3222 5d20 3d20 6f75 7470  "image2"] = outp
-000012b0: 7574 5f70 6172 6d5b 2269 6d61 6765 3122  ut_parm["image1"
-000012c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000012d0: 2020 2020 2020 206f 7574 7075 745f 7061         output_pa
-000012e0: 726d 5b22 7461 7267 6574 5f76 6572 7369  rm["target_versi
-000012f0: 6f6e 225d 203d 206f 7574 7075 745f 7061  on"] = output_pa
-00001300: 726d 5b22 6261 7365 5f76 6572 7369 6f6e  rm["base_version
-00001310: 225d 0d0a 2020 2020 2020 2020 7265 7475  "]..        retu
-00001320: 726e 206f 7574 7075 745f 7061 726d 0d0a  rn output_parm..
-00001330: 0d0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
-00001340: 5f70 6572 7365 735f 6677 5f70 6174 6828  _perses_fw_path(
-00001350: 7365 6c66 2c20 7061 7261 6d65 7465 7273  self, parameters
-00001360: 293a 0d0a 2020 2020 2020 2020 6966 2022  ):..        if "
-00001370: 6677 5f70 6174 6822 2069 6e20 7061 7261  fw_path" in para
-00001380: 6d65 7465 7273 2e6b 6579 7328 293a 0d0a  meters.keys():..
-00001390: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-000013a0: 7769 6e22 2069 6e20 706c 6174 666f 726d  win" in platform
-000013b0: 2e73 7973 7465 6d28 292e 6c6f 7765 7228  .system().lower(
-000013c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000013d0: 2020 2020 7465 6d70 5f70 6174 6820 3d20      temp_path = 
-000013e0: 7365 6c66 2e63 6861 6e67 655f 7061 7468  self.change_path
-000013f0: 5f6c 696e 7578 5f32 5f77 696e 2870 6172  _linux_2_win(par
-00001400: 616d 6574 6572 735b 2266 775f 7061 7468  ameters["fw_path
-00001410: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
-00001420: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00001430: 2020 2020 2020 2020 7465 6d70 5f70 6174          temp_pat
-00001440: 6820 3d20 7365 6c66 2e63 6861 6e67 655f  h = self.change_
-00001450: 7061 7468 5f77 696e 5f32 5f6c 696e 7578  path_win_2_linux
-00001460: 2870 6172 616d 6574 6572 735b 2266 775f  (parameters["fw_
-00001470: 7061 7468 225d 290d 0a20 2020 2020 2020  path"])..       
-00001480: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00001490: 2020 2020 7465 6d70 5f70 6174 6820 3d20      temp_path = 
-000014a0: 7365 6c66 2e67 6574 5f64 6566 6175 6c74  self.get_default
-000014b0: 5f62 6173 655f 7061 7468 5f65 6e68 616e  _base_path_enhan
-000014c0: 6365 2870 6172 616d 6574 6572 7329 0d0a  ce(parameters)..
-000014d0: 2020 2020 2020 2020 6677 5f70 6174 6820          fw_path 
-000014e0: 3d20 7365 6c66 2e67 6574 5f66 775f 7061  = self.get_fw_pa
-000014f0: 7468 5f66 726f 6d5f 7061 7261 6d65 7465  th_from_paramete
-00001500: 7228 7061 7261 6d65 7465 7273 2c20 7465  r(parameters, te
-00001510: 6d70 5f70 6174 6829 0d0a 2020 2020 2020  mp_path)..      
-00001520: 2020 6966 2066 775f 7061 7468 2069 7320    if fw_path is 
-00001530: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00001540: 2020 2020 2020 206c 6f67 2e49 4e46 4f28         log.INFO(
-00001550: 2275 7064 6174 655f 7065 7273 6573 5f66  "update_perses_f
-00001560: 775f 7061 7468 3a20 7b7d 222e 666f 726d  w_path: {}".form
-00001570: 6174 2866 775f 7061 7468 2929 0d0a 2020  at(fw_path))..  
-00001580: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
-00001590: 7465 7273 5b22 6677 5f70 6174 6822 5d20  ters["fw_path"] 
-000015a0: 3d20 6677 5f70 6174 680d 0a20 2020 2020  = fw_path..     
-000015b0: 2020 2020 2020 206f 732e 656e 7669 726f         os.enviro
-000015c0: 6e5b 2266 775f 7061 7468 225d 203d 2066  n["fw_path"] = f
-000015d0: 775f 7061 7468 0d0a 2020 2020 2020 2020  w_path..        
-000015e0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000015f0: 2020 206c 6f67 2e57 4152 4e28 224e 6f74     log.WARN("Not
-00001600: 2066 696e 6420 7061 7468 3a20 7065 7273   find path: pers
-00001610: 6573 5f66 775f 7061 7468 2229 0d0a 2020  es_fw_path")..  
-00001620: 2020 2020 2020 7072 696e 7428 7061 7261        print(para
-00001630: 6d65 7465 7273 290d 0a20 2020 2020 2020  meters)..       
-00001640: 2072 6574 7572 6e20 7061 7261 6d65 7465   return paramete
-00001650: 7273 0d0a                                rs..
+000000a0: 2f73 6861 7265 2f72 656c 6561 7365 220d  /share/release".
+000000b0: 0a20 2020 2020 2020 2073 656c 662e 7769  .        self.wi
+000000c0: 6e64 6f77 735f 7061 7468 203d 2072 225c  ndows_path = r"\
+000000d0: 5c31 3732 2e32 392e 3139 302e 345c 7368  \172.29.190.4\sh
+000000e0: 6172 655c 7265 6c65 6173 6522 0d0a 2020  are\release"..  
+000000f0: 2020 2020 2020 7365 6c66 2e61 7574 6f5f        self.auto_
+00000100: 6275 696c 645f 666f 6c64 6572 203d 2022  build_folder = "
+00000110: 6e69 6768 746c 7922 0d0a 0d0a 2020 2020  nightly"....    
+00000120: 6465 6620 6765 745f 6465 6661 756c 745f  def get_default_
+00000130: 6261 7365 5f70 6174 6828 7365 6c66 293a  base_path(self):
+00000140: 0d0a 2020 2020 2020 2020 6966 2022 7769  ..        if "wi
+00000150: 6e22 2069 6e20 7379 732e 706c 6174 666f  n" in sys.platfo
+00000160: 726d 2e6c 6f77 6572 2829 3a0d 0a20 2020  rm.lower():..   
+00000170: 2020 2020 2020 2020 2062 6173 655f 7061           base_pa
+00000180: 7468 203d 2073 656c 662e 7769 6e64 6f77  th = self.window
+00000190: 735f 7061 7468 0d0a 2020 2020 2020 2020  s_path..        
+000001a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000001b0: 2020 2062 6173 655f 7061 7468 203d 2073     base_path = s
+000001c0: 656c 662e 6c69 6e75 785f 7061 7468 0d0a  elf.linux_path..
+000001d0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+000001e0: 6173 655f 7061 7468 0d0a 0d0a 2020 2020  ase_path....    
+000001f0: 6465 6620 6765 745f 696d 6167 655f 7061  def get_image_pa
+00000200: 7468 2873 656c 662c 2062 6173 655f 7061  th(self, base_pa
+00000210: 7468 2c20 636f 6d6d 6974 5f69 642c 206e  th, commit_id, n
+00000220: 616e 6429 3a0d 0a20 2020 2020 2020 2069  and):..        i
+00000230: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
+00000240: 2862 6173 655f 7061 7468 293a 0d0a 2020  (base_path):..  
+00000250: 2020 2020 2020 2020 2020 636f 6d6d 6974            commit
+00000260: 5f36 6269 7420 3d20 636f 6d6d 6974 5f69  _6bit = commit_i
+00000270: 645b 303a 365d 0d0a 2020 2020 2020 2020  d[0:6]..        
+00000280: 2020 2020 6e61 6e64 203d 206e 616e 642e      nand = nand.
+00000290: 6c6f 7765 7228 290d 0a20 2020 2020 2020  lower()..       
+000002a0: 2020 2020 205f 6669 6c65 7320 3d20 6f73       _files = os
+000002b0: 2e6c 6973 7464 6972 2862 6173 655f 7061  .listdir(base_pa
+000002c0: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
+000002d0: 2066 6f72 2069 7465 6d20 696e 205f 6669   for item in _fi
+000002e0: 6c65 733a 0d0a 2020 2020 2020 2020 2020  les:..          
+000002f0: 2020 2020 2020 6974 656d 5f70 6174 6820        item_path 
+00000300: 3d20 6f73 2e70 6174 682e 6a6f 696e 2862  = os.path.join(b
+00000310: 6173 655f 7061 7468 2c20 6974 656d 290d  ase_path, item).
+00000320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000330: 2069 6620 6f73 2e70 6174 682e 6973 6469   if os.path.isdi
+00000340: 7228 6974 656d 5f70 6174 6829 2061 6e64  r(item_path) and
+00000350: 2063 6f6d 6d69 745f 3662 6974 2069 6e20   commit_6bit in 
+00000360: 6974 656d 3a0d 0a20 2020 2020 2020 2020  item:..         
+00000370: 2020 2020 2020 2020 2020 2072 6574 203d             ret =
+00000380: 2073 656c 662e 6765 745f 696d 6167 655f   self.get_image_
+00000390: 7061 7468 2869 7465 6d5f 7061 7468 2c20  path(item_path, 
+000003a0: 636f 6d6d 6974 5f69 642c 206e 616e 6429  commit_id, nand)
+000003b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000003c0: 2020 2020 2020 6966 2072 6574 2069 7320        if ret is 
+000003d0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003f0: 2020 2072 6574 7572 6e20 7265 740d 0a20     return ret.. 
+00000400: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00000410: 6c69 6620 2270 7265 426f 6f74 6c6f 6164  lif "preBootload
+00000420: 6572 222e 6c6f 7765 7228 2920 6e6f 7420  er".lower() not 
+00000430: 696e 2069 7465 6d2e 6c6f 7765 7228 2920  in item.lower() 
+00000440: 616e 6420 6974 656d 2e65 6e64 7377 6974  and item.endswit
+00000450: 6828 222e 6269 6e22 2920 616e 6420 5c0d  h(".bin") and \.
+00000460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000470: 2020 2020 2020 2020 2022 7b7d 222e 666f           "{}".fo
+00000480: 726d 6174 286e 616e 6429 2069 6e20 6974  rmat(nand) in it
+00000490: 656d 2e6c 6f77 6572 2829 3a0d 0a20 2020  em.lower():..   
+000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004b0: 2072 6574 7572 6e20 6f73 2e70 6174 682e   return os.path.
+000004c0: 6a6f 696e 2862 6173 655f 7061 7468 2c20  join(base_path, 
+000004d0: 6974 656d 290d 0a0d 0a20 2020 2040 7374  item)....    @st
+000004e0: 6174 6963 6d65 7468 6f64 0d0a 2020 2020  aticmethod..    
+000004f0: 6465 6620 6765 745f 6361 7028 7061 7261  def get_cap(para
+00000500: 6d65 7465 7273 293a 0d0a 2020 2020 2020  meters):..      
+00000510: 2020 6261 7365 5f70 6174 6820 3d20 7061    base_path = pa
+00000520: 7261 6d65 7465 7273 2e67 6574 2822 6677  rameters.get("fw
+00000530: 5f70 6174 6822 2c20 2222 290d 0a20 2020  _path", "")..   
+00000540: 2020 2020 206e 616e 6420 3d20 7061 7261       nand = para
+00000550: 6d65 7465 7273 2e67 6574 2822 6e61 6e64  meters.get("nand
+00000560: 222c 2022 5256 3034 2229 0d0a 2020 2020  ", "RV04")..    
+00000570: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
+00000580: 6f73 2e6c 6973 7464 6972 2862 6173 655f  os.listdir(base_
+00000590: 7061 7468 293a 0d0a 2020 2020 2020 2020  path):..        
+000005a0: 2020 2020 6966 206e 616e 6420 696e 2069      if nand in i
+000005b0: 7465 6d20 616e 6420 6974 656d 2e65 6e64  tem and item.end
+000005c0: 7377 6974 6828 222e 6361 7022 293a 0d0a  swith(".cap"):..
+000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005e0: 7265 7475 726e 206f 732e 7061 7468 2e6a  return os.path.j
+000005f0: 6f69 6e28 6261 7365 5f70 6174 682c 2069  oin(base_path, i
+00000600: 7465 6d29 0d0a 0d0a 2020 2020 6465 6620  tem)....    def 
+00000610: 6765 745f 6677 5f70 6174 685f 6672 6f6d  get_fw_path_from
+00000620: 5f70 6172 616d 6574 6572 2873 656c 662c  _parameter(self,
+00000630: 2070 6172 616d 6574 6572 732c 2062 6173   parameters, bas
+00000640: 655f 7061 7468 3d22 2229 3a0d 0a20 2020  e_path=""):..   
+00000650: 2020 2020 206e 616e 6420 3d20 7061 7261       nand = para
+00000660: 6d65 7465 7273 2e67 6574 2822 6e61 6e64  meters.get("nand
+00000670: 222c 2022 4249 4353 3522 290d 0a20 2020  ", "BICS5")..   
+00000680: 2020 2020 2063 6f6d 6d69 7420 3d20 7061       commit = pa
+00000690: 7261 6d65 7465 7273 2e67 6574 2822 636f  rameters.get("co
+000006a0: 6d6d 6974 222c 2022 2229 0d0a 2020 2020  mmit", "")..    
+000006b0: 2020 2020 6677 5f70 6174 6820 3d20 7061      fw_path = pa
+000006c0: 7261 6d65 7465 7273 2e67 6574 2822 6677  rameters.get("fw
+000006d0: 5f70 6174 6822 2c20 6261 7365 5f70 6174  _path", base_pat
+000006e0: 6829 2069 6620 6261 7365 5f70 6174 6820  h) if base_path 
+000006f0: 3d3d 2022 2220 656c 7365 2062 6173 655f  == "" else base_
+00000700: 7061 7468 0d0a 2020 2020 2020 2020 6966  path..        if
+00000710: 206e 6f74 206f 732e 7061 7468 2e69 7366   not os.path.isf
+00000720: 696c 6528 6677 5f70 6174 6829 3a0d 0a20  ile(fw_path):.. 
+00000730: 2020 2020 2020 2020 2020 206c 6f67 2e49             log.I
+00000740: 4e46 4f28 2266 7720 7061 7468 207b 7d20  NFO("fw path {} 
+00000750: 636f 6d6d 6974 207b 7d20 6e61 6e64 207b  commit {} nand {
+00000760: 7d22 2e66 6f72 6d61 7428 6677 5f70 6174  }".format(fw_pat
+00000770: 682c 2063 6f6d 6d69 742c 206e 616e 6429  h, commit, nand)
+00000780: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00000790: 775f 7061 7468 203d 2073 656c 662e 6765  w_path = self.ge
+000007a0: 745f 696d 6167 655f 7061 7468 2866 775f  t_image_path(fw_
+000007b0: 7061 7468 2c20 636f 6d6d 6974 2c20 6e61  path, commit, na
+000007c0: 6e64 290d 0a20 2020 2020 2020 206c 6f67  nd)..        log
+000007d0: 2e49 4e46 4f28 2247 6574 2070 6174 6820  .INFO("Get path 
+000007e0: 6672 6f6d 2070 6172 616d 6574 6572 733a  from parameters:
+000007f0: 207b 7d22 2e66 6f72 6d61 7428 6677 5f70   {}".format(fw_p
+00000800: 6174 6829 290d 0a20 2020 2020 2020 2072  ath))..        r
+00000810: 6574 7572 6e20 6677 5f70 6174 680d 0a0d  eturn fw_path...
+00000820: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00000830: 6f64 0d0a 2020 2020 6465 6620 6765 745f  od..    def get_
+00000840: 7370 695f 7061 7468 2870 6172 616d 6574  spi_path(paramet
+00000850: 6572 7329 3a0d 0a20 2020 2020 2020 2073  ers):..        s
+00000860: 7069 203d 204e 6f6e 650d 0a20 2020 2020  pi = None..     
+00000870: 2020 2066 775f 7061 7468 203d 2070 6172     fw_path = par
+00000880: 616d 6574 6572 732e 6765 7428 2266 775f  ameters.get("fw_
+00000890: 7061 7468 222c 2022 2229 0d0a 2020 2020  path", "")..    
+000008a0: 2020 2020 6966 206f 732e 7061 7468 2e65      if os.path.e
+000008b0: 7869 7374 7328 6677 5f70 6174 6829 3a0d  xists(fw_path):.
+000008c0: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
+000008d0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+000008e0: 6469 726e 616d 6528 6677 5f70 6174 6829  dirname(fw_path)
+000008f0: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
+00000900: 6c65 2866 775f 7061 7468 2920 656c 7365  le(fw_path) else
+00000910: 2066 775f 7061 7468 0d0a 2020 2020 2020   fw_path..      
+00000920: 2020 2020 2020 6669 6c65 7320 3d20 5b0d        files = [.
+00000930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000940: 206f 732e 7061 7468 2e6a 6f69 6e28 6469   os.path.join(di
+00000950: 725f 7061 7468 2c20 6974 656d 2920 666f  r_path, item) fo
+00000960: 7220 6974 656d 2069 6e20 6f73 2e6c 6973  r item in os.lis
+00000970: 7464 6972 2864 6972 5f70 6174 6829 0d0a  tdir(dir_path)..
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 6966 2022 5f53 5049 4150 505f 2220 696e  if "_SPIAPP_" in
+000009a0: 2069 7465 6d20 616e 6420 6974 656d 2e65   item and item.e
+000009b0: 6e64 7377 6974 6828 222e 6361 7022 290d  ndswith(".cap").
+000009c0: 0a20 2020 2020 2020 2020 2020 205d 0d0a  .            ]..
+000009d0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000009e0: 656e 2866 696c 6573 2920 3d3d 2030 3a0d  en(files) == 0:.
+000009f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a00: 206c 6f67 2e45 5252 2866 2263 616e 206e   log.ERR(f"can n
+00000a10: 6f74 2066 696e 6420 5f53 5049 4150 505f  ot find _SPIAPP_
+00000a20: 2066 696c 6520 696e 2064 6972 6563 746f   file in directo
+00000a30: 7279 3a20 7b64 6972 5f70 6174 687d 2229  ry: {dir_path}")
+00000a40: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00000a50: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000a60: 2020 2020 2073 7069 203d 2066 696c 6573       spi = files
+00000a70: 5b30 5d0d 0a20 2020 2020 2020 2072 6574  [0]..        ret
+00000a80: 7572 6e20 7370 690d 0a0d 0a20 2020 2040  urn spi....    @
+00000a90: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
+00000aa0: 2020 6465 6620 6368 616e 6765 5f70 6174    def change_pat
+00000ab0: 685f 7769 6e5f 325f 6c69 6e75 7828 7769  h_win_2_linux(wi
+00000ac0: 6e5f 7061 7468 293a 0d0a 2020 2020 2020  n_path):..      
+00000ad0: 2020 6966 2077 696e 5f70 6174 6820 6973    if win_path is
+00000ae0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00000af0: 2020 2020 2020 2020 7061 7468 5f74 656d          path_tem
+00000b00: 7020 3d20 7769 6e5f 7061 7468 2e72 6570  p = win_path.rep
+00000b10: 6c61 6365 2822 5c5c 5c5c 3137 322e 3239  lace("\\\\172.29
+00000b20: 2e31 3930 2e34 222c 2022 2f68 6f6d 6522  .190.4", "/home"
+00000b30: 290d 0a20 2020 2020 2020 2020 2020 206c  )..            l
+00000b40: 696e 7578 5f70 6174 6820 3d20 7061 7468  inux_path = path
+00000b50: 5f74 656d 702e 7265 706c 6163 6528 225c  _temp.replace("\
+00000b60: 5c22 2c20 222f 2229 0d0a 2020 2020 2020  \", "/")..      
+00000b70: 2020 2020 2020 6c6f 672e 494e 464f 2822        log.INFO("
+00000b80: 4765 7420 6c69 6e75 7820 7061 7468 3a20  Get linux path: 
+00000b90: 7b7d 222e 666f 726d 6174 286c 696e 7578  {}".format(linux
+00000ba0: 5f70 6174 6829 290d 0a20 2020 2020 2020  _path))..       
+00000bb0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00000bc0: 2020 2020 6c69 6e75 785f 7061 7468 203d      linux_path =
+00000bd0: 2022 6e6f 745f 6669 6e64 5f6c 696e 7578   "not_find_linux
+00000be0: 5f70 6174 6822 0d0a 2020 2020 2020 2020  _path"..        
+00000bf0: 7265 7475 726e 206c 696e 7578 5f70 6174  return linux_pat
+00000c00: 680d 0a0d 0a20 2020 2040 7374 6174 6963  h....    @static
+00000c10: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
+00000c20: 6368 616e 6765 5f70 6174 685f 6c69 6e75  change_path_linu
+00000c30: 785f 325f 7769 6e28 6c69 6e75 785f 7061  x_2_win(linux_pa
+00000c40: 7468 293a 0d0a 2020 2020 2020 2020 6966  th):..        if
+00000c50: 206c 696e 7578 5f70 6174 6820 6973 206e   linux_path is n
+00000c60: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00000c70: 2020 2020 2020 6c69 6e75 785f 7061 7468        linux_path
+00000c80: 203d 206c 696e 7578 5f70 6174 682e 7265   = linux_path.re
+00000c90: 706c 6163 6528 222f 2f22 2c20 222f 2229  place("//", "/")
+00000ca0: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
+00000cb0: 7468 5f74 656d 7020 3d20 6c69 6e75 785f  th_temp = linux_
+00000cc0: 7061 7468 2e72 6570 6c61 6365 2822 2f68  path.replace("/h
+00000cd0: 6f6d 6522 2c20 225c 5c5c 5c31 3732 2e32  ome", "\\\\172.2
+00000ce0: 392e 3139 302e 3422 290d 0a20 2020 2020  9.190.4")..     
+00000cf0: 2020 2020 2020 2077 696e 5f70 6174 6820         win_path 
+00000d00: 3d20 7061 7468 5f74 656d 702e 7265 706c  = path_temp.repl
+00000d10: 6163 6528 222f 222c 2022 5c5c 2229 0d0a  ace("/", "\\")..
+00000d20: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+00000d30: 494e 464f 2822 4765 7420 7769 6e20 7061  INFO("Get win pa
+00000d40: 7468 3a20 7b7d 222e 666f 726d 6174 2877  th: {}".format(w
+00000d50: 696e 5f70 6174 6829 290d 0a20 2020 2020  in_path))..     
+00000d60: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000d70: 2020 2020 2020 7769 6e5f 7061 7468 203d        win_path =
+00000d80: 2022 6e6f 745f 6669 6e64 5f77 696e 5f70   "not_find_win_p
+00000d90: 6174 6822 0d0a 2020 2020 2020 2020 7265  ath"..        re
+00000da0: 7475 726e 2077 696e 5f70 6174 680d 0a0d  turn win_path...
+00000db0: 0a20 2020 2064 6566 2067 6574 5f64 6566  .    def get_def
+00000dc0: 6175 6c74 5f62 6173 655f 7061 7468 5f65  ault_base_path_e
+00000dd0: 6e68 616e 6365 2873 656c 662c 2070 6172  nhance(self, par
+00000de0: 616d 6574 6572 7329 3a0d 0a20 2020 2020  ameters):..     
+00000df0: 2020 2069 6620 2262 6173 655f 7061 7468     if "base_path
+00000e00: 2220 696e 2070 6172 616d 6574 6572 732e  " in parameters.
+00000e10: 6b65 7973 2829 3a20 2023 2066 6f72 206f  keys():  # for o
+00000e20: 616b 6761 7465 0d0a 2020 2020 2020 2020  akgate..        
+00000e30: 2020 2020 7265 7475 726e 2070 6172 616d      return param
+00000e40: 6574 6572 735b 2262 6173 655f 7061 7468  eters["base_path
+00000e50: 225d 0d0a 2020 2020 2020 2020 6966 2022  "]..        if "
+00000e60: 6677 5f70 6174 6822 2069 6e20 7061 7261  fw_path" in para
+00000e70: 6d65 7465 7273 2e6b 6579 7328 293a 2020  meters.keys():  
+00000e80: 2023 2066 6f72 2070 6572 7365 730d 0a20   # for perses.. 
+00000e90: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00000ea0: 7061 7468 203d 2070 6172 616d 6574 6572  path = parameter
+00000eb0: 735b 2266 775f 7061 7468 225d 0d0a 2020  s["fw_path"]..  
+00000ec0: 2020 2020 2020 2020 2020 6966 2022 3137            if "17
+00000ed0: 322e 3239 2e31 3930 2e34 2220 696e 2074  2.29.190.4" in t
+00000ee0: 656d 705f 7061 7468 3a0d 0a20 2020 2020  emp_path:..     
+00000ef0: 2020 2020 2020 2020 2020 2069 6620 2277             if "w
+00000f00: 696e 2220 696e 2073 7973 2e70 6c61 7466  in" in sys.platf
+00000f10: 6f72 6d2e 6c6f 7765 7228 293a 0d0a 2020  orm.lower():..  
+00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f30: 2020 6261 7365 5f70 6174 6820 3d20 7465    base_path = te
+00000f40: 6d70 5f70 6174 680d 0a20 2020 2020 2020  mp_path..       
+00000f50: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f70: 2020 2020 6261 7365 5f70 6174 6820 3d20      base_path = 
+00000f80: 7365 6c66 2e63 6861 6e67 655f 7061 7468  self.change_path
+00000f90: 5f77 696e 5f32 5f6c 696e 7578 2874 656d  _win_2_linux(tem
+00000fa0: 705f 7061 7468 290d 0a20 2020 2020 2020  p_path)..       
+00000fb0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00000fc0: 2020 2020 2020 2020 2020 2020 6261 7365              base
+00000fd0: 5f70 6174 6820 3d20 7465 6d70 5f70 6174  _path = temp_pat
+00000fe0: 680d 0a20 2020 2020 2020 2065 6c73 653a  h..        else:
+00000ff0: 0d0a 2020 2020 2020 2020 2020 2020 6261  ..            ba
+00001000: 7365 5f70 6174 6820 3d20 7365 6c66 2e67  se_path = self.g
+00001010: 6574 5f64 6566 6175 6c74 5f62 6173 655f  et_default_base_
+00001020: 7061 7468 2829 0d0a 2020 2020 2020 2020  path()..        
+00001030: 6c6f 672e 494e 464f 2822 4765 7420 6261  log.INFO("Get ba
+00001040: 7365 2070 6174 683a 207b 7d22 2e66 6f72  se path: {}".for
+00001050: 6d61 7428 6261 7365 5f70 6174 6829 290d  mat(base_path)).
+00001060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001070: 6261 7365 5f70 6174 680d 0a0d 0a20 2020  base_path....   
+00001080: 2064 6566 2067 656e 6572 6174 655f 6f61   def generate_oa
+00001090: 6b67 6174 655f 696d 6167 6573 2873 656c  kgate_images(sel
+000010a0: 662c 2070 6172 616d 6574 6572 7329 3a0d  f, parameters):.
+000010b0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+000010c0: 7061 726d 203d 2064 6963 7428 290d 0a20  parm = dict().. 
+000010d0: 2020 2020 2020 206e 616e 6420 3d20 7061         nand = pa
+000010e0: 7261 6d65 7465 7273 2e67 6574 2822 6e61  rameters.get("na
+000010f0: 6e64 222c 2022 414c 4c22 290d 0a20 2020  nd", "ALL")..   
+00001100: 2020 2020 2066 6f72 2069 6d61 6765 5f6b       for image_k
+00001110: 6579 2069 6e20 5b22 6261 7365 5f69 6d61  ey in ["base_ima
+00001120: 6765 222c 2022 7461 7267 6574 5f69 6d61  ge", "target_ima
+00001130: 6765 225d 3a0d 0a20 2020 2020 2020 2020  ge"]:..         
+00001140: 2020 2069 6620 696d 6167 655f 6b65 7920     if image_key 
+00001150: 696e 2070 6172 616d 6574 6572 733a 0d0a  in parameters:..
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 696d 6167 655f 7061 7468 203d 2070 6172  image_path = par
+00001180: 616d 6574 6572 732e 6765 7428 696d 6167  ameters.get(imag
+00001190: 655f 6b65 7929 0d0a 2020 2020 2020 2020  e_key)..        
+000011a0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+000011b0: 7468 2e69 7364 6972 2869 6d61 6765 5f70  th.isdir(image_p
+000011c0: 6174 6829 3a0d 0a20 2020 2020 2020 2020  ath):..         
+000011d0: 2020 2020 2020 2020 2020 2072 6574 203d             ret =
+000011e0: 2073 656c 662e 6765 745f 696d 6167 655f   self.get_image_
+000011f0: 7061 7468 2869 6d61 6765 5f70 6174 682c  path(image_path,
+00001200: 2022 222c 206e 616e 6429 0d0a 2020 2020   "", nand)..    
+00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001220: 6966 2072 6574 2069 7320 6e6f 7420 4e6f  if ret is not No
+00001230: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00001240: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00001250: 7075 745f 7061 726d 5b69 6d61 6765 5f6b  put_parm[image_k
+00001260: 6579 5d20 3d20 7265 740d 0a20 2020 2020  ey] = ret..     
+00001270: 2020 2072 6574 7572 6e20 6f75 7470 7574     return output
+00001280: 5f70 6172 6d0d 0a0d 0a20 2020 2064 6566  _parm....    def
+00001290: 2075 7064 6174 655f 7065 7273 6573 5f66   update_perses_f
+000012a0: 775f 7061 7468 2873 656c 662c 2070 6172  w_path(self, par
+000012b0: 616d 6574 6572 7329 3a0d 0a20 2020 2020  ameters):..     
+000012c0: 2020 2069 6620 2266 775f 7061 7468 2220     if "fw_path" 
+000012d0: 696e 2070 6172 616d 6574 6572 732e 6b65  in parameters.ke
+000012e0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+000012f0: 2020 2069 6620 2277 696e 2220 696e 2070     if "win" in p
+00001300: 6c61 7466 6f72 6d2e 7379 7374 656d 2829  latform.system()
+00001310: 2e6c 6f77 6572 2829 3a0d 0a20 2020 2020  .lower():..     
+00001320: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00001330: 7061 7468 203d 2073 656c 662e 6368 616e  path = self.chan
+00001340: 6765 5f70 6174 685f 6c69 6e75 785f 325f  ge_path_linux_2_
+00001350: 7769 6e28 7061 7261 6d65 7465 7273 5b22  win(parameters["
+00001360: 6677 5f70 6174 6822 5d29 0d0a 2020 2020  fw_path"])..    
+00001370: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00001380: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001390: 656d 705f 7061 7468 203d 2073 656c 662e  emp_path = self.
+000013a0: 6368 616e 6765 5f70 6174 685f 7769 6e5f  change_path_win_
+000013b0: 325f 6c69 6e75 7828 7061 7261 6d65 7465  2_linux(paramete
+000013c0: 7273 5b22 6677 5f70 6174 6822 5d29 0d0a  rs["fw_path"])..
+000013d0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000013e0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+000013f0: 7061 7468 203d 2073 656c 662e 6765 745f  path = self.get_
+00001400: 6465 6661 756c 745f 6261 7365 5f70 6174  default_base_pat
+00001410: 685f 656e 6861 6e63 6528 7061 7261 6d65  h_enhance(parame
+00001420: 7465 7273 290d 0a20 2020 2020 2020 2066  ters)..        f
+00001430: 775f 7061 7468 203d 2073 656c 662e 6765  w_path = self.ge
+00001440: 745f 6677 5f70 6174 685f 6672 6f6d 5f70  t_fw_path_from_p
+00001450: 6172 616d 6574 6572 2870 6172 616d 6574  arameter(paramet
+00001460: 6572 732c 2074 656d 705f 7061 7468 290d  ers, temp_path).
+00001470: 0a20 2020 2020 2020 2069 6620 6677 5f70  .        if fw_p
+00001480: 6174 6820 6973 206e 6f74 204e 6f6e 653a  ath is not None:
+00001490: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+000014a0: 672e 494e 464f 2822 7570 6461 7465 5f70  g.INFO("update_p
+000014b0: 6572 7365 735f 6677 5f70 6174 683a 207b  erses_fw_path: {
+000014c0: 7d22 2e66 6f72 6d61 7428 6677 5f70 6174  }".format(fw_pat
+000014d0: 6829 290d 0a20 2020 2020 2020 2020 2020  h))..           
+000014e0: 2070 6172 616d 6574 6572 735b 2266 775f   parameters["fw_
+000014f0: 7061 7468 225d 203d 2066 775f 7061 7468  path"] = fw_path
+00001500: 0d0a 2020 2020 2020 2020 2020 2020 6f73  ..            os
+00001510: 2e65 6e76 6972 6f6e 5b22 6677 5f70 6174  .environ["fw_pat
+00001520: 6822 5d20 3d20 6677 5f70 6174 680d 0a20  h"] = fw_path.. 
+00001530: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00001540: 2020 2020 2020 2020 2020 6c6f 672e 5741            log.WA
+00001550: 524e 2822 4e6f 7420 6669 6e64 2070 6174  RN("Not find pat
+00001560: 683a 2070 6572 7365 735f 6677 5f70 6174  h: perses_fw_pat
+00001570: 6822 290d 0a20 2020 2020 2020 2070 7269  h")..        pri
+00001580: 6e74 2870 6172 616d 6574 6572 7329 0d0a  nt(parameters)..
+00001590: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+000015a0: 6172 616d 6574 6572 730d 0a              arameters..
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server/utils/log.py` & `automation_rest_server-3.6.1/automation_rest_server/utils/log.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/utils/nose_xml.py` & `automation_rest_server-3.6.1/automation_rest_server/utils/nose_xml.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/utils/pip_operation.py` & `automation_rest_server-3.6.1/automation_rest_server/utils/pip_operation.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/utils/process.py` & `automation_rest_server-3.6.1/automation_rest_server/utils/process.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/utils/ssh.py` & `automation_rest_server-3.6.1/automation_rest_server/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server/utils/system.py` & `automation_rest_server-3.6.1/automation_rest_server/utils/system.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.5.9/automation_rest_server.egg-info/PKG-INFO` & `automation_rest_server-3.6.1/automation_rest_server.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation-rest-server
-Version: 3.5.9
+Version: 3.6.1
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.5.9/automation_rest_server.egg-info/SOURCES.txt` & `automation_rest_server-3.6.1/automation_rest_server.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
 automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
 automation_rest_server/test_framework/engine/__init__.py
 automation_rest_server/test_framework/engine/nose_engine.py
 automation_rest_server/test_framework/engine/oakgate_engine.py
 automation_rest_server/test_framework/engine/perses_engine.py
 automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
-automation_rest_server/test_framework/engine/perses_power_cycle_engine_old.py
 automation_rest_server/test_framework/engine/special_parameter.py
 automation_rest_server/test_framework/engine/sse_engine.py
 automation_rest_server/test_framework/firmware_engine/__init__.py
 automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
 automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
 automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
 automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
```

### Comparing `automation_rest_server-3.5.9/setup.py` & `automation_rest_server-3.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 packages = ["automation_rest_server"]
 #python setup.py sdist upload  
 #python setup.py bdist_wheel
 
 setup(
     name = 'automation_rest_server',
-    version = '3.5.9',
+    version = '3.6.1',
     keywords = ['runner', 'server'],
     description = 'NVMe production server',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
```

