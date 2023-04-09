# Comparing `tmp/gridworks_protocol-0.4.2.tar.gz` & `tmp/gridworks_protocol-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_protocol-0.4.2.tar", max compression
+gzip compressed data, was "gridworks_protocol-0.4.3.tar", max compression
```

## Comparing `gridworks_protocol-0.4.2.tar` & `gridworks_protocol-0.4.3.tar`

### file list

```diff
@@ -1,84 +1,85 @@
--rw-r--r--   0        0        0     1070 2023-04-06 21:28:19.145376 gridworks_protocol-0.4.2/LICENSE
--rw-r--r--   0        0        0     2552 2023-04-06 21:28:19.145376 gridworks_protocol-0.4.2/README.md
--rw-r--r--   0        0        0     2287 2023-04-06 21:28:30.321394 gridworks_protocol-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/__init__.py
--rw-r--r--   0        0        0     6694 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/api_types.py
--rw-r--r--   0        0        0     1152 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/boolean_actuator_cac.py
--rw-r--r--   0        0        0     1339 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/electric_meter_cac.py
--rw-r--r--   0        0        0     1488 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
--rw-r--r--   0        0        0      995 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
--rw-r--r--   0        0        0     1118 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/resistive_heater_cac.py
--rw-r--r--   0        0        0     1580 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
--rw-r--r--   0        0        0     1388 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/component.py
--rw-r--r--   0        0        0     1094 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/component_attribute_class.py
--rw-r--r--   0        0        0     1276 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/components/boolean_actuator_component.py
--rw-r--r--   0        0        0     1659 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/components/electric_meter_component.py
--rw-r--r--   0        0        0     1479 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/components/multipurpose_sensor_component.py
--rw-r--r--   0        0        0     1357 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
--rw-r--r--   0        0        0     1465 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/components/resistive_heater_component.py
--rw-r--r--   0        0        0     1308 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/components/simple_temp_sensor_component.py
--rw-r--r--   0        0        0      165 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/errors.py
--rw-r--r--   0        0        0    14778 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/hardware_layout.py
--rw-r--r--   0        0        0      273 2023-04-06 21:28:19.149376 gridworks_protocol-0.4.2/src/gwproto/data_classes/mixin.py
--rw-r--r--   0        0        0     1957 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/data_classes/sh_node.py
--rw-r--r--   0        0        0      362 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/data_classes/telemetry_tuple.py
--rw-r--r--   0        0        0    12051 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/decoders.py
--rw-r--r--   0        0        0      451 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/enums/__init__.py
--rw-r--r--   0        0        0     3462 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/enums/actor_class.py
--rw-r--r--   0        0        0     1119 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/enums/local_comm_interface.py
--rw-r--r--   0        0        0     2657 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/enums/make_model.py
--rw-r--r--   0        0        0     3480 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/enums/role.py
--rw-r--r--   0        0        0     1823 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/enums/telemetry_name.py
--rw-r--r--   0        0        0     1148 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/enums/unit.py
--rw-r--r--   0        0        0       89 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/errors.py
--rw-r--r--   0        0        0      249 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/gs/__init__.py
--rw-r--r--   0        0        0      464 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/gs/gs_dispatch.py
--rw-r--r--   0        0        0      800 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/gs/gs_dispatch_base.py
--rw-r--r--   0        0        0      678 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/gs/gs_dispatch_maker.py
--rw-r--r--   0        0        0      446 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/gs/gs_pwr.py
--rw-r--r--   0        0        0      851 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/gs/gs_pwr_base.py
--rw-r--r--   0        0        0      609 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/gs/gs_pwr_maker.py
--rw-r--r--   0        0        0     3168 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/message.py
--rw-r--r--   0        0        0     1474 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/messages/__init__.py
--rw-r--r--   0        0        0     3058 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/messages/event.py
--rw-r--r--   0        0        0      669 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/messages/misc.py
--rw-r--r--   0        0        0     4045 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/property_format.py
--rw-r--r--   0        0        0        0 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/py.typed
--rw-r--r--   0        0        0     2892 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/topic.py
--rw-r--r--   0        0        0     6756 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/__init__.py
--rw-r--r--   0        0        0     5474 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/component_attribute_class_gt.py
--rw-r--r--   0        0        0     6119 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/component_gt.py
--rw-r--r--   0        0        0    10192 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/data_channel.py
--rw-r--r--   0        0        0     3892 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/egauge_io.py
--rw-r--r--   0        0        0     3603 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/egauge_register_config.py
--rw-r--r--   0        0        0    21265 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/electric_meter_cac_gt.py
--rw-r--r--   0        0        0    13413 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/electric_meter_component_gt.py
--rw-r--r--   0        0        0    11376 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_boolean_actuator_cac.py
--rw-r--r--   0        0        0     7187 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_boolean_actuator_component.py
--rw-r--r--   0        0        0     8451 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0     5798 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_dispatch_boolean_local.py
--rw-r--r--   0        0        0     4973 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_driver_booleanactuator_cmd.py
--rw-r--r--   0        0        0     5584 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
--rw-r--r--   0        0        0     5327 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_cli_atn_cmd.py
--rw-r--r--   0        0        0    12792 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
--rw-r--r--   0        0        0    11884 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_simple_telemetry_status.py
--rw-r--r--   0        0        0    13663 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_status.py
--rw-r--r--   0        0        0    12350 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
--rw-r--r--   0        0        0     8389 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/gt_telemetry.py
--rw-r--r--   0        0        0     9471 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/heartbeat_b.py
--rw-r--r--   0        0        0    21597 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/multipurpose_sensor_cac_gt.py
--rw-r--r--   0        0        0     9935 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/multipurpose_sensor_component_gt.py
--rw-r--r--   0        0        0    11300 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/pipe_flow_sensor_cac_gt.py
--rw-r--r--   0        0        0     7622 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/pipe_flow_sensor_component_gt.py
--rw-r--r--   0        0        0     2761 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/power_watts.py
--rw-r--r--   0        0        0    11736 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/resistive_heater_cac_gt.py
--rw-r--r--   0        0        0     8096 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/resistive_heater_component_gt.py
--rw-r--r--   0        0        0    20796 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/simple_temp_sensor_cac_gt.py
--rw-r--r--   0        0        0     7280 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/simple_temp_sensor_component_gt.py
--rw-r--r--   0        0        0     6007 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/snapshot_spaceheat.py
--rw-r--r--   0        0        0    18219 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/spaceheat_node_gt.py
--rw-r--r--   0        0        0    14059 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/telemetry_reporting_config.py
--rw-r--r--   0        0        0    12227 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/types/telemetry_snapshot_spaceheat.py
--rw-r--r--   0        0        0     2556 2023-04-06 21:28:19.153376 gridworks_protocol-0.4.2/src/gwproto/utils.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.2/setup.py
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-09 21:31:14.387178 gridworks_protocol-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2552 2023-04-09 21:31:14.387178 gridworks_protocol-0.4.3/README.md
+-rw-r--r--   0        0        0     2287 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1443 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/__init__.py
+-rw-r--r--   0        0        0     6695 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/api_types.py
+-rw-r--r--   0        0        0     1152 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/boolean_actuator_cac.py
+-rw-r--r--   0        0        0     1339 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/electric_meter_cac.py
+-rw-r--r--   0        0        0     1488 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
+-rw-r--r--   0        0        0      995 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
+-rw-r--r--   0        0        0     1118 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/resistive_heater_cac.py
+-rw-r--r--   0        0        0     1580 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
+-rw-r--r--   0        0        0     1388 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/component.py
+-rw-r--r--   0        0        0     1094 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/component_attribute_class.py
+-rw-r--r--   0        0        0     1348 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/boolean_actuator_component.py
+-rw-r--r--   0        0        0     1659 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/electric_meter_component.py
+-rw-r--r--   0        0        0     1479 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/multipurpose_sensor_component.py
+-rw-r--r--   0        0        0     1357 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
+-rw-r--r--   0        0        0     1465 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/resistive_heater_component.py
+-rw-r--r--   0        0        0     1308 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/components/simple_temp_sensor_component.py
+-rw-r--r--   0        0        0      165 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/errors.py
+-rw-r--r--   0        0        0    14778 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/hardware_layout.py
+-rw-r--r--   0        0        0      273 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/mixin.py
+-rw-r--r--   0        0        0     1957 2023-04-09 21:31:14.391178 gridworks_protocol-0.4.3/src/gwproto/data_classes/sh_node.py
+-rw-r--r--   0        0        0      362 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/data_classes/telemetry_tuple.py
+-rw-r--r--   0        0        0    12051 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/decoders.py
+-rw-r--r--   0        0        0      451 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/__init__.py
+-rw-r--r--   0        0        0     3462 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/actor_class.py
+-rw-r--r--   0        0        0     1119 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/local_comm_interface.py
+-rw-r--r--   0        0        0     2657 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/make_model.py
+-rw-r--r--   0        0        0     3480 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/role.py
+-rw-r--r--   0        0        0     1823 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/telemetry_name.py
+-rw-r--r--   0        0        0     1148 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/enums/unit.py
+-rw-r--r--   0        0        0       89 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/errors.py
+-rw-r--r--   0        0        0      249 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/__init__.py
+-rw-r--r--   0        0        0      464 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch.py
+-rw-r--r--   0        0        0      800 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch_base.py
+-rw-r--r--   0        0        0      678 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch_maker.py
+-rw-r--r--   0        0        0      446 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr.py
+-rw-r--r--   0        0        0      851 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr_base.py
+-rw-r--r--   0        0        0      609 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr_maker.py
+-rw-r--r--   0        0        0     3168 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/message.py
+-rw-r--r--   0        0        0     1474 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/messages/__init__.py
+-rw-r--r--   0        0        0     3058 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/messages/event.py
+-rw-r--r--   0        0        0      669 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/messages/misc.py
+-rw-r--r--   0        0        0     4045 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/property_format.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/py.typed
+-rw-r--r--   0        0        0     2892 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/topic.py
+-rw-r--r--   0        0        0     6756 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/types/__init__.py
+-rw-r--r--   0        0        0    11376 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/types/boolean_actuator_cac_gt.py
+-rw-r--r--   0        0        0     7878 2023-04-09 21:31:26.519993 gridworks_protocol-0.4.3/src/gwproto/types/boolean_actuator_component_gt.py
+-rw-r--r--   0        0        0     5474 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/component_attribute_class_gt.py
+-rw-r--r--   0        0        0     6119 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/component_gt.py
+-rw-r--r--   0        0        0    10192 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/data_channel.py
+-rw-r--r--   0        0        0     3892 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/egauge_io.py
+-rw-r--r--   0        0        0     3603 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/egauge_register_config.py
+-rw-r--r--   0        0        0    21265 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/electric_meter_cac_gt.py
+-rw-r--r--   0        0        0    13413 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/electric_meter_component_gt.py
+-rw-r--r--   0        0        0     7187 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_boolean_actuator_component.py
+-rw-r--r--   0        0        0     8451 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0     5798 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_dispatch_boolean_local.py
+-rw-r--r--   0        0        0     4973 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_driver_booleanactuator_cmd.py
+-rw-r--r--   0        0        0     5584 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
+-rw-r--r--   0        0        0     5327 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_cli_atn_cmd.py
+-rw-r--r--   0        0        0    12792 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
+-rw-r--r--   0        0        0    11884 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_simple_telemetry_status.py
+-rw-r--r--   0        0        0    13663 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_status.py
+-rw-r--r--   0        0        0    12350 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
+-rw-r--r--   0        0        0     8389 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/gt_telemetry.py
+-rw-r--r--   0        0        0     9471 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/heartbeat_b.py
+-rw-r--r--   0        0        0    21597 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/multipurpose_sensor_cac_gt.py
+-rw-r--r--   0        0        0     9935 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/multipurpose_sensor_component_gt.py
+-rw-r--r--   0        0        0    11300 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/pipe_flow_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7622 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/pipe_flow_sensor_component_gt.py
+-rw-r--r--   0        0        0     2761 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/power_watts.py
+-rw-r--r--   0        0        0    11736 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/resistive_heater_cac_gt.py
+-rw-r--r--   0        0        0     8096 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/resistive_heater_component_gt.py
+-rw-r--r--   0        0        0    20796 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/simple_temp_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7280 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/simple_temp_sensor_component_gt.py
+-rw-r--r--   0        0        0     6007 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/snapshot_spaceheat.py
+-rw-r--r--   0        0        0    18219 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/spaceheat_node_gt.py
+-rw-r--r--   0        0        0    14059 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/telemetry_reporting_config.py
+-rw-r--r--   0        0        0    12227 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/types/telemetry_snapshot_spaceheat.py
+-rw-r--r--   0        0        0     2556 2023-04-09 21:31:14.395178 gridworks_protocol-0.4.3/src/gwproto/utils.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.3/setup.py
+-rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.3/PKG-INFO
```

### Comparing `gridworks_protocol-0.4.2/LICENSE` & `gridworks_protocol-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/README.md` & `gridworks_protocol-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/pyproject.toml` & `gridworks_protocol-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-protocol"
-version = "0.4.2"
+version = "0.4.3"
 description = "Gridworks Protocol"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-protocol"
 repository = "https://github.com/thegridelectric/gridworks-protocol"
 documentation = "https://gridworks-protocol.readthedocs.io"
```

### Comparing `gridworks_protocol-0.4.2/src/gwproto/__init__.py` & `gridworks_protocol-0.4.3/src/gwproto/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/api_types.py` & `gridworks_protocol-0.4.3/src/gwproto/api_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ List of all the types used"""
 from typing import Dict
 from typing import List
 from typing import no_type_check
 
+from gwproto.types import BooleanActuatorCacGt_Maker
+from gwproto.types import BooleanActuatorComponentGt_Maker
 from gwproto.types import ComponentAttributeClassGt_Maker
 from gwproto.types import ComponentGt_Maker
 from gwproto.types import DataChannel_Maker
 from gwproto.types import EgaugeIo_Maker
 from gwproto.types import EgaugeRegisterConfig_Maker
 from gwproto.types import ElectricMeterCacGt_Maker
 from gwproto.types import ElectricMeterComponentGt_Maker
-from gwproto.types import GtBooleanActuatorCac_Maker
-from gwproto.types import GtBooleanActuatorComponent_Maker
 from gwproto.types import GtDispatchBoolean_Maker
 from gwproto.types import GtDispatchBooleanLocal_Maker
 from gwproto.types import GtDriverBooleanactuatorCmd_Maker
 from gwproto.types import GtShBooleanactuatorCmdStatus_Maker
 from gwproto.types import GtShCliAtnCmd_Maker
 from gwproto.types import GtShMultipurposeTelemetryStatus_Maker
 from gwproto.types import GtShSimpleTelemetryStatus_Maker
@@ -40,23 +40,23 @@
 
 TypeMakerByName: Dict[str, HeartbeatB_Maker] = {}
 
 
 @no_type_check
 def type_makers() -> List[HeartbeatB_Maker]:
     return [
+        BooleanActuatorCacGt_Maker,
+        BooleanActuatorComponentGt_Maker,
         ComponentAttributeClassGt_Maker,
         ComponentGt_Maker,
         DataChannel_Maker,
         EgaugeIo_Maker,
         EgaugeRegisterConfig_Maker,
         ElectricMeterCacGt_Maker,
         ElectricMeterComponentGt_Maker,
-        GtBooleanActuatorCac_Maker,
-        GtBooleanActuatorComponent_Maker,
         GtDispatchBoolean_Maker,
         GtDispatchBooleanLocal_Maker,
         GtDriverBooleanactuatorCmd_Maker,
         GtShBooleanactuatorCmdStatus_Maker,
         GtShCliAtnCmd_Maker,
         GtShMultipurposeTelemetryStatus_Maker,
         GtShSimpleTelemetryStatus_Maker,
@@ -87,23 +87,23 @@
 def version_by_type_name() -> Dict[str, str]:
     """
     Returns:
         Dict[str, str]: Keys are TypeNames, values are versions
     """
 
     v: Dict[str, str] = {
+        "boolean.actuator.cac.gt": "000",
+        "boolean.actuator.component.gt": "000",
         "component.attribute.class.gt": "000",
         "component.gt": "000",
         "data.channel": "000",
         "egauge.io": "000",
         "egauge.register.config": "000",
         "electric.meter.cac.gt": "000",
         "electric.meter.component.gt": "000",
-        "gt.boolean.actuator.cac": "000",
-        "gt.boolean.actuator.component": "000",
         "gt.dispatch.boolean": "110",
         "gt.dispatch.boolean.local": "110",
         "gt.driver.booleanactuator.cmd": "100",
         "gt.sh.booleanactuator.cmd.status": "100",
         "gt.sh.cli.atn.cmd": "110",
         "gt.sh.multipurpose.telemetry.status": "100",
         "gt.sh.simple.telemetry.status": "100",
@@ -132,23 +132,23 @@
 def status_by_versioned_type_name() -> Dict[str, str]:
     """
     Returns:
         Dict[str, str]: Keys are versioned TypeNames, values are type status
     """
 
     v: Dict[str, str] = {
+        "boolean.actuator.cac.gt.000": "Active",
+        "boolean.actuator.component.gt.000": "Pending",
         "component.attribute.class.gt.000": "Active",
         "component.gt.000": "Active",
         "data.channel.000": "Active",
         "egauge.io.000": "Active",
         "egauge.register.config.000": "Active",
         "electric.meter.cac.gt.000": "Active",
         "electric.meter.component.gt.000": "Active",
-        "gt.boolean.actuator.cac.000": "Active",
-        "gt.boolean.actuator.component.000": "Active",
         "gt.dispatch.boolean.110": "Active",
         "gt.dispatch.boolean.local.110": "Active",
         "gt.driver.booleanactuator.cmd.100": "Active",
         "gt.sh.booleanactuator.cmd.status.100": "Active",
         "gt.sh.cli.atn.cmd.110": "Active",
         "gt.sh.multipurpose.telemetry.status.100": "Active",
         "gt.sh.simple.telemetry.status.100": "Active",
```

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/boolean_actuator_cac.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/boolean_actuator_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/electric_meter_cac.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/electric_meter_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/resistive_heater_cac.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/resistive_heater_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/component.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/component_attribute_class.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/component_attribute_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/components/boolean_actuator_component.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/boolean_actuator_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 class BooleanActuatorComponent(Component):
     by_id: Dict[str, "BooleanActuatorComponent"] = {}
 
     def __init__(
         self,
         component_id: str,
         component_attribute_class_id: str,
+        normally_open: bool,
         display_name: Optional[str] = None,
         gpio: Optional[int] = None,
         hw_uid: Optional[str] = None,
     ):
         super(self.__class__, self).__init__(
             display_name=display_name,
             component_id=component_id,
             hw_uid=hw_uid,
             component_attribute_class_id=component_attribute_class_id,
         )
+        self.normally_open = normally_open
         self.gpio = gpio
 
         BooleanActuatorComponent.by_id[self.component_id] = self
         Component.by_id[self.component_id] = self
 
     @property
     def cac(self) -> BooleanActuatorCac:
```

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/components/electric_meter_component.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/electric_meter_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/components/multipurpose_sensor_component.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/multipurpose_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/components/pipe_flow_sensor_component.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/pipe_flow_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/components/resistive_heater_component.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/resistive_heater_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/components/simple_temp_sensor_component.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/components/simple_temp_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/hardware_layout.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/hardware_layout.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/data_classes/sh_node.py` & `gridworks_protocol-0.4.3/src/gwproto/data_classes/sh_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/decoders.py` & `gridworks_protocol-0.4.3/src/gwproto/decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/enums/actor_class.py` & `gridworks_protocol-0.4.3/src/gwproto/enums/actor_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/enums/local_comm_interface.py` & `gridworks_protocol-0.4.3/src/gwproto/enums/local_comm_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/enums/make_model.py` & `gridworks_protocol-0.4.3/src/gwproto/enums/make_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/enums/role.py` & `gridworks_protocol-0.4.3/src/gwproto/enums/role.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/enums/telemetry_name.py` & `gridworks_protocol-0.4.3/src/gwproto/enums/telemetry_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/enums/unit.py` & `gridworks_protocol-0.4.3/src/gwproto/enums/unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/gs/gs_dispatch_base.py` & `gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/gs/gs_dispatch_maker.py` & `gridworks_protocol-0.4.3/src/gwproto/gs/gs_dispatch_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/gs/gs_pwr_base.py` & `gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/gs/gs_pwr_maker.py` & `gridworks_protocol-0.4.3/src/gwproto/gs/gs_pwr_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/message.py` & `gridworks_protocol-0.4.3/src/gwproto/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/messages/__init__.py` & `gridworks_protocol-0.4.3/src/gwproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/messages/event.py` & `gridworks_protocol-0.4.3/src/gwproto/messages/event.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/messages/misc.py` & `gridworks_protocol-0.4.3/src/gwproto/messages/misc.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/property_format.py` & `gridworks_protocol-0.4.3/src/gwproto/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/topic.py` & `gridworks_protocol-0.4.3/src/gwproto/topic.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/__init__.py` & `gridworks_protocol-0.4.3/src/gwproto/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """ List of all the schema types """
 
+from gwproto.types.boolean_actuator_cac_gt import BooleanActuatorCacGt
+from gwproto.types.boolean_actuator_cac_gt import BooleanActuatorCacGt_Maker
+from gwproto.types.boolean_actuator_component_gt import BooleanActuatorComponentGt
+from gwproto.types.boolean_actuator_component_gt import BooleanActuatorComponentGt_Maker
 from gwproto.types.component_attribute_class_gt import ComponentAttributeClassGt
 from gwproto.types.component_attribute_class_gt import ComponentAttributeClassGt_Maker
 from gwproto.types.component_gt import ComponentGt
 from gwproto.types.component_gt import ComponentGt_Maker
 from gwproto.types.data_channel import DataChannel
 from gwproto.types.data_channel import DataChannel_Maker
 from gwproto.types.egauge_io import EgaugeIo
 from gwproto.types.egauge_io import EgaugeIo_Maker
 from gwproto.types.egauge_register_config import EgaugeRegisterConfig
 from gwproto.types.egauge_register_config import EgaugeRegisterConfig_Maker
 from gwproto.types.electric_meter_cac_gt import ElectricMeterCacGt
 from gwproto.types.electric_meter_cac_gt import ElectricMeterCacGt_Maker
-from gwproto.types.gt_boolean_actuator_cac import GtBooleanActuatorCac
-from gwproto.types.gt_boolean_actuator_cac import GtBooleanActuatorCac_Maker
-from gwproto.types.gt_boolean_actuator_component import GtBooleanActuatorComponent
-from gwproto.types.gt_boolean_actuator_component import GtBooleanActuatorComponent_Maker
 from gwproto.types.gt_dispatch_boolean import GtDispatchBoolean
 from gwproto.types.gt_dispatch_boolean import GtDispatchBoolean_Maker
 from gwproto.types.gt_dispatch_boolean_local import GtDispatchBooleanLocal
 from gwproto.types.gt_dispatch_boolean_local import GtDispatchBooleanLocal_Maker
 from gwproto.types.gt_driver_booleanactuator_cmd import GtDriverBooleanactuatorCmd
 from gwproto.types.gt_driver_booleanactuator_cmd import GtDriverBooleanactuatorCmd_Maker
 from gwproto.types.gt_sh_booleanactuator_cmd_status import GtShBooleanactuatorCmdStatus
@@ -73,32 +73,32 @@
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig_Maker
 from gwproto.types.telemetry_snapshot_spaceheat import TelemetrySnapshotSpaceheat
 from gwproto.types.telemetry_snapshot_spaceheat import TelemetrySnapshotSpaceheat_Maker
 
 
 __all__ = [
+    "BooleanActuatorCacGt",
+    "BooleanActuatorCacGt_Maker",
+    "BooleanActuatorComponentGt",
+    "BooleanActuatorComponentGt_Maker",
     "ComponentAttributeClassGt",
     "ComponentAttributeClassGt_Maker",
     "ComponentGt",
     "ComponentGt_Maker",
     "DataChannel",
     "DataChannel_Maker",
     "EgaugeIo",
     "EgaugeIo_Maker",
     "EgaugeRegisterConfig",
     "EgaugeRegisterConfig_Maker",
     "ElectricMeterCacGt",
     "ElectricMeterCacGt_Maker",
     # "ElectricMeterComponentGt",
     # "ElectricMeterComponentGt_Maker",
-    "GtBooleanActuatorCac",
-    "GtBooleanActuatorCac_Maker",
-    "GtBooleanActuatorComponent",
-    "GtBooleanActuatorComponent_Maker",
     "GtDispatchBoolean",
     "GtDispatchBoolean_Maker",
     "GtDispatchBooleanLocal",
     "GtDispatchBooleanLocal_Maker",
     "GtDriverBooleanactuatorCmd",
     "GtDriverBooleanactuatorCmd_Maker",
     "GtShBooleanactuatorCmdStatus",
```

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/component_attribute_class_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/component_attribute_class_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/component_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/data_channel.py` & `gridworks_protocol-0.4.3/src/gwproto/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/egauge_io.py` & `gridworks_protocol-0.4.3/src/gwproto/types/egauge_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/egauge_register_config.py` & `gridworks_protocol-0.4.3/src/gwproto/types/egauge_register_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/electric_meter_cac_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/electric_meter_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/electric_meter_component_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/electric_meter_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_boolean_actuator_cac.py` & `gridworks_protocol-0.4.3/src/gwproto/types/boolean_actuator_cac_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Type gt.boolean.actuator.cac, version 000"""
+"""Type boolean.actuator.cac.gt, version 000"""
 import json
 from enum import auto
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
@@ -154,15 +154,15 @@
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
     if len(x[3]) != 4:
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
     if len(x[4]) != 12:
         raise ValueError(f"{v} word lengths not 8-4-4-4-12")
 
 
-class GtBooleanActuatorCac(BaseModel):
+class BooleanActuatorCacGt(BaseModel):
     """Type for tracking Boolean Actuator ComponentAttributeClasses.
 
     GridWorks Spaceheat SCADA uses the GridWorks GNodeRegistry structures and abstractions for managing relational device data. The Cac, or ComponentAttributeClass, is part of this structure.
     [More info](https://g-node-registry.readthedocs.io/en/latest/component-attribute-class.html).
     """
 
     ComponentAttributeClassId: str = Field(
@@ -174,15 +174,15 @@
     DisplayName: Optional[str] = Field(
         title="DisplayName",
         default=None,
     )
     TypicalResponseTimeMs: int = Field(
         title="TypicalResponseTimeMs",
     )
-    TypeName: Literal["gt.boolean.actuator.cac"] = "gt.boolean.actuator.cac"
+    TypeName: Literal["boolean.actuator.cac.gt"] = "boolean.actuator.cac.gt"
     Version: str = "000"
 
     @validator("ComponentAttributeClassId")
     def _check_component_attribute_class_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
@@ -207,55 +207,55 @@
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
     def __hash__(self):
         return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
 
 
-class GtBooleanActuatorCac_Maker:
-    type_name = "gt.boolean.actuator.cac"
+class BooleanActuatorCacGt_Maker:
+    type_name = "boolean.actuator.cac.gt"
     version = "000"
 
     def __init__(
         self,
         component_attribute_class_id: str,
         make_model: EnumMakeModel,
         display_name: Optional[str],
         typical_response_time_ms: int,
     ):
-        self.tuple = GtBooleanActuatorCac(
+        self.tuple = BooleanActuatorCacGt(
             ComponentAttributeClassId=component_attribute_class_id,
             MakeModel=make_model,
             DisplayName=display_name,
             TypicalResponseTimeMs=typical_response_time_ms,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: GtBooleanActuatorCac) -> str:
+    def tuple_to_type(cls, tuple: BooleanActuatorCacGt) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> GtBooleanActuatorCac:
+    def type_to_tuple(cls, t: str) -> BooleanActuatorCacGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise MpSchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise MpSchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> GtBooleanActuatorCac:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> BooleanActuatorCacGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "MakeModelGtEnumSymbol" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
         if d2["MakeModelGtEnumSymbol"] in SpaceheatMakeModel000SchemaEnum.symbols:
             d2["MakeModel"] = MakeModelMap.type_to_local(d2["MakeModelGtEnumSymbol"])
@@ -264,40 +264,40 @@
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "TypicalResponseTimeMs" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing TypicalResponseTimeMs")
         if "TypeName" not in d2.keys():
             raise MpSchemaError(f"dict {d2} missing TypeName")
 
-        return GtBooleanActuatorCac(
+        return BooleanActuatorCacGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             MakeModel=d2["MakeModel"],
             DisplayName=d2["DisplayName"],
             TypicalResponseTimeMs=d2["TypicalResponseTimeMs"],
             TypeName=d2["TypeName"],
             Version="000",
         )
 
     @classmethod
-    def tuple_to_dc(cls, t: GtBooleanActuatorCac) -> BooleanActuatorCac:
+    def tuple_to_dc(cls, t: BooleanActuatorCacGt) -> BooleanActuatorCac:
         if t.ComponentAttributeClassId in BooleanActuatorCac.by_id.keys():
             dc = BooleanActuatorCac.by_id[t.ComponentAttributeClassId]
         else:
             dc = BooleanActuatorCac(
                 component_attribute_class_id=t.ComponentAttributeClassId,
                 make_model=t.MakeModel,
                 display_name=t.DisplayName,
                 typical_response_time_ms=t.TypicalResponseTimeMs,
             )
 
         return dc
 
     @classmethod
-    def dc_to_tuple(cls, dc: BooleanActuatorCac) -> GtBooleanActuatorCac:
-        t = GtBooleanActuatorCac_Maker(
+    def dc_to_tuple(cls, dc: BooleanActuatorCac) -> BooleanActuatorCacGt:
+        t = BooleanActuatorCacGt_Maker(
             component_attribute_class_id=dc.component_attribute_class_id,
             make_model=dc.make_model,
             display_name=dc.display_name,
             typical_response_time_ms=dc.typical_response_time_ms,
         ).tuple
         return t
```

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_boolean_actuator_component.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_boolean_actuator_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_dispatch_boolean.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_dispatch_boolean_local.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_dispatch_boolean_local.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_driver_booleanactuator_cmd.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_driver_booleanactuator_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_cli_atn_cmd.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_cli_atn_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_simple_telemetry_status.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_simple_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_status.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/gt_telemetry.py` & `gridworks_protocol-0.4.3/src/gwproto/types/gt_telemetry.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/heartbeat_b.py` & `gridworks_protocol-0.4.3/src/gwproto/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/multipurpose_sensor_cac_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/multipurpose_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/multipurpose_sensor_component_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/multipurpose_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/pipe_flow_sensor_cac_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/pipe_flow_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/pipe_flow_sensor_component_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/pipe_flow_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/power_watts.py` & `gridworks_protocol-0.4.3/src/gwproto/types/power_watts.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/resistive_heater_cac_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/resistive_heater_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/resistive_heater_component_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/resistive_heater_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/simple_temp_sensor_cac_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/simple_temp_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/simple_temp_sensor_component_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/simple_temp_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/snapshot_spaceheat.py` & `gridworks_protocol-0.4.3/src/gwproto/types/snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/spaceheat_node_gt.py` & `gridworks_protocol-0.4.3/src/gwproto/types/spaceheat_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/telemetry_reporting_config.py` & `gridworks_protocol-0.4.3/src/gwproto/types/telemetry_reporting_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/types/telemetry_snapshot_spaceheat.py` & `gridworks_protocol-0.4.3/src/gwproto/types/telemetry_snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/src/gwproto/utils.py` & `gridworks_protocol-0.4.3/src/gwproto/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.2/setup.py` & `gridworks_protocol-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 install_requires = \
 ['fastapi-utils>=0.2.1,<0.3.0',
  'pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'gridworks-protocol',
-    'version': '0.4.2',
+    'version': '0.4.3',
     'description': 'Gridworks Protocol',
     'long_description': "# Gridworks Protocol\n\n[![PyPI](https://img.shields.io/pypi/v/gridworks-protocol.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/gridworks-protocol.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-protocol)][python version]\n[![License](https://img.shields.io/pypi/l/gridworks-protocol)][license]\n\n[![Read the documentation at https://gridworks-protocol.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-protocol/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/thegridelectric/gridworks-protocol/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-protocol/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/gridworks-protocol/\n[status]: https://pypi.org/project/gridworks-protocol/\n[python version]: https://pypi.org/project/gridworks-protocol\n[read the docs]: https://gridworks-protocol.readthedocs.io/\n[tests]: https://github.com/thegridelectric/gridworks-protocol/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-protocol\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Gridworks Protocol_ via [pip] from [PyPI]:\n\n```console\n$ pip install gridworks-protocol\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Gridworks Protocol_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/thegridelectric/gridworks-protocol/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/thegridelectric/gridworks-protocol/blob/main/LICENSE\n[contributor guide]: https://github.com/thegridelectric/gridworks-protocol/blob/main/CONTRIBUTING.md\n",
     'author': 'Jessica Millar',
     'author_email': 'jmillar@gridworks-consulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/thegridelectric/gridworks-protocol',
```

### Comparing `gridworks_protocol-0.4.2/PKG-INFO` & `gridworks_protocol-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-protocol
-Version: 0.4.2
+Version: 0.4.3
 Summary: Gridworks Protocol
 Home-page: https://github.com/thegridelectric/gridworks-protocol
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

