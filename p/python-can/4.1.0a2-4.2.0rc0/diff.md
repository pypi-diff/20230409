# Comparing `tmp/python-can-4.1.0a2.tar.gz` & `tmp/python-can-4.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-can-4.1.0a2.tar", last modified: Fri Nov 18 06:40:00 2022, max compression
+gzip compressed data, was "python-can-4.2.0rc0.tar", last modified: Sun Apr  9 18:21:46 2023, max compression
```

## Comparing `python-can-4.1.0a2.tar` & `python-can-4.2.0rc0.tar`

### file list

```diff
@@ -1,237 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.108861 python-can-4.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-11-18 06:39:50.000000 python-can-4.1.0a2/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-11-18 06:39:50.000000 python-can-4.1.0a2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-18 06:39:50.000000 python-can-4.1.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6872 2022-11-18 06:40:00.108861 python-can-4.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5060 2022-11-18 06:39:50.000000 python-can-4.1.0a2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.088860 python-can-4.1.0a2/can/
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7472 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/bit_timing.py
--rw-r--r--   0 runner    (1001) docker     (121)    10162 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/broadcastmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)    16396 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/ctypesutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6504 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.088860 python-can-4.1.0a2/can/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7619 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/canalystii.py
--rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/cantact.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.088860 python-can-4.1.0a2/can/interfaces/etas/
--rw-r--r--   0 runner    (1001) docker     (121)    11827 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/etas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20644 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/etas/boa.py
--rw-r--r--   0 runner    (1001) docker     (121)     4724 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/gs_usb.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.088860 python-can-4.1.0a2/can/interfaces/ics_neovi/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ics_neovi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17374 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ics_neovi/neovi_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     6254 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/iscan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.088860 python-can-4.1.0a2/can/interfaces/ixxat/
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ixxat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5193 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ixxat/canlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    34906 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ixxat/canlib_vcinpl.py
--rw-r--r--   0 runner    (1001) docker     (121)    38381 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ixxat/canlib_vcinpl2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9102 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ixxat/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ixxat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10533 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/ixxat/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.088860 python-can-4.1.0a2/can/interfaces/kvaser/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/kvaser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24051 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/kvaser/canlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     6904 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/kvaser/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/kvaser/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/neousys/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/neousys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7568 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/neousys/neousys.py
--rw-r--r--   0 runner    (1001) docker     (121)    11509 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/nican.py
--rw-r--r--   0 runner    (1001) docker     (121)     8725 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/nixnet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/pcan/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/pcan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40890 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/pcan/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)    23161 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/pcan/pcan.py
--rw-r--r--   0 runner    (1001) docker     (121)    15704 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/robotell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/seeedstudio/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/seeedstudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9569 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/seeedstudio/seeedstudio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/serial/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7226 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/serial/serial_can.py
--rw-r--r--   0 runner    (1001) docker     (121)    11427 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/slcan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/socketcan/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/socketcan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/socketcan/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    31607 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/socketcan/socketcan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2831 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/socketcan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/socketcand/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/socketcand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6514 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/socketcand/socketcand.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/systec/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/systec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22664 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/systec/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/systec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12820 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/systec/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)    46742 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/systec/ucan.py
--rw-r--r--   0 runner    (1001) docker     (121)    11209 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/systec/ucanbus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/udp_multicast/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/udp_multicast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16612 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/udp_multicast/bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/udp_multicast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/usb2can/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/usb2can/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/usb2can/serial_selector.py
--rw-r--r--   0 runner    (1001) docker     (121)     5529 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/usb2can/usb2canInterface.py
--rw-r--r--   0 runner    (1001) docker     (121)     6091 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/usb2can/usb2canabstractionlayer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/interfaces/vector/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39836 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/vector/canlib.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/vector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8461 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/vector/xlclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     9439 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/vector/xldefine.py
--rw-r--r--   0 runner    (1001) docker     (121)     9594 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/vector/xldriver.py
--rw-r--r--   0 runner    (1001) docker     (121)     5418 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/interfaces/virtual.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.092860 python-can-4.1.0a2/can/io/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17505 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/asc.py
--rw-r--r--   0 runner    (1001) docker     (121)    21949 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/blf.py
--rw-r--r--   0 runner    (1001) docker     (121)     6351 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/canutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3279 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    13025 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/player.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/printer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9163 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (121)    13071 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/io/trc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     1577 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/logconvert.py
--rw-r--r--   0 runner    (1001) docker     (121)     8219 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    12081 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     6660 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/notifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/player.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/thread_safe_bus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/typechecking.py
--rw-r--r--   0 runner    (1001) docker     (121)    12133 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    22255 2022-11-18 06:39:50.000000 python-can-4.1.0a2/can/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.096860 python-can-4.1.0a2/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/bcm.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/bit_timing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/bus.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5565 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5366 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/development.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/errors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3925 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.096860 python-can-4.1.0a2/doc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/canalystii.rst
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/cantact.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/etas.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     2562 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/gs_usb.rst
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/iscan.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/ixxat.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/kvaser.rst
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/neousys.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/neovi.rst
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/nican.rst
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/nixnet.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/pcan.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/robotell.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/seeedstudio.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6364 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/serial.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1055 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/slcan.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/socketcan.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/socketcand.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/systec.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/udp_multicast.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/usb2can.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/vector.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces/virtual.rst
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4782 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/internal-api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5999 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/listeners.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6127 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/message.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/plugin-interface.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8462 2022-11-18 06:39:50.000000 python-can-4.1.0a2/doc/virtual-interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-18 06:39:50.000000 python-can-4.1.0a2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.096860 python-can-4.1.0a2/python_can.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6872 2022-11-18 06:40:00.000000 python-can-4.1.0a2/python_can.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5547 2022-11-18 06:40:00.000000 python-can-4.1.0a2/python_can.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 06:40:00.000000 python-can-4.1.0a2/python_can.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-11-18 06:40:00.000000 python-can-4.1.0a2/python_can.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-18 06:40:00.000000 python-can-4.1.0a2/python_can.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-18 06:39:50.000000 python-can-4.1.0a2/requirements-lint.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.096860 python-can-4.1.0a2/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-18 06:39:50.000000 python-can-4.1.0a2/scripts/can_logconvert.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-18 06:39:50.000000 python-can-4.1.0a2/scripts/can_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-18 06:39:50.000000 python-can-4.1.0a2/scripts/can_player.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-18 06:39:50.000000 python-can-4.1.0a2/scripts/can_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-11-18 06:40:00.108861 python-can-4.1.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-11-18 06:39:50.000000 python-can-4.1.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.104861 python-can-4.1.0a2/test/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15703 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/back2back_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/contextmanager_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 06:40:00.108861 python-can-4.1.0a2/test/data/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6215 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/example_data.py
--rw-r--r--   0 runner    (1001) docker     (121)   128078 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/issue_1256.asc
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/issue_1299.asc
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/logfile.asc
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/logfile_errorframes.asc
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanErrorFrameExt.blf
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanErrorFrames.asc
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanFdMessage.asc
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanFdMessage.blf
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanFdMessage64.asc
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanFdMessage64.blf
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanFdRemoteMessage.asc
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage.asc
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage.asc.gz
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage.blf
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage.trc
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage2.blf
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage_V1_0_BUS1.trc
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage_V1_1.trc
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage_V2_0_BUS1.trc
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanMessage_V2_1.trc
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/data/test_CanRemoteMessage.asc
--rw-r--r--   0 runner    (1001) docker     (121)     5964 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/listener_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    32132 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/logformats_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/message_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3701 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/network_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/notifier_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5665 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/serial_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6647 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/simplecyclic_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_bit_timing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_cantact.py
--rw-r--r--   0 runner    (1001) docker     (121)    22484 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_cyclic_socketcan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_detect_available_configs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3583 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_interface_canalystii.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_interface_ixxat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_interface_ixxat_fd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_interface_virtual.py
--rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_kvaser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_load_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_load_file_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6426 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4782 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_message_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_message_filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)     3634 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_message_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_neousys.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_neovi.py
--rw-r--r--   0 runner    (1001) docker     (121)    14656 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_pcan.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3930 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_player.py
--rw-r--r--   0 runner    (1001) docker     (121)    24827 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_robotell.py
--rw-r--r--   0 runner    (1001) docker     (121)     9342 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_rotating_loggers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3379 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)     4235 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_slcan.py
--rw-r--r--   0 runner    (1001) docker     (121)    12340 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_socketcan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_socketcan_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_socketcan_loopback.py
--rw-r--r--   0 runner    (1001) docker     (121)     9887 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_systec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    40530 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (121)    20997 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-11-18 06:39:50.000000 python-can-4.1.0a2/test/zero_dlc_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.875723 python-can-4.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-09 18:21:46.875723 python-can-4.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.851723 python-can-4.2.0rc0/can/
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/bit_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/broadcastmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/ctypesutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.851723 python-can-4.2.0rc0/can/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/canalystii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/cantact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/etas/
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/etas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/etas/boa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/gs_usb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/ics_neovi/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ics_neovi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ics_neovi/neovi_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/iscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/ixxat/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/canlib_vcinpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38458 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/canlib_vcinpl2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/ixxat/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/kvaser/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/kvaser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24303 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/kvaser/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/kvaser/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/kvaser/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/neousys/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/neousys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/neousys/neousys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/nican.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/nixnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/pcan/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/pcan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41828 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/pcan/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/pcan/pcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/robotell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/seeedstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/seeedstudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/seeedstudio/seeedstudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/serial/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/serial/serial_can.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/slcan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/socketcan/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcan/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcan/socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.855723 python-can-4.2.0rc0/can/interfaces/socketcand/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/socketcand/socketcand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/interfaces/systec/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46740 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/ucan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/systec/ucanbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/interfaces/udp_multicast/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/udp_multicast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/udp_multicast/bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/udp_multicast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/interfaces/usb2can/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/usb2can/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/usb2can/serial_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/usb2can/usb2canInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/usb2can/usb2canabstractionlayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/interfaces/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43839 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/canlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/xlclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/xldefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/vector/xldriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/interfaces/virtual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.859723 python-can-4.2.0rc0/can/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/asc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/blf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/canutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18222 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/mf4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/io/trc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/logconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/thread_safe_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/typechecking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/can/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.863723 python-can-4.2.0rc0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/bcm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/bit_timing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/bus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.867724 python-can-4.2.0rc0/doc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/canalystii.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/cantact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/etas.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/gs_usb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/iscan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/ixxat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/kvaser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/neousys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/neovi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/nican.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/nixnet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/pcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/robotell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/seeedstudio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/serial.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1055 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/slcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/socketcan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/socketcand.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/systec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/udp_multicast.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/usb2can.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/vector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces/virtual.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/internal-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/listeners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/message.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/other-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/plugin-interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/doc/virtual-interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.867724 python-can-4.2.0rc0/python_can.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-09 18:21:46.000000 python-can-4.2.0rc0/python_can.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/requirements-lint.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.867724 python-can-4.2.0rc0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/scripts/can_logconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/scripts/can_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/scripts/can_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/scripts/can_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-09 18:21:46.875723 python-can-4.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.871724 python-can-4.2.0rc0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/back2back_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/contextmanager_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:46.875723 python-can-4.2.0rc0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128078 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/issue_1256.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/issue_1299.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/logfile.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/logfile_errorframes.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanErrorFrameExt.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanErrorFrames.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdMessage.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdMessage64.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdMessage64.blf
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanFdRemoteMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage.asc.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage.trc
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage2.blf
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage_V1_0_BUS1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage_V1_1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage_V2_0_BUS1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanMessage_V2_1.trc
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/data/test_CanRemoteMessage.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/listener_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33541 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/logformats_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/message_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/notifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/serial_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/simplecyclic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_bit_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_cantact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22230 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_cyclic_socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_detect_available_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3367 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface_canalystii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface_ixxat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface_ixxat_fd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_interface_virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_kvaser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_load_file_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_message_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_message_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_message_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_neousys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_neovi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_pcan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3930 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24830 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_robotell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_rotating_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_slcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13308 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_socketcan_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_socketcan_loopback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_systec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47118 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20951 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-09 18:21:37.000000 python-can-4.2.0rc0/test/zero_dlc_test.py
```

### Comparing `python-can-4.1.0a2/CONTRIBUTORS.txt` & `python-can-4.2.0rc0/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/LICENSE.txt` & `python-can-4.2.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/PKG-INFO` & `python-can-4.2.0rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can
-Version: 4.1.0a2
+Version: 4.2.0rc0
 Summary: Controller Area Network interface module for Python
 Home-page: https://github.com/hardbyte/python-can
 Author: python-can contributors
 License: LGPL v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,31 +34,40 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: seeedstudio
 Provides-Extra: serial
 Provides-Extra: neovi
 Provides-Extra: canalystii
 Provides-Extra: cantact
+Provides-Extra: cvector
 Provides-Extra: gs_usb
 Provides-Extra: nixnet
 Provides-Extra: pcan
+Provides-Extra: remote
+Provides-Extra: sontheim
+Provides-Extra: canine
 Provides-Extra: viewer
+Provides-Extra: mf4
 License-File: LICENSE.txt
 
 python-can
 ==========
 
-|release| |python_implementation| |downloads| |downloads_monthly| |formatter|
+|pypi| |conda| |python_implementation| |downloads| |downloads_monthly|
 
-|docs| |github-actions| |build_travis| |coverage| |mergify|
+|docs| |github-actions| |build_travis| |coverage| |mergify| |formatter|
 
-.. |release| image:: https://img.shields.io/pypi/v/python-can.svg
+.. |pypi| image:: https://img.shields.io/pypi/v/python-can.svg
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Latest Version on PyPi
 
+.. |conda| image:: https://img.shields.io/conda/v/conda-forge/python-can
+   :target: https://github.com/conda-forge/python-can-feedstock
+   :alt: Latest Version on conda-forge
+
 .. |python_implementation| image:: https://img.shields.io/pypi/implementation/python-can
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Supported Python implementations
 
 .. |downloads| image:: https://pepy.tech/badge/python-can
    :target: https://pepy.tech/project/python-can
    :alt: Downloads on PePy
@@ -71,16 +80,16 @@
    :target: https://github.com/python/black
    :alt: This project uses the black formatter.
 
 .. |docs| image:: https://readthedocs.org/projects/python-can/badge/?version=stable
    :target: https://python-can.readthedocs.io/en/stable/
    :alt: Documentation
 
-.. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/build.yml/badge.svg?branch=develop
-   :target: https://github.com/hardbyte/python-can/actions/workflows/build.yml
+.. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/hardbyte/python-can/actions/workflows/ci.yml
    :alt: Github Actions workflow status
 
 .. |build_travis| image:: https://img.shields.io/travis/hardbyte/python-can/develop.svg?label=Travis%20CI
    :target: https://app.travis-ci.com/github/hardbyte/python-can
    :alt: Travis CI Server for develop branch
 
 .. |coverage| image:: https://coveralls.io/repos/github/hardbyte/python-can/badge.svg?branch=develop
@@ -116,15 +125,15 @@
 --------
 
 - common abstractions for CAN communication
 - support for many different backends (see the `docs <https://python-can.readthedocs.io/en/stable/interfaces.html>`__)
 - receiving, sending, and periodically sending messages
 - normal and extended arbitration IDs
 - `CAN FD <https://en.wikipedia.org/wiki/CAN_FD>`__ support
-- many different loggers and readers supporting playback: ASC (CANalyzer format), BLF (Binary Logging Format by Vector), TRC, CSV, SQLite, and Canutils log
+- many different loggers and readers supporting playback: ASC (CANalyzer format), BLF (Binary Logging Format by Vector), MF4 (Measurement Data Format v4 by ASAM), TRC, CSV, SQLite, and Canutils log
 - efficient in-kernel or in-hardware filtering of messages on supported interfaces
 - bus configuration reading from a file or from environment variables
 - command line tools for working with CAN buses (see the `docs <https://python-can.readthedocs.io/en/stable/scripts.html>`__)
 - more
 
 
 Example usage
@@ -133,31 +142,32 @@
 ``pip install python-can``
 
 .. code:: python
 
     # import the library
     import can
 
-    # create a bus instance
+    # create a bus instance using 'with' statement,
+    # this will cause bus.shutdown() to be called on the block exit;
     # many other interfaces are supported as well (see documentation)
-    bus = can.Bus(interface='socketcan',
+    with can.Bus(interface='socketcan',
                   channel='vcan0',
-                  receive_own_messages=True)
+                  receive_own_messages=True) as bus:
 
-    # send a message
-    message = can.Message(arbitration_id=123, is_extended_id=True,
-                          data=[0x11, 0x22, 0x33])
-    bus.send(message, timeout=0.2)
-
-    # iterate over received messages
-    for msg in bus:
-        print(f"{msg.arbitration_id:X}: {msg.data}")
+       # send a message
+       message = can.Message(arbitration_id=123, is_extended_id=True,
+                             data=[0x11, 0x22, 0x33])
+       bus.send(message, timeout=0.2)
+
+       # iterate over received messages
+       for msg in bus:
+           print(f"{msg.arbitration_id:X}: {msg.data}")
 
-    # or use an asynchronous notifier
-    notifier = can.Notifier(bus, [can.Logger("recorded.log"), can.Printer()])
+       # or use an asynchronous notifier
+       notifier = can.Notifier(bus, [can.Logger("recorded.log"), can.Printer()])
 
 You can find more information in the documentation, online at
 `python-can.readthedocs.org <https://python-can.readthedocs.org/en/stable/>`__.
 
 
 Discussion
 ----------
```

### Comparing `python-can-4.1.0a2/README.rst` & `python-can-4.2.0rc0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 python-can
 ==========
 
-|release| |python_implementation| |downloads| |downloads_monthly| |formatter|
+|pypi| |conda| |python_implementation| |downloads| |downloads_monthly|
 
-|docs| |github-actions| |build_travis| |coverage| |mergify|
+|docs| |github-actions| |build_travis| |coverage| |mergify| |formatter|
 
-.. |release| image:: https://img.shields.io/pypi/v/python-can.svg
+.. |pypi| image:: https://img.shields.io/pypi/v/python-can.svg
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Latest Version on PyPi
 
+.. |conda| image:: https://img.shields.io/conda/v/conda-forge/python-can
+   :target: https://github.com/conda-forge/python-can-feedstock
+   :alt: Latest Version on conda-forge
+
 .. |python_implementation| image:: https://img.shields.io/pypi/implementation/python-can
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Supported Python implementations
 
 .. |downloads| image:: https://pepy.tech/badge/python-can
    :target: https://pepy.tech/project/python-can
    :alt: Downloads on PePy
@@ -25,16 +29,16 @@
    :target: https://github.com/python/black
    :alt: This project uses the black formatter.
 
 .. |docs| image:: https://readthedocs.org/projects/python-can/badge/?version=stable
    :target: https://python-can.readthedocs.io/en/stable/
    :alt: Documentation
 
-.. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/build.yml/badge.svg?branch=develop
-   :target: https://github.com/hardbyte/python-can/actions/workflows/build.yml
+.. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/hardbyte/python-can/actions/workflows/ci.yml
    :alt: Github Actions workflow status
 
 .. |build_travis| image:: https://img.shields.io/travis/hardbyte/python-can/develop.svg?label=Travis%20CI
    :target: https://app.travis-ci.com/github/hardbyte/python-can
    :alt: Travis CI Server for develop branch
 
 .. |coverage| image:: https://coveralls.io/repos/github/hardbyte/python-can/badge.svg?branch=develop
@@ -70,15 +74,15 @@
 --------
 
 - common abstractions for CAN communication
 - support for many different backends (see the `docs <https://python-can.readthedocs.io/en/stable/interfaces.html>`__)
 - receiving, sending, and periodically sending messages
 - normal and extended arbitration IDs
 - `CAN FD <https://en.wikipedia.org/wiki/CAN_FD>`__ support
-- many different loggers and readers supporting playback: ASC (CANalyzer format), BLF (Binary Logging Format by Vector), TRC, CSV, SQLite, and Canutils log
+- many different loggers and readers supporting playback: ASC (CANalyzer format), BLF (Binary Logging Format by Vector), MF4 (Measurement Data Format v4 by ASAM), TRC, CSV, SQLite, and Canutils log
 - efficient in-kernel or in-hardware filtering of messages on supported interfaces
 - bus configuration reading from a file or from environment variables
 - command line tools for working with CAN buses (see the `docs <https://python-can.readthedocs.io/en/stable/scripts.html>`__)
 - more
 
 
 Example usage
@@ -87,31 +91,32 @@
 ``pip install python-can``
 
 .. code:: python
 
     # import the library
     import can
 
-    # create a bus instance
+    # create a bus instance using 'with' statement,
+    # this will cause bus.shutdown() to be called on the block exit;
     # many other interfaces are supported as well (see documentation)
-    bus = can.Bus(interface='socketcan',
+    with can.Bus(interface='socketcan',
                   channel='vcan0',
-                  receive_own_messages=True)
+                  receive_own_messages=True) as bus:
 
-    # send a message
-    message = can.Message(arbitration_id=123, is_extended_id=True,
-                          data=[0x11, 0x22, 0x33])
-    bus.send(message, timeout=0.2)
-
-    # iterate over received messages
-    for msg in bus:
-        print(f"{msg.arbitration_id:X}: {msg.data}")
+       # send a message
+       message = can.Message(arbitration_id=123, is_extended_id=True,
+                             data=[0x11, 0x22, 0x33])
+       bus.send(message, timeout=0.2)
+
+       # iterate over received messages
+       for msg in bus:
+           print(f"{msg.arbitration_id:X}: {msg.data}")
 
-    # or use an asynchronous notifier
-    notifier = can.Notifier(bus, [can.Logger("recorded.log"), can.Printer()])
+       # or use an asynchronous notifier
+       notifier = can.Notifier(bus, [can.Logger("recorded.log"), can.Printer()])
 
 You can find more information in the documentation, online at
 `python-can.readthedocs.org <https://python-can.readthedocs.org/en/stable/>`__.
 
 
 Discussion
 ----------
```

### Comparing `python-can-4.1.0a2/can/broadcastmanager.py` & `python-can-4.2.0rc0/can/broadcastmanager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 """
 Exposes several methods for transmitting cyclic messages.
 
 The main entry point to these classes should be through
 :meth:`can.BusABC.send_periodic`.
 """
 
-from typing import Optional, Sequence, Tuple, Union, Callable, TYPE_CHECKING
+import abc
+import logging
+import sys
+import threading
+import time
+from typing import TYPE_CHECKING, Callable, Optional, Sequence, Tuple, Union
+
+from typing_extensions import Final
 
 from can import typechecking
+from can.message import Message
 
 if TYPE_CHECKING:
     from can.bus import BusABC
 
-from can.message import Message
-
-import abc
-import logging
-import threading
-import time
 
 # try to import win32event for event-based cyclic send task (needs the pywin32 package)
+USE_WINDOWS_EVENTS = False
 try:
     import win32event
 
-    HAS_EVENTS = True
+    # Python 3.11 provides a more precise sleep implementation on Windows, so this is not necessary.
+    # Put version check here, so mypy does not complain about `win32event` not being defined.
+    if sys.version_info < (3, 11):
+        USE_WINDOWS_EVENTS = True
 except ImportError:
-    HAS_EVENTS = False
+    pass
 
 log = logging.getLogger("can.bcm")
 
+NANOSECONDS_IN_SECOND: Final[int] = 1_000_000_000
+NANOSECONDS_IN_MILLISECOND: Final[int] = 1_000_000
+
 
 class CyclicTask(abc.ABC):
     """
     Abstract Base for all cyclic tasks.
     """
 
     @abc.abstractmethod
@@ -60,14 +69,15 @@
         :raises ValueError: If the given messages are invalid
         """
         messages = self._check_and_convert_messages(messages)
 
         # Take the Arbitration ID of the first element
         self.arbitration_id = messages[0].arbitration_id
         self.period = period
+        self.period_ns = int(round(period * 1e9))
         self.messages = messages
 
     @staticmethod
     def _check_and_convert_messages(
         messages: Union[Sequence[Message], Message]
     ) -> Tuple[Message, ...]:
         """Helper function to convert a Message or Sequence of messages into a
@@ -242,57 +252,72 @@
         self.stopped = True
         self.thread: Optional[threading.Thread] = None
         self.end_time: Optional[float] = (
             time.perf_counter() + duration if duration else None
         )
         self.on_error = on_error
 
-        if HAS_EVENTS:
+        if USE_WINDOWS_EVENTS:
             self.period_ms = int(round(period * 1000, 0))
-            self.event = win32event.CreateWaitableTimer(None, False, None)
+            try:
+                self.event = win32event.CreateWaitableTimerEx(
+                    None,
+                    None,
+                    win32event.CREATE_WAITABLE_TIMER_HIGH_RESOLUTION,
+                    win32event.TIMER_ALL_ACCESS,
+                )
+            except (AttributeError, OSError):
+                self.event = win32event.CreateWaitableTimer(None, False, None)
 
         self.start()
 
     def stop(self) -> None:
-        if HAS_EVENTS:
+        if USE_WINDOWS_EVENTS:
             win32event.CancelWaitableTimer(self.event.handle)
         self.stopped = True
 
     def start(self) -> None:
         self.stopped = False
         if self.thread is None or not self.thread.is_alive():
             name = f"Cyclic send task for 0x{self.messages[0].arbitration_id:X}"
             self.thread = threading.Thread(target=self._run, name=name)
             self.thread.daemon = True
 
-            if HAS_EVENTS:
+            if USE_WINDOWS_EVENTS:
                 win32event.SetWaitableTimer(
                     self.event.handle, 0, self.period_ms, None, None, False
                 )
 
             self.thread.start()
 
     def _run(self) -> None:
         msg_index = 0
+        msg_due_time_ns = time.perf_counter_ns()
+
         while not self.stopped:
             # Prevent calling bus.send from multiple threads
             with self.send_lock:
-                started = time.perf_counter()
                 try:
                     self.bus.send(self.messages[msg_index])
                 except Exception as exc:  # pylint: disable=broad-except
                     log.exception(exc)
                     if self.on_error:
                         if not self.on_error(exc):
                             break
                     else:
                         break
+            msg_due_time_ns += self.period_ns
             if self.end_time is not None and time.perf_counter() >= self.end_time:
                 break
             msg_index = (msg_index + 1) % len(self.messages)
 
-            if HAS_EVENTS:
-                win32event.WaitForSingleObject(self.event.handle, self.period_ms)
-            else:
-                # Compensate for the time it takes to send the message
-                delay = self.period - (time.perf_counter() - started)
-                time.sleep(max(0.0, delay))
+            # Compensate for the time it takes to send the message
+            delay_ns = msg_due_time_ns - time.perf_counter_ns()
+
+            if delay_ns > 0:
+                if USE_WINDOWS_EVENTS:
+                    win32event.WaitForSingleObject(
+                        self.event.handle,
+                        int(round(delay_ns / NANOSECONDS_IN_MILLISECOND)),
+                    )
+                else:
+                    time.sleep(delay_ns / NANOSECONDS_IN_SECOND)
```

### Comparing `python-can-4.1.0a2/can/bus.py` & `python-can-4.2.0rc0/can/bus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Contains the ABC bus implementation and its documentation.
 """
 
-from typing import cast, Any, Iterator, List, Optional, Sequence, Tuple, Union
-
-import can.typechecking
-
-from abc import ABC, ABCMeta, abstractmethod
-import can
+import contextlib
 import logging
 import threading
-from time import time
+from abc import ABC, ABCMeta, abstractmethod
 from enum import Enum, auto
+from time import time
+from typing import Any, Iterator, List, Optional, Sequence, Tuple, Union, cast
 
-from can.broadcastmanager import ThreadBasedCyclicSendTask, CyclicSendTaskABC
+import can
+import can.typechecking
+from can.broadcastmanager import CyclicSendTaskABC, ThreadBasedCyclicSendTask
 from can.message import Message
 
 LOG = logging.getLogger(__name__)
 
 
 class BusState(Enum):
     """The state in which a :class:`can.BusABC` can be."""
@@ -40,20 +39,22 @@
 
     #: a string describing the underlying bus and/or channel
     channel_info = "unknown"
 
     #: Log level for received messages
     RECV_LOGGING_LEVEL = 9
 
+    _is_shutdown: bool = False
+
     @abstractmethod
     def __init__(
         self,
         channel: Any,
         can_filters: Optional[can.typechecking.CanFilters] = None,
-        **kwargs: object
+        **kwargs: object,
     ):
         """Construct and open a CAN bus instance of the specified type.
 
         Subclasses should call though this method with all given parameters
         as it handles generic tasks like applying filters.
 
         :param channel:
@@ -89,15 +90,14 @@
         :raises ~can.exceptions.CanOperationError:
             If an error occurred while reading
         """
         start = time()
         time_left = timeout
 
         while True:
-
             # try to get a message
             msg, already_filtered = self._recv_internal(timeout=time_left)
 
             # return it, if it matches
             if msg and (already_filtered or self._matches_filters(msg)):
                 LOG.log(self.RECV_LOGGING_LEVEL, "Received: %s", msg)
                 return msg
@@ -105,15 +105,14 @@
             # if not, and timeout is None, try indefinitely
             elif timeout is None:
                 continue
 
             # try next one only if there still is time, and with
             # reduced timeout
             else:
-
                 time_left = timeout - (time() - start)
 
                 if time_left > 0:
                     continue
 
                 return None
 
@@ -299,27 +298,33 @@
 
         .. note::
             The result is undefined if a single task throws an exception while being stopped.
 
         :param remove_tasks:
             Stop tracking the stopped tasks.
         """
+        if not hasattr(self, "_periodic_tasks"):
+            # avoid AttributeError for partially initialized BusABC instance
+            return
+
         for task in self._periodic_tasks:
             # we cannot let `task.stop()` modify `self._periodic_tasks` while we are
             # iterating over it (#634)
             task.stop(remove_task=False)
 
         if remove_tasks:
             self._periodic_tasks.clear()
 
     def __iter__(self) -> Iterator[Message]:
         """Allow iteration on messages as they are received.
 
-            >>> for msg in bus:
-            ...     print(msg)
+        .. code-block:: python
+
+            for msg in bus:
+                print(msg)
 
 
         :yields:
             :class:`Message` msg objects.
         """
         while True:
             msg = self.recv(timeout=1.0)
@@ -348,17 +353,17 @@
         messages are matched.
 
         Calling without passing any filters will reset the applied
         filters to ``None``.
 
         :param filters:
             A iterable of dictionaries each containing a "can_id",
-            a "can_mask", and an optional "extended" key.
+            a "can_mask", and an optional "extended" key::
 
-            >>> [{"can_id": 0x11, "can_mask": 0x21, "extended": False}]
+                [{"can_id": 0x11, "can_mask": 0x21, "extended": False}]
 
             A filter matches, when
             ``<received_can_id> & can_mask == can_id & can_mask``.
             If ``extended`` is set as well, it only matches messages where
             ``<received_is_extended> == extended``. Else it matches every
             messages based only on the arbitration ID and mask.
         """
@@ -411,25 +416,39 @@
         return False
 
     def flush_tx_buffer(self) -> None:
         """Discard every message that may be queued in the output buffer(s)."""
 
     def shutdown(self) -> None:
         """
-        Called to carry out any interface specific cleanup required
-        in shutting down a bus.
+        Called to carry out any interface specific cleanup required in shutting down a bus.
+
+        This method can be safely called multiple times.
         """
+        if self._is_shutdown:
+            LOG.debug("%s is already shut down", self.__class__)
+            return
+
+        self._is_shutdown = True
         self.stop_all_periodic_tasks()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.shutdown()
 
+    def __del__(self) -> None:
+        if not self._is_shutdown:
+            LOG.warning("%s was not properly shut down", self.__class__)
+            # We do some best-effort cleanup if the user
+            # forgot to properly close the bus instance
+            with contextlib.suppress(AttributeError):
+                self.shutdown()
+
     @property
     def state(self) -> BusState:
         """
         Return the current state of the hardware
         """
         return BusState.ACTIVE
 
@@ -460,11 +479,9 @@
 
 class _SelfRemovingCyclicTask(CyclicSendTaskABC, ABC):
     """Removes itself from a bus.
 
     Only needed for typing :meth:`Bus._periodic_tasks`. Do not instantiate.
     """
 
-    def stop(  # pylint: disable=arguments-differ
-        self, remove_task: bool = True
-    ) -> None:
+    def stop(self, remove_task: bool = True) -> None:
         raise NotImplementedError()
```

### Comparing `python-can-4.1.0a2/can/ctypesutil.py` & `python-can-4.2.0rc0/can/ctypesutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # type: ignore
 """
 This module contains common `ctypes` utils.
 """
 import ctypes
 import logging
 import sys
-
 from typing import Any, Callable, Optional, Tuple, Union
 
 log = logging.getLogger("can.ctypesutil")
 
 __all__ = ["CLibrary", "HANDLE", "PHANDLE", "HRESULT"]
```

### Comparing `python-can-4.1.0a2/can/exceptions.py` & `python-can-4.2.0rc0/can/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,126 @@
-"""
-There are several specific :class:`Exception` classes to allow user
-code to react to specific scenarios related to CAN busses::
-
-    Exception (Python standard library)
-     +-- ...
-     +-- CanError (python-can)
-         +-- CanInterfaceNotImplementedError
-         +-- CanInitializationError
-         +-- CanOperationError
-         +-- CanTimeoutError
-
-Keep in mind that some functions and methods may raise different exceptions.
-For example, validating typical arguments and parameters might result in a
-:class:`ValueError`. This should always be documented for the function at hand.
-"""
-
-import sys
-from contextlib import contextmanager
-
-from typing import Optional
-from typing import Type
-
-if sys.version_info >= (3, 9):
-    from collections.abc import Generator
-else:
-    from typing import Generator
-
-
-class CanError(Exception):
-    """Base class for all CAN related exceptions.
-
-    If specified, the error code is automatically appended to the message:
-
-    >>> # With an error code (it also works with a specific error):
-    >>> error = CanOperationError(message="Failed to do the thing", error_code=42)
-    >>> str(error)
-    'Failed to do the thing [Error Code 42]'
-    >>>
-    >>> # Missing the error code:
-    >>> plain_error = CanError(message="Something went wrong ...")
-    >>> str(plain_error)
-    'Something went wrong ...'
-
-    :param error_code:
-        An optional error code to narrow down the cause of the fault
-
-    :arg error_code:
-        An optional error code to narrow down the cause of the fault
-    """
-
-    def __init__(
-        self,
-        message: str = "",
-        error_code: Optional[int] = None,
-    ) -> None:
-        self.error_code = error_code
-        super().__init__(
-            message if error_code is None else f"{message} [Error Code {error_code}]"
-        )
-
-
-class CanInterfaceNotImplementedError(CanError, NotImplementedError):
-    """Indicates that the interface is not supported on the current platform.
-
-    Example scenarios:
-      - No interface with that name exists
-      - The interface is unsupported on the current operating system or interpreter
-      - The driver could not be found or has the wrong version
-    """
-
-
-class CanInitializationError(CanError):
-    """Indicates an error the occurred while initializing a :class:`can.BusABC`.
-
-    If initialization fails due to a driver or platform missing/being unsupported,
-    a :exc:`~can.exceptions.CanInterfaceNotImplementedError` is raised instead.
-    If initialization fails due to a value being out of range, a :class:`ValueError`
-    is raised.
-
-    Example scenarios:
-      - Try to open a non-existent device and/or channel
-      - Try to use an invalid setting, which is ok by value, but not ok for the interface
-      - The device or other resources are already used
-    """
-
-
-class CanOperationError(CanError):
-    """Indicates an error while in operation.
-
-    Example scenarios:
-      - A call to a library function results in an unexpected return value
-      - An invalid message was received
-      - The driver rejected a message that was meant to be sent
-      - Cyclic redundancy check (CRC) failed
-      - A message remained unacknowledged
-      - A buffer is full
-    """
-
-
-class CanTimeoutError(CanError, TimeoutError):
-    """Indicates the timeout of an operation.
-
-    Example scenarios:
-      - Some message could not be sent after the timeout elapsed
-      - No message was read within the given time
-    """
-
-
-@contextmanager
-def error_check(
-    error_message: Optional[str] = None,
-    exception_type: Type[CanError] = CanOperationError,
-) -> Generator[None, None, None]:
-    """Catches any exceptions and turns them into the new type while preserving the stack trace."""
-    try:
-        yield
-    except Exception as error:  # pylint: disable=broad-except
-        if error_message is None:
-            raise exception_type(str(error)) from error
-        else:
-            raise exception_type(error_message) from error
+"""
+There are several specific :class:`Exception` classes to allow user
+code to react to specific scenarios related to CAN busses::
+
+    Exception (Python standard library)
+     +-- ...
+     +-- CanError (python-can)
+         +-- CanInterfaceNotImplementedError
+         +-- CanInitializationError
+         +-- CanOperationError
+         +-- CanTimeoutError
+
+Keep in mind that some functions and methods may raise different exceptions.
+For example, validating typical arguments and parameters might result in a
+:class:`ValueError`. This should always be documented for the function at hand.
+"""
+
+import sys
+from contextlib import contextmanager
+from typing import Optional, Type
+
+if sys.version_info >= (3, 9):
+    from collections.abc import Generator
+else:
+    from typing import Generator
+
+
+class CanError(Exception):
+    """Base class for all CAN related exceptions.
+
+    If specified, the error code is automatically appended to the message:
+
+    .. testsetup:: canerror
+
+        from can import CanError, CanOperationError
+
+    .. doctest:: canerror
+
+        >>> # With an error code (it also works with a specific error):
+        >>> error = CanOperationError(message="Failed to do the thing", error_code=42)
+        >>> str(error)
+        'Failed to do the thing [Error Code 42]'
+        >>>
+        >>> # Missing the error code:
+        >>> plain_error = CanError(message="Something went wrong ...")
+        >>> str(plain_error)
+        'Something went wrong ...'
+
+    :param error_code:
+        An optional error code to narrow down the cause of the fault
+
+    :arg error_code:
+        An optional error code to narrow down the cause of the fault
+    """
+
+    def __init__(
+        self,
+        message: str = "",
+        error_code: Optional[int] = None,
+    ) -> None:
+        self.error_code = error_code
+        super().__init__(
+            message if error_code is None else f"{message} [Error Code {error_code}]"
+        )
+
+
+class CanInterfaceNotImplementedError(CanError, NotImplementedError):
+    """Indicates that the interface is not supported on the current platform.
+
+    Example scenarios:
+      - No interface with that name exists
+      - The interface is unsupported on the current operating system or interpreter
+      - The driver could not be found or has the wrong version
+    """
+
+
+class CanInitializationError(CanError):
+    """Indicates an error the occurred while initializing a :class:`can.BusABC`.
+
+    If initialization fails due to a driver or platform missing/being unsupported,
+    a :exc:`~can.exceptions.CanInterfaceNotImplementedError` is raised instead.
+    If initialization fails due to a value being out of range, a :class:`ValueError`
+    is raised.
+
+    Example scenarios:
+      - Try to open a non-existent device and/or channel
+      - Try to use an invalid setting, which is ok by value, but not ok for the interface
+      - The device or other resources are already used
+    """
+
+
+class CanOperationError(CanError):
+    """Indicates an error while in operation.
+
+    Example scenarios:
+      - A call to a library function results in an unexpected return value
+      - An invalid message was received
+      - The driver rejected a message that was meant to be sent
+      - Cyclic redundancy check (CRC) failed
+      - A message remained unacknowledged
+      - A buffer is full
+    """
+
+
+class CanTimeoutError(CanError, TimeoutError):
+    """Indicates the timeout of an operation.
+
+    Example scenarios:
+      - Some message could not be sent after the timeout elapsed
+      - No message was read within the given time
+    """
+
+
+@contextmanager
+def error_check(
+    error_message: Optional[str] = None,
+    exception_type: Type[CanError] = CanOperationError,
+) -> Generator[None, None, None]:
+    """Catches any exceptions and turns them into the new type while preserving the stack trace."""
+    try:
+        yield
+    except Exception as error:  # pylint: disable=broad-except
+        if error_message is None:
+            raise exception_type(str(error)) from error
+        else:
+            raise exception_type(error_message) from error
```

### Comparing `python-can-4.1.0a2/can/interface.py` & `python-can-4.2.0rc0/can/interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 This module contains the base implementation of :class:`can.BusABC` as well
 as a list of all available backends and some implemented
 CyclicSendTasks.
 """
 
 import importlib
 import logging
-from typing import Any, cast, Iterable, Type, Optional, Union, List
+from typing import Any, Iterable, List, Optional, Type, Union, cast
 
+from . import util
 from .bus import BusABC
-from .util import load_config
-from .interfaces import BACKENDS
 from .exceptions import CanInterfaceNotImplementedError
+from .interfaces import BACKENDS
 from .typechecking import AutoDetectedConfig, Channel
 
 log = logging.getLogger("can.interface")
 log_autodetect = log.getChild("detect_available_configs")
 
 
 def _get_class_for_interface(interface: str) -> Type[BusABC]:
@@ -57,26 +57,38 @@
 
 class Bus(BusABC):  # pylint: disable=abstract-method
     """Bus wrapper with configuration loading.
 
     Instantiates a CAN Bus of the given ``interface``, falls back to reading a
     configuration file from default locations.
 
+    .. note::
+        Please note that while the arguments provided to this class take precedence
+        over any existing values from configuration, it is possible that other parameters
+        from the configuration may be added to the bus instantiation.
+        This could potentially have unintended consequences. To prevent this,
+        you may use the *ignore_config* parameter to ignore any existing configurations.
+
     :param channel:
         Channel identification. Expected type is backend dependent.
         Set to ``None`` to let it be resolved automatically from the default
         :ref:`configuration`.
 
     :param interface:
         See :ref:`interface names` for a list of supported interfaces.
         Set to ``None`` to let it be resolved automatically from the default
         :ref:`configuration`.
 
-    :param args:
-        ``interface`` specific positional arguments.
+    :param config_context:
+        Extra 'context', that is passed to config sources.
+        This can be used to select a section other than 'default' in the configuration file.
+
+    :param ignore_config:
+        If ``True``, only the given arguments will be used for the bus instantiation. Existing
+        configuration sources will be ignored.
 
     :param kwargs:
         ``interface`` specific keyword arguments.
 
     :raises ~can.exceptions.CanInterfaceNotImplementedError:
         if the ``interface`` isn't recognized or cannot be loaded
 
@@ -84,51 +96,50 @@
         if the bus cannot be instantiated
 
     :raises ValueError:
         if the ``channel`` could not be determined
     """
 
     @staticmethod
-    def __new__(  # type: ignore  # pylint: disable=keyword-arg-before-vararg
+    @util.deprecated_args_alias(
+        deprecation_start="4.2.0",
+        deprecation_end="5.0.0",
+        bustype="interface",
+        context="config_context",
+    )
+    def __new__(  # type: ignore
         cls: Any,
         channel: Optional[Channel] = None,
         interface: Optional[str] = None,
-        *args: Any,
+        config_context: Optional[str] = None,
+        ignore_config: bool = False,
         **kwargs: Any,
     ) -> BusABC:
         # figure out the rest of the configuration; this might raise an error
         if interface is not None:
             kwargs["interface"] = interface
         if channel is not None:
             kwargs["channel"] = channel
-        if "context" in kwargs:
-            context = kwargs["context"]
-            del kwargs["context"]
-        else:
-            context = None
-        kwargs = load_config(config=kwargs, context=context)
+
+        if not ignore_config:
+            kwargs = util.load_config(config=kwargs, context=config_context)
 
         # resolve the bus class to use for that interface
         cls = _get_class_for_interface(kwargs["interface"])
 
         # remove the "interface" key, so it doesn't get passed to the backend
         del kwargs["interface"]
 
         # make sure the bus can handle this config format
-        if "channel" not in kwargs:
-            raise ValueError("'channel' argument missing")
-        else:
-            channel = kwargs["channel"]
-            del kwargs["channel"]
-
+        channel = kwargs.pop("channel", channel)
         if channel is None:
             # Use the default channel for the backend
-            bus = cls(*args, **kwargs)
+            bus = cls(**kwargs)
         else:
-            bus = cls(channel, *args, **kwargs)
+            bus = cls(channel, **kwargs)
 
         return cast(BusABC, bus)
 
 
 def detect_available_configs(
     interfaces: Union[None, str, Iterable[str]] = None
 ) -> List[AutoDetectedConfig]:
@@ -156,15 +167,14 @@
         interfaces = BACKENDS
     elif isinstance(interfaces, str):
         interfaces = (interfaces,)
     # else it is supposed to be an iterable of strings
 
     result = []
     for interface in interfaces:
-
         try:
             bus_class = _get_class_for_interface(interface)
         except CanInterfaceNotImplementedError:
             log_autodetect.debug(
                 'interface "%s" cannot be loaded for detection of available configurations',
                 interface,
             )
```

### Comparing `python-can-4.1.0a2/can/interfaces/__init__.py` & `python-can-4.2.0rc0/can/interfaces/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,44 @@
 """
 Interfaces contain low level implementations that interact with CAN hardware.
 """
 
 import sys
-from typing import Dict, Tuple
+from typing import Dict, Tuple, cast
+
+__all__ = [
+    "BACKENDS",
+    "VALID_INTERFACES",
+    "canalystii",
+    "cantact",
+    "etas",
+    "gs_usb",
+    "ics_neovi",
+    "iscan",
+    "ixxat",
+    "kvaser",
+    "neousys",
+    "nican",
+    "nixnet",
+    "pcan",
+    "robotell",
+    "seeedstudio",
+    "serial",
+    "slcan",
+    "socketcan",
+    "socketcand",
+    "systec",
+    "udp_multicast",
+    "usb2can",
+    "vector",
+    "virtual",
+]
 
 # interface_name => (module, classname)
-BACKENDS: Dict[str, Tuple[str, ...]] = {
+BACKENDS: Dict[str, Tuple[str, str]] = {
     "kvaser": ("can.interfaces.kvaser", "KvaserBus"),
     "socketcan": ("can.interfaces.socketcan", "SocketcanBus"),
     "serial": ("can.interfaces.serial.serial_can", "SerialBus"),
     "pcan": ("can.interfaces.pcan", "PcanBus"),
     "usb2can": ("can.interfaces.usb2can", "Usb2canBus"),
     "ixxat": ("can.interfaces.ixxat", "IXXATBus"),
     "nican": ("can.interfaces.nican", "NicanBus"),
@@ -31,23 +59,37 @@
     "etas": ("can.interfaces.etas", "EtasBus"),
     "socketcand": ("can.interfaces.socketcand", "SocketCanDaemonBus"),
 }
 
 if sys.version_info >= (3, 8):
     from importlib.metadata import entry_points
 
-    entries = entry_points().get("can.interface", ())
-    BACKENDS.update(
-        {interface.name: tuple(interface.value.split(":")) for interface in entries}
-    )
+    # See https://docs.python.org/3/library/importlib.metadata.html#entry-points,
+    # "Compatibility Note".
+    if sys.version_info >= (3, 10):
+        BACKENDS.update(
+            {
+                interface.name: (interface.module, interface.attr)
+                for interface in entry_points(group="can.interface")
+            }
+        )
+    else:
+        # The entry_points().get(...) causes a deprecation warning on Python >= 3.10.
+        BACKENDS.update(
+            {
+                interface.name: cast(
+                    Tuple[str, str], tuple(interface.value.split(":", maxsplit=1))
+                )
+                for interface in entry_points().get("can.interface", [])
+            }
+        )
 else:
     from pkg_resources import iter_entry_points
 
-    entries = iter_entry_points("can.interface")
     BACKENDS.update(
         {
             interface.name: (interface.module_name, interface.attrs[0])
-            for interface in entries
+            for interface in iter_entry_points("can.interface")
         }
     )
 
 VALID_INTERFACES = frozenset(BACKENDS.keys())
```

### Comparing `python-can-4.1.0a2/can/interfaces/canalystii.py` & `python-can-4.2.0rc0/can/interfaces/canalystii.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,90 @@
-import collections
-from ctypes import c_ubyte
 import logging
-import canalystii as driver
 import time
-import warnings
-from typing import Any, Dict, Optional, Deque, Sequence, Tuple, Union
-from can import BitTiming, BusABC, Message
+from collections import deque
+from ctypes import c_ubyte
+from typing import Any, Deque, Dict, Optional, Sequence, Tuple, Union
+
+import canalystii as driver
+
+from can import BitTiming, BitTimingFd, BusABC, Message
 from can.exceptions import CanTimeoutError
 from can.typechecking import CanFilters
+from can.util import check_or_adjust_timing_clock, deprecated_args_alias
 
 logger = logging.getLogger(__name__)
 
 
 class CANalystIIBus(BusABC):
+    @deprecated_args_alias(
+        deprecation_start="4.2.0", deprecation_end="5.0.0", bit_timing="timing"
+    )
     def __init__(
         self,
         channel: Union[int, Sequence[int], str] = (0, 1),
         device: int = 0,
         bitrate: Optional[int] = None,
-        bit_timing: Optional[BitTiming] = None,
+        timing: Optional[Union[BitTiming, BitTimingFd]] = None,
         can_filters: Optional[CanFilters] = None,
         rx_queue_size: Optional[int] = None,
         **kwargs: Dict[str, Any],
     ):
         """
 
         :param channel:
             Optional channel number, list/tuple of multiple channels, or comma
             separated string of channels. Default is to configure both
             channels.
         :param device:
             Optional USB device number. Default is 0 (first device found).
         :param bitrate:
             CAN bitrate in bits/second. Required unless the bit_timing argument is set.
-        :param bit_timing:
-            Optional BitTiming instance to use for custom bit timing setting.
-            If this argument is set then it overrides the bitrate argument.
+        :param timing:
+            Optional :class:`~can.BitTiming` instance to use for custom bit timing setting.
+            If this argument is set then it overrides the bitrate argument. The
+            `f_clock` value of the timing instance must be set to 8_000_000 (8MHz)
+            for standard CAN.
+            CAN FD and the :class:`~can.BitTimingFd` class are not supported.
         :param can_filters:
             Optional filters for received CAN messages.
         :param rx_queue_size:
             If set, software received message queue can only grow to this many
             messages (for all channels) before older messages are dropped
         """
-        super().__init__(channel=channel, can_filters=can_filters, **kwargs)
+        if not (bitrate or timing):
+            raise ValueError("Either bitrate or timing argument is required")
 
-        if not (bitrate or bit_timing):
-            raise ValueError("Either bitrate or bit_timing argument is required")
+        # Do this after the error handling
+        super().__init__(channel=channel, can_filters=can_filters, **kwargs)
 
         if isinstance(channel, str):
             # Assume comma separated string of channels
             self.channels = [int(ch.strip()) for ch in channel.split(",")]
         elif isinstance(channel, int):
             self.channels = [channel]
         else:  # Sequence[int]
             self.channels = list(channel)
 
-        self.rx_queue = collections.deque(
-            maxlen=rx_queue_size
-        )  # type: Deque[Tuple[int, driver.Message]]
+        self.rx_queue: Deque[Tuple[int, driver.Message]] = deque(maxlen=rx_queue_size)
 
         self.channel_info = f"CANalyst-II: device {device}, channels {self.channels}"
 
         self.device = driver.CanalystDevice(device_index=device)
-        for channel in self.channels:
-            if bit_timing:
-                try:
-                    if bit_timing.f_clock != 8_000_000:
-                        warnings.warn(
-                            f"bit_timing.f_clock value {bit_timing.f_clock} "
-                            "doesn't match expected device f_clock 8MHz."
-                        )
-                except ValueError:
-                    pass  # f_clock not specified
+        for single_channel in self.channels:
+            if isinstance(timing, BitTiming):
+                timing = check_or_adjust_timing_clock(timing, valid_clocks=[8_000_000])
                 self.device.init(
-                    channel, timing0=bit_timing.btr0, timing1=bit_timing.btr1
+                    single_channel, timing0=timing.btr0, timing1=timing.btr1
+                )
+            elif isinstance(timing, BitTimingFd):
+                raise NotImplementedError(
+                    f"CAN FD is not supported by {self.__class__.__name__}."
                 )
             else:
-                self.device.init(channel, bitrate=bitrate)
+                self.device.init(single_channel, bitrate=bitrate)
 
     # Delay to use between each poll for new messages
     #
     # The timeout is deliberately kept low to avoid the possibility of
     # a hardware buffer overflow. This value was determined
     # experimentally, but the ideal value will depend on the specific
     # system.
```

### Comparing `python-can-4.1.0a2/can/interfaces/cantact.py` & `python-can-4.2.0rc0/can/interfaces/cantact.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 Interface for CANtact devices from Linklayer Labs
 """
 
-import time
 import logging
+import time
+from typing import Any, Optional, Union
 from unittest.mock import Mock
 
-from can import BusABC, Message
+from can import BitTiming, BitTimingFd, BusABC, Message
+
 from ..exceptions import (
     CanInitializationError,
     CanInterfaceNotImplementedError,
     error_check,
 )
+from ..util import check_or_adjust_timing_clock, deprecated_args_alias
 
 logger = logging.getLogger(__name__)
 
 try:
     import cantact
 except ImportError:
     cantact = None
@@ -38,64 +41,78 @@
             return []
 
         channels = []
         for i in range(0, interface.channel_count()):
             channels.append({"interface": "cantact", "channel": f"ch:{i}"})
         return channels
 
+    @deprecated_args_alias(
+        deprecation_start="4.2.0", deprecation_end="5.0.0", bit_timing="timing"
+    )
     def __init__(
         self,
-        channel,
-        bitrate=500000,
-        poll_interval=0.01,
-        monitor=False,
-        bit_timing=None,
-        _testing=False,
-        **kwargs,
-    ):
+        channel: int,
+        bitrate: int = 500_000,
+        poll_interval: float = 0.01,
+        monitor: bool = False,
+        timing: Optional[Union[BitTiming, BitTimingFd]] = None,
+        **kwargs: Any,
+    ) -> None:
         """
         :param int channel:
             Channel number (zero indexed, labeled on multi-channel devices)
         :param int bitrate:
             Bitrate in bits/s
         :param bool monitor:
             If true, operate in listen-only monitoring mode
-        :param BitTiming bit_timing:
-            Optional BitTiming to use for custom bit timing setting. Overrides bitrate if not None.
+        :param timing:
+            Optional :class:`~can.BitTiming` instance to use for custom bit timing setting.
+            If this argument is set then it overrides the bitrate argument. The
+            `f_clock` value of the timing instance must be set to 24_000_000 (24MHz)
+            for standard CAN.
+            CAN FD and the :class:`~can.BitTimingFd` class are not supported.
         """
 
-        if _testing:
+        if kwargs.get("_testing", False):
             self.interface = MockInterface()
         else:
             if cantact is None:
                 raise CanInterfaceNotImplementedError(
-                    "The CANtact module is not installed. Install it using `python -m pip install cantact`"
+                    "The CANtact module is not installed. "
+                    "Install it using `python -m pip install cantact`"
                 )
             with error_check(
                 "Cannot create the cantact.Interface", CanInitializationError
             ):
                 self.interface = cantact.Interface()
 
         self.channel = int(channel)
         self.channel_info = f"CANtact: ch:{channel}"
 
         # Configure the interface
         with error_check("Cannot setup the cantact.Interface", CanInitializationError):
-            if bit_timing is None:
-                # use bitrate
-                self.interface.set_bitrate(int(channel), int(bitrate))
-            else:
+            if isinstance(timing, BitTiming):
+                timing = check_or_adjust_timing_clock(timing, valid_clocks=[24_000_000])
+
                 # use custom bit timing
                 self.interface.set_bit_timing(
                     int(channel),
-                    int(bit_timing.brp),
-                    int(bit_timing.tseg1),
-                    int(bit_timing.tseg2),
-                    int(bit_timing.sjw),
+                    int(timing.brp),
+                    int(timing.tseg1),
+                    int(timing.tseg2),
+                    int(timing.sjw),
+                )
+            elif isinstance(timing, BitTimingFd):
+                raise NotImplementedError(
+                    f"CAN FD is not supported by {self.__class__.__name__}."
                 )
+            else:
+                # use bitrate
+                self.interface.set_bitrate(int(channel), int(bitrate))
+
             self.interface.set_enabled(int(channel), True)
             self.interface.set_monitor(int(channel), monitor)
             self.interface.start()
 
         super().__init__(
             channel=channel, bitrate=bitrate, poll_interval=poll_interval, **kwargs
         )
```

### Comparing `python-can-4.1.0a2/can/interfaces/etas/__init__.py` & `python-can-4.2.0rc0/can/interfaces/etas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ctypes
 import time
 from typing import Dict, List, Optional, Tuple
 
 import can
-from ...exceptions import CanInitializationError
+from can.exceptions import CanInitializationError
+
 from .boa import *
 
 
 class EtasBus(can.BusABC):
     def __init__(
         self,
         channel: str,
@@ -244,14 +245,15 @@
 
         OCI_AddCANFrameFilterEx(self.rxQueue, self._oci_filters, len(self._oci_filters))
 
     def flush_tx_buffer(self) -> None:
         OCI_ResetQueue(self.txQueue)
 
     def shutdown(self) -> None:
+        super().shutdown()
         # Cleanup TX
         if self.txQueue:
             OCI_DestroyCANTxQueue(self.txQueue)
             self.txQueue = None
 
         # Cleanup RX
         if self.rxQueue:
@@ -285,14 +287,15 @@
         # else:
         #     self.ctrlConf.busParticipationMode = OCI_BUSMODE_PASSIVE
         # ec = OCI_AdaptCANConfiguration(self.ctrl, ctypes.byref(self.ctrlConf))
         # if ec != 0x0:
         #     raise CanOperationError(f"OCI_AdaptCANConfiguration failed with error 0x{ec:X}")
         raise NotImplementedError("Setting state is not implemented.")
 
+    @staticmethod
     def _detect_available_configs() -> List[can.typechecking.AutoDetectedConfig]:
         nodeRange = CSI_NodeRange(CSI_NODE_MIN, CSI_NODE_MAX)
         tree = ctypes.POINTER(CSI_Tree)()
         CSI_CreateProtocolTree(ctypes.c_char_p(b""), nodeRange, ctypes.byref(tree))
 
         nodes: Dict[str, str] = []
```

### Comparing `python-can-4.1.0a2/can/interfaces/etas/boa.py` & `python-can-4.2.0rc0/can/interfaces/etas/boa.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/can/interfaces/gs_usb.py` & `python-can-4.2.0rc0/can/interfaces/gs_usb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import logging
 from typing import Optional, Tuple
 
+import usb
+from gs_usb.constants import CAN_EFF_FLAG, CAN_ERR_FLAG, CAN_MAX_DLC, CAN_RTR_FLAG
 from gs_usb.gs_usb import GsUsb
-from gs_usb.gs_usb_frame import GsUsbFrame, GS_USB_NONE_ECHO_ID
-from gs_usb.constants import CAN_ERR_FLAG, CAN_RTR_FLAG, CAN_EFF_FLAG, CAN_MAX_DLC
+from gs_usb.gs_usb_frame import GS_USB_NONE_ECHO_ID, GsUsbFrame
+
 import can
-import usb
-import logging
 
 from ..exceptions import CanInitializationError, CanOperationError
 
-
 logger = logging.getLogger(__name__)
 
 
 class GsUsbBus(can.BusABC):
     def __init__(
         self,
         channel,
```

### Comparing `python-can-4.1.0a2/can/interfaces/ics_neovi/neovi_bus.py` & `python-can-4.2.0rc0/can/interfaces/ics_neovi/neovi_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 Implementation references:
 * https://github.com/intrepidcs/python_ics
 """
 
 import logging
 import os
 import tempfile
-from collections import deque, defaultdict, Counter
+from collections import Counter, defaultdict, deque
 from itertools import cycle
 from threading import Event
 from warnings import warn
 
-from can import Message, BusABC
+from can import BusABC, Message
+
 from ...exceptions import (
     CanError,
-    CanTimeoutError,
-    CanOperationError,
     CanInitializationError,
+    CanOperationError,
+    CanTimeoutError,
 )
 
 logger = logging.getLogger(__name__)
 
 try:
     import ics
 except ImportError as ie:
@@ -36,15 +37,14 @@
     )
     ics = None
 
 
 try:
     from filelock import FileLock
 except ImportError as ie:
-
     logger.warning(
         "Using ICS neoVI can backend without the "
         "filelock module installed may cause some issues!: %s",
         ie,
     )
 
     class FileLock:
@@ -167,16 +167,16 @@
             May or may not be a :class:`~ICSInitializationError`.
         """
         if ics is None:
             raise ImportError("Please install python-ics")
 
         super().__init__(channel=channel, can_filters=can_filters, **kwargs)
 
-        logger.info("CAN Filters: {}".format(can_filters))
-        logger.info("Got configuration of: {}".format(kwargs))
+        logger.info(f"CAN Filters: {can_filters}")
+        logger.info(f"Got configuration of: {kwargs}")
 
         if "override_library_name" in kwargs:
             ics.override_library_name(kwargs.get("override_library_name"))
 
         if isinstance(channel, (list, tuple)):
             self.channels = channel
         elif isinstance(channel, int):
@@ -211,30 +211,30 @@
                 self.shutdown()
             finally:
                 raise err
 
         self._use_system_timestamp = bool(kwargs.get("use_system_timestamp", False))
         self._receive_own_messages = kwargs.get("receive_own_messages", True)
 
-        self.channel_info = "%s %s CH:%s" % (
+        self.channel_info = "{} {} CH:{}".format(
             self.dev.Name,
             self.get_serial_number(self.dev),
             self.channels,
         )
-        logger.info("Using device: {}".format(self.channel_info))
+        logger.info(f"Using device: {self.channel_info}")
 
         self.rx_buffer = deque()
         self.message_receipts = defaultdict(Event)
 
     @staticmethod
     def channel_to_netid(channel_name_or_id):
         try:
             channel = int(channel_name_or_id)
         except ValueError:
-            netid = "NETID_{}".format(channel_name_or_id.upper())
+            netid = f"NETID_{channel_name_or_id.upper()}"
             if hasattr(ics, netid):
                 channel = getattr(ics, netid)
             else:
                 raise ValueError(
                     "channel must be an integer or a valid ICS channel name"
                 ) from None
         return channel
@@ -294,17 +294,17 @@
         for device in devices:
             if serial is None or self.get_serial_number(device) == str(serial):
                 return device
         else:
             msg = ["No device"]
 
             if type_filter is not None:
-                msg.append("with type {}".format(type_filter))
+                msg.append(f"with type {type_filter}")
             if serial is not None:
-                msg.append("with serial {}".format(serial))
+                msg.append(f"with serial {serial}")
             msg.append("found.")
             raise CanInitializationError(" ".join(msg))
 
     def _process_msg_queue(self, timeout=0.1):
         try:
             messages, errors = ics.get_messages(self.dev, False, timeout)
         except ics.RuntimeError:
```

### Comparing `python-can-4.1.0a2/can/interfaces/iscan.py` & `python-can-4.2.0rc0/can/interfaces/iscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Interface for isCAN from *Thorsis Technologies GmbH*, former *ifak system GmbH*.
 """
 
 import ctypes
-import time
 import logging
+import time
 from typing import Optional, Tuple, Union
 
-from can import BusABC, Message
 from can import (
+    BusABC,
     CanError,
-    CanInterfaceNotImplementedError,
     CanInitializationError,
+    CanInterfaceNotImplementedError,
     CanOperationError,
+    Message,
 )
 
 logger = logging.getLogger(__name__)
 
 CanData = ctypes.c_ubyte * 8
 
 
@@ -153,15 +154,14 @@
 
     def shutdown(self) -> None:
         super().shutdown()
         iscan.isCAN_CloseDevice(self.channel)
 
 
 class IscanError(CanError):
-
     ERROR_CODES = {
         0: "Success",
         1: "No access to device",
         2: "Device with ID not found",
         3: "Driver operation failed",
         4: "Invalid parameter",
         5: "Operation allowed only in online state",
```

### Comparing `python-can-4.1.0a2/can/interfaces/ixxat/canlib.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/canlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+from typing import Optional
+
 import can.interfaces.ixxat.canlib_vcinpl as vcinpl
 import can.interfaces.ixxat.canlib_vcinpl2 as vcinpl2
-
 from can import BusABC, Message
 from can.bus import BusState
 
-from typing import Optional
-
 
 class IXXATBus(BusABC):
     """The CAN Bus implemented for the IXXAT interface.
 
     Based on the C implementation of IXXAT, two different dlls are provided by IXXAT, one to work with CAN,
     the other with CAN-FD.
 
@@ -142,19 +141,17 @@
 
     def send(self, msg: Message, timeout: Optional[float] = None) -> None:
         return self.bus.send(msg, timeout)
 
     def _send_periodic_internal(self, msgs, period, duration=None):
         return self.bus._send_periodic_internal(msgs, period, duration)
 
-    def shutdown(self):
-        return self.bus.shutdown()
+    def shutdown(self) -> None:
+        super().shutdown()
+        self.bus.shutdown()
 
     @property
     def state(self) -> BusState:
         """
         Return the current state of the hardware
         """
         return self.bus.state
-
-
-# ~class IXXATBus(BusABC): ---------------------------------------------------
```

### Comparing `python-can-4.1.0a2/can/interfaces/ixxat/canlib_vcinpl.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/canlib_vcinpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 
 """
 
 import ctypes
 import functools
 import logging
 import sys
-from typing import Optional, Callable, Tuple
+from typing import Callable, Optional, Tuple
 
 from can import BusABC, Message
-from can.bus import BusState
-from can.exceptions import CanInterfaceNotImplementedError, CanInitializationError
 from can.broadcastmanager import (
     LimitedDurationCyclicSendTaskABC,
     RestartableCyclicTaskABC,
 )
-from can.ctypesutil import CLibrary, HANDLE, PHANDLE, HRESULT as ctypes_HRESULT
+from can.bus import BusState
+from can.ctypesutil import HANDLE, PHANDLE, CLibrary
+from can.ctypesutil import HRESULT as ctypes_HRESULT
+from can.exceptions import CanInitializationError, CanInterfaceNotImplementedError
 from can.util import deprecated_args_alias
 
 from . import constants, structures
 from .exceptions import *
 
 __all__ = [
     "VCITimeout",
@@ -115,15 +116,15 @@
             :class:VCIError
     """
     if isinstance(result, int):
         # Real return value is an unsigned long, the following line converts the number to unsigned
         result = ctypes.c_ulong(result).value
 
     if result == constants.VCI_E_TIMEOUT:
-        raise VCITimeout("Function {} timed out".format(function._name))
+        raise VCITimeout(f"Function {function._name} timed out")
     elif result == constants.VCI_E_RXQUEUE_EMPTY:
         raise VCIRxQueueEmptyError()
     elif result == constants.VCI_E_NO_MORE_ITEMS:
         raise StopIteration()
     elif result == constants.VCI_E_ACCESSDENIED:
         pass  # not a real error, might happen if another program has initialized the bus
     elif result != constants.VCI_OK:
@@ -413,14 +414,16 @@
             667000: constants.CAN_BT1_667KB,
             800000: constants.CAN_BT1_800KB,
             1000000: constants.CAN_BT1_1000KB,
         },
     }
 
     @deprecated_args_alias(
+        deprecation_start="4.0.0",
+        deprecation_end="5.0.0",
         UniqueHardwareId="unique_hardware_id",
         rxFifoSize="rx_fifo_size",
         txFifoSize="tx_fifo_size",
     )
     def __init__(
         self,
         channel: int,
@@ -465,15 +468,15 @@
         log.info("CAN Filters: %s", can_filters)
         # Configuration options
         self._receive_own_messages = receive_own_messages
         # Usually comes as a string from the config file
         channel = int(channel)
 
         if bitrate not in self.CHANNEL_BITRATES[0]:
-            raise ValueError("Invalid bitrate {}".format(bitrate))
+            raise ValueError(f"Invalid bitrate {bitrate}")
 
         if rx_fifo_size <= 0:
             raise ValueError("rx_fifo_size must be > 0")
 
         if tx_fifo_size <= 0:
             raise ValueError("tx_fifo_size must be > 0")
 
@@ -883,15 +886,15 @@
     states = []
     for flag, description in CAN_STATUS_FLAGS.items():
         if status_flags & flag:
             states.append(description)
             status_flags &= ~flag
 
     if status_flags:
-        states.append("unknown state 0x{:02x}".format(status_flags))
+        states.append(f"unknown state 0x{status_flags:02x}")
 
     if states:
         return "CAN status message: {}".format(", ".join(states))
     else:
         return "Empty CAN status message"
```

### Comparing `python-can-4.1.0a2/can/interfaces/ixxat/canlib_vcinpl2.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/canlib_vcinpl2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 """
 
 import ctypes
 import functools
 import logging
 import sys
-from typing import Optional, Callable, Tuple
+from typing import Callable, Optional, Tuple
 
+import can.util
 from can import BusABC, Message
-from can.exceptions import CanInterfaceNotImplementedError, CanInitializationError
 from can.broadcastmanager import (
     LimitedDurationCyclicSendTaskABC,
     RestartableCyclicTaskABC,
 )
-from can.ctypesutil import CLibrary, HANDLE, PHANDLE, HRESULT as ctypes_HRESULT
-
-import can.util
+from can.ctypesutil import HANDLE, PHANDLE, CLibrary
+from can.ctypesutil import HRESULT as ctypes_HRESULT
+from can.exceptions import CanInitializationError, CanInterfaceNotImplementedError
 from can.util import deprecated_args_alias
 
 from . import constants, structures
 from .exceptions import *
 
 __all__ = [
     "VCITimeout",
@@ -113,15 +113,15 @@
         :raise:
             :class:VCITimeout
             :class:VCIRxQueueEmptyError
             :class:StopIteration
             :class:VCIError
     """
     if result == constants.VCI_E_TIMEOUT:
-        raise VCITimeout("Function {} timed out".format(function._name))
+        raise VCITimeout(f"Function {function._name} timed out")
     elif result == constants.VCI_E_RXQUEUE_EMPTY:
         raise VCIRxQueueEmptyError()
     elif result == constants.VCI_E_NO_MORE_ITEMS:
         raise StopIteration()
     elif result == constants.VCI_E_ACCESSDENIED:
         pass  # not a real error, might happen if another program has initialized the bus
     elif result != constants.VCI_OK:
@@ -413,14 +413,16 @@
         This interface does implement efficient filtering of messages, but
         the filters have to be set in ``__init__`` using the ``can_filters`` parameter.
         Using :meth:`~can.BusABC.set_filters` does not work.
 
     """
 
     @deprecated_args_alias(
+        deprecation_start="4.0.0",
+        deprecation_end="5.0.0",
         UniqueHardwareId="unique_hardware_id",
         rxFifoSize="rx_fifo_size",
         txFifoSize="tx_fifo_size",
     )
     def __init__(
         self,
         channel: int,
@@ -1007,15 +1009,15 @@
     states = []
     for flag, description in CAN_STATUS_FLAGS.items():
         if status_flags & flag:
             states.append(description)
             status_flags &= ~flag
 
     if status_flags:
-        states.append("unknown state 0x{:02x}".format(status_flags))
+        states.append(f"unknown state 0x{status_flags:02x}")
 
     if states:
         return "CAN status message: {}".format(", ".join(states))
     else:
         return "Empty CAN status message"
```

### Comparing `python-can-4.1.0a2/can/interfaces/ixxat/constants.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/can/interfaces/ixxat/exceptions.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/can/interfaces/ixxat/structures.py` & `python-can-4.2.0rc0/can/interfaces/ixxat/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         # CAN ID of the message in Intel format (aligned right) without RTR bit.
         ("dwMsgId", ctypes.c_uint32),
         ("uMsgInfo", CANMSGINFO),
         ("abData", ctypes.c_uint8 * 8),
     ]
 
     def __str__(self) -> str:
-        return """ID: 0x{0:04x}{1} DLC: {2:02d} DATA: {3}""".format(
+        return """ID: 0x{:04x}{} DLC: {:02d} DATA: {}""".format(
             self.dwMsgId,
             "[RTR]" if self.uMsgInfo.Bits.rtr else "",
             self.uMsgInfo.Bits.dlc,
             memoryview(self.abData)[: self.uMsgInfo.Bits.dlc].hex(sep=" "),
         )
```

### Comparing `python-can-4.1.0a2/can/interfaces/kvaser/canlib.py` & `python-can-4.2.0rc0/can/interfaces/kvaser/canlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Contains Python equivalents of the function and constant
 definitions in CANLIB's canlib.h, with some supporting functionality
 specific to Python.
 
 Copyright (C) 2010 Dynamic Controls
 """
 
+import ctypes
+import logging
 import sys
 import time
-import logging
-import ctypes
 
-from can import BusABC
-from ...exceptions import CanError, CanInitializationError, CanOperationError
-from can import Message
+from can import BusABC, Message
 from can.util import time_perfcounter_correlation
+
+from ...exceptions import CanError, CanInitializationError, CanOperationError
 from . import constants as canstat
 from . import structures
 
 log = logging.getLogger("can.kvaser")
 
 # Resolution in us
 TIMESTAMP_RESOLUTION = 10
@@ -406,16 +406,16 @@
             If CAN-FD frames should be supported.
         :param int data_bitrate:
             Which bitrate to use for data phase in CAN FD.
             Defaults to arbitration bitrate.
 
         """
 
-        log.info("CAN Filters: {}".format(can_filters))
-        log.info("Got configuration of: {}".format(kwargs))
+        log.info(f"CAN Filters: {can_filters}")
+        log.info(f"Got configuration of: {kwargs}")
         bitrate = kwargs.get("bitrate", 500000)
         tseg1 = kwargs.get("tseg1", 0)
         tseg2 = kwargs.get("tseg2", 0)
         sjw = kwargs.get("sjw", 0)
         no_samp = kwargs.get("no_samp", 0)
         driver_mode = kwargs.get("driver_mode", DRIVER_MODE_NORMAL)
         single_handle = kwargs.get("single_handle", False)
@@ -658,17 +658,26 @@
         canClose(self._write_handle)
 
     def get_stats(self) -> structures.BusStatistics:
         """Retrieves the bus statistics.
 
         Use like so:
 
-        >>> stats = bus.get_stats()
-        >>> print(stats)
-        std_data: 0, std_remote: 0, ext_data: 0, ext_remote: 0, err_frame: 0, bus_load: 0.0%, overruns: 0
+        .. testsetup:: kvaser
+
+            from unittest.mock import Mock
+            from can.interfaces.kvaser.structures import BusStatistics
+            bus = Mock()
+            bus.get_stats = Mock(side_effect=lambda: BusStatistics())
+
+        .. doctest:: kvaser
+
+            >>> stats = bus.get_stats()
+            >>> print(stats)
+            std_data: 0, std_remote: 0, ext_data: 0, ext_remote: 0, err_frame: 0, bus_load: 0.0%, overruns: 0
 
         :returns: bus statistics.
         """
         canRequestBusStatistics(self._write_handle)
         stats = structures.BusStatistics()
         canGetBusStatistics(
             self._write_handle, ctypes.pointer(stats), ctypes.sizeof(stats)
```

### Comparing `python-can-4.1.0a2/can/interfaces/kvaser/constants.py` & `python-can-4.2.0rc0/can/interfaces/kvaser/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/can/interfaces/kvaser/structures.py` & `python-can-4.2.0rc0/can/interfaces/kvaser/structures.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/can/interfaces/neousys/neousys.py` & `python-can-4.2.0rc0/can/interfaces/neousys/neousys.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,43 +10,42 @@
 # with Windows but you have to replace with correct named DLL
 #
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=wrong-import-position
 
-import queue
 import logging
 import platform
-from time import time
-
+import queue
 from ctypes import (
-    byref,
     CFUNCTYPE,
+    POINTER,
+    Structure,
+    byref,
     c_ubyte,
     c_uint,
     c_ushort,
-    POINTER,
     sizeof,
-    Structure,
 )
+from time import time
 
 try:
     from ctypes import WinDLL
 except ImportError:
     from ctypes import CDLL
 
 from can import BusABC, Message
+
 from ...exceptions import (
     CanInitializationError,
-    CanOperationError,
     CanInterfaceNotImplementedError,
+    CanOperationError,
 )
 
-
 logger = logging.getLogger(__name__)
 
 
 class NeousysCanSetup(Structure):
     """C CAN Setup struct"""
 
     _fields_ = [
```

### Comparing `python-can-4.1.0a2/can/interfaces/nican.py` & `python-can-4.2.0rc0/can/interfaces/nican.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,25 @@
       See also the IXXAT interface.
 
 """
 
 import ctypes
 import logging
 import sys
+from typing import Optional, Tuple, Type
 
-from can import BusABC, Message
 import can.typechecking
+from can import BusABC, Message
+
 from ..exceptions import (
     CanError,
+    CanInitializationError,
     CanInterfaceNotImplementedError,
     CanOperationError,
-    CanInitializationError,
 )
-from typing import Optional, Tuple, Type
-
 
 logger = logging.getLogger(__name__)
 
 NC_SUCCESS = 0
 NC_ERR_TIMEOUT = 1
 TIMEOUT_ERROR_CODE = -1074388991
```

### Comparing `python-can-4.1.0a2/can/interfaces/pcan/basic.py` & `python-can-4.2.0rc0/can/interfaces/pcan/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 #
 #  PCAN-Basic API
 #
 #  ~~~~~~~~~~~~
 #
 #  ------------------------------------------------------------------
 #  Author : Keneth Wagner
+#  Last change: 2022-07-06
 #  ------------------------------------------------------------------
 #
-#  Copyright (C) 1999-2021  PEAK-System Technik GmbH, Darmstadt
+#  Copyright (C) 1999-2022  PEAK-System Technik GmbH, Darmstadt
 #  more Info at http://www.peak-system.com
 
 # Module Imports
+import logging
+import platform
 from ctypes import *
 from ctypes.util import find_library
-from string import *
-import platform
 
-import logging
+PLATFORM = platform.system()
+IS_WINDOWS = PLATFORM == "Windows"
+IS_LINUX = PLATFORM == "Linux"
 
-if platform.system() == "Windows":
+if IS_WINDOWS:
     import winreg
 
-
 logger = logging.getLogger("can.pcan")
 
 # ///////////////////////////////////////////////////////////
 # Type definitions
 # ///////////////////////////////////////////////////////////
 
 TPCANHandle = c_ushort  # Represents a PCAN hardware channel handle
@@ -278,14 +280,20 @@
 )  # Get the version of the firmware used by the device associated with a PCAN-Channel
 PCAN_ATTACHED_CHANNELS_COUNT = TPCANParameter(
     0x2A
 )  # Get the amount of PCAN channels attached to a system
 PCAN_ATTACHED_CHANNELS = TPCANParameter(
     0x2B
 )  # Get information about PCAN channels attached to a system
+PCAN_ALLOW_ECHO_FRAMES = TPCANParameter(
+    0x2C
+)  # Echo messages reception status within a PCAN-Channel
+PCAN_DEVICE_PART_NUMBER = TPCANParameter(
+    0x2D
+)  # Get the part number associated to a device
 
 # DEPRECATED parameters
 #
 PCAN_DEVICE_NUMBER = PCAN_DEVICE_ID  # DEPRECATED. Use PCAN_DEVICE_ID instead
 
 # PCAN parameter values
 #
@@ -350,16 +358,16 @@
 
 # Other constants
 #
 MAX_LENGTH_HARDWARE_NAME = int(
     33
 )  # Maximum length of the name of a device: 32 characters + terminator
 MAX_LENGTH_VERSION_STRING = int(
-    18
-)  # Maximum length of a version string: 17 characters + terminator
+    256
+)  # Maximum length of a version string: 255 characters + terminator
 
 # PCAN message types
 #
 PCAN_MESSAGE_STANDARD = TPCANMessageType(
     0x00
 )  # The PCAN message is a CAN Standard Frame (11-bit identifier)
 PCAN_MESSAGE_RTR = TPCANMessageType(
@@ -373,14 +381,17 @@
 )  # The PCAN message represents a FD frame in terms of CiA Specs
 PCAN_MESSAGE_BRS = TPCANMessageType(
     0x08
 )  # The PCAN message represents a FD bit rate switch (CAN data at a higher bit rate)
 PCAN_MESSAGE_ESI = TPCANMessageType(
     0x10
 )  # The PCAN message represents a FD error state indicator(CAN FD transmitter was error active)
+PCAN_MESSAGE_ECHO = TPCANMessageType(
+    0x20
+)  # The PCAN message represents an echo CAN Frame
 PCAN_MESSAGE_ERRFRAME = TPCANMessageType(
     0x40
 )  # The PCAN message represents an error frame
 PCAN_MESSAGE_STATUS = TPCANMessageType(
     0x80
 )  # The PCAN message represents a PCAN status message
 
@@ -639,63 +650,79 @@
     "PCAN_LANBUS12": PCAN_LANBUS12,
     "PCAN_LANBUS13": PCAN_LANBUS13,
     "PCAN_LANBUS14": PCAN_LANBUS14,
     "PCAN_LANBUS15": PCAN_LANBUS15,
     "PCAN_LANBUS16": PCAN_LANBUS16,
 }
 
+VALID_PCAN_CAN_CLOCKS = [8_000_000]
+
+VALID_PCAN_FD_CLOCKS = [
+    20_000_000,
+    24_000_000,
+    30_000_000,
+    40_000_000,
+    60_000_000,
+    80_000_000,
+]
 
 # ///////////////////////////////////////////////////////////
 # PCAN-Basic API function declarations
 # ///////////////////////////////////////////////////////////
 
+
 # PCAN-Basic API class implementation
 #
 class PCANBasic:
     """PCAN-Basic API class implementation"""
 
     def __init__(self):
-        # Loads the PCANBasic API
-        #
         if platform.system() == "Windows":
-            # Loads the API on Windows
-            self.__m_dllBasic = windll.LoadLibrary("PCANBasic")
-            aReg = winreg.ConnectRegistry(None, winreg.HKEY_LOCAL_MACHINE)
-            try:
-                aKey = winreg.OpenKey(aReg, r"SOFTWARE\PEAK-System\PEAK-Drivers")
-                winreg.CloseKey(aKey)
-            except WindowsError:
-                logger.error("Exception: The PEAK-driver couldn't be found!")
-            finally:
-                winreg.CloseKey(aReg)
-        elif "CYGWIN" in platform.system():
-            self.__m_dllBasic = cdll.LoadLibrary("PCANBasic.dll")
-            # Unfortunately cygwin python has no winreg module, so we can't
-            # check for the registry key.
-        elif platform.system() == "Linux":
-            # Loads the API on Linux
-            self.__m_dllBasic = cdll.LoadLibrary("libpcanbasic.so")
+            load_library_func = windll.LoadLibrary
+
+            # look for Peak drivers in Windows registry
+            with winreg.ConnectRegistry(None, winreg.HKEY_LOCAL_MACHINE) as reg:
+                try:
+                    with winreg.OpenKey(reg, r"SOFTWARE\PEAK-System\PEAK-Drivers"):
+                        pass
+                except OSError:
+                    raise OSError("The PEAK-driver could not be found!") from None
+        else:
+            load_library_func = cdll.LoadLibrary
+
+        if platform.system() == "Windows" or "CYGWIN" in platform.system():
+            lib_name = "PCANBasic.dll"
         elif platform.system() == "Darwin":
-            self.__m_dllBasic = cdll.LoadLibrary(find_library("libPCBUSB.dylib"))
+            # PCBUSB library is a third-party software created
+            # and maintained by the MacCAN project
+            lib_name = "libPCBUSB.dylib"
         else:
-            self.__m_dllBasic = cdll.LoadLibrary("libpcanbasic.so")
-        if self.__m_dllBasic is None:
-            logger.error("Exception: The PCAN-Basic DLL couldn't be loaded!")
+            lib_name = "libpcanbasic.so"
+
+        lib_path = find_library(lib_name)
+        if not lib_path:
+            raise OSError(f"{lib_name} library not found.")
+
+        try:
+            self.__m_dllBasic = load_library_func(lib_path)
+        except OSError:
+            raise OSError(
+                f"The PCAN-Basic API could not be loaded. ({lib_path})"
+            ) from None
 
     # Initializes a PCAN Channel
     #
     def Initialize(
         self,
         Channel,
         Btr0Btr1,
         HwType=TPCANType(0),
         IOPort=c_uint(0),
         Interrupt=c_ushort(0),
     ):
-
         """Initializes a PCAN Channel
 
         Parameters:
           Channel  : A TPCANHandle representing a PCAN Channel
           Btr0Btr1 : The speed for the communication (BTR0BTR1 code)
           HwType   : Non-PnP: The type of hardware and operation mode
           IOPort   : Non-PnP: The I/O address for the parallel port
@@ -712,15 +739,14 @@
         except:
             logger.error("Exception on PCANBasic.Initialize")
             raise
 
     # Initializes a FD capable PCAN Channel
     #
     def InitializeFD(self, Channel, BitrateFD):
-
         """Initializes a FD capable PCAN Channel
 
         Parameters:
           Channel  : The handle of a FD capable PCAN Channel
           BitrateFD : The speed for the communication (FD bit rate string)
 
         Remarks:
@@ -743,15 +769,14 @@
         except:
             logger.error("Exception on PCANBasic.InitializeFD")
             raise
 
     #  Uninitializes one or all PCAN Channels initialized by CAN_Initialize
     #
     def Uninitialize(self, Channel):
-
         """Uninitializes one or all PCAN Channels initialized by CAN_Initialize
 
         Remarks:
           Giving the TPCANHandle value "PCAN_NONEBUS", uninitialize all initialized channels
 
         Parameters:
           Channel  : A TPCANHandle representing a PCAN Channel
@@ -765,15 +790,14 @@
         except:
             logger.error("Exception on PCANBasic.Uninitialize")
             raise
 
     #  Resets the receive and transmit queues of the PCAN Channel
     #
     def Reset(self, Channel):
-
         """Resets the receive and transmit queues of the PCAN Channel
 
         Remarks:
           A reset of the CAN controller is not performed
 
         Parameters:
           Channel  : A TPCANHandle representing a PCAN Channel
@@ -787,15 +811,14 @@
         except:
             logger.error("Exception on PCANBasic.Reset")
             raise
 
     #  Gets the current status of a PCAN Channel
     #
     def GetStatus(self, Channel):
-
         """Gets the current status of a PCAN Channel
 
         Parameters:
           Channel  : A TPCANHandle representing a PCAN Channel
 
         Returns:
           A TPCANStatus error code
@@ -806,15 +829,14 @@
         except:
             logger.error("Exception on PCANBasic.GetStatus")
             raise
 
     # Reads a CAN message from the receive queue of a PCAN Channel
     #
     def Read(self, Channel):
-
         """Reads a CAN message from the receive queue of a PCAN Channel
 
         Remarks:
           The return value of this method is a 3-tuple, where
           the first value is the result (TPCANStatus) of the method.
           The order of the values are:
           [0]: A TPCANStatus error code
@@ -835,15 +857,14 @@
         except:
             logger.error("Exception on PCANBasic.Read")
             raise
 
     # Reads a CAN message from the receive queue of a FD capable PCAN Channel
     #
     def ReadFD(self, Channel):
-
         """Reads a CAN message from the receive queue of a FD capable PCAN Channel
 
         Remarks:
           The return value of this method is a 3-tuple, where
           the first value is the result (TPCANStatus) of the method.
           The order of the values are:
           [0]: A TPCANStatus error code
@@ -864,15 +885,14 @@
         except:
             logger.error("Exception on PCANBasic.ReadFD")
             raise
 
     # Transmits a CAN message
     #
     def Write(self, Channel, MessageBuffer):
-
         """Transmits a CAN message
 
         Parameters:
           Channel      : A TPCANHandle representing a PCAN Channel
           MessageBuffer: A TPCANMsg representing the CAN message to be sent
 
         Returns:
@@ -884,15 +904,14 @@
         except:
             logger.error("Exception on PCANBasic.Write")
             raise
 
     # Transmits a CAN message over a FD capable PCAN Channel
     #
     def WriteFD(self, Channel, MessageBuffer):
-
         """Transmits a CAN message over a FD capable PCAN Channel
 
         Parameters:
           Channel      : The handle of a FD capable PCAN Channel
           MessageBuffer: A TPCANMsgFD buffer with the message to be sent
 
         Returns:
@@ -904,15 +923,14 @@
         except:
             logger.error("Exception on PCANBasic.WriteFD")
             raise
 
     # Configures the reception filter
     #
     def FilterMessages(self, Channel, FromID, ToID, Mode):
-
         """Configures the reception filter
 
         Remarks:
           The message filter will be expanded with every call to this function.
           If it is desired to reset the filter, please use the 'SetValue' function.
 
         Parameters:
@@ -931,15 +949,14 @@
         except:
             logger.error("Exception on PCANBasic.FilterMessages")
             raise
 
     # Retrieves a PCAN Channel value
     #
     def GetValue(self, Channel, Parameter):
-
         """Retrieves a PCAN Channel value
 
         Remarks:
           Parameters can be present or not according with the kind
           of Hardware (PCAN Channel) being used. If a parameter is not available,
           a PCAN_ERROR_ILLPARAMTYPE error will be returned.
 
@@ -960,23 +977,30 @@
                 or Parameter == PCAN_HARDWARE_NAME
                 or Parameter == PCAN_CHANNEL_VERSION
                 or Parameter == PCAN_LOG_LOCATION
                 or Parameter == PCAN_TRACE_LOCATION
                 or Parameter == PCAN_BITRATE_INFO_FD
                 or Parameter == PCAN_IP_ADDRESS
                 or Parameter == PCAN_FIRMWARE_VERSION
+                or Parameter == PCAN_DEVICE_PART_NUMBER
             ):
                 mybuffer = create_string_buffer(256)
 
             elif Parameter == PCAN_ATTACHED_CHANNELS:
                 res = self.GetValue(Channel, PCAN_ATTACHED_CHANNELS_COUNT)
                 if TPCANStatus(res[0]) != PCAN_ERROR_OK:
                     return (TPCANStatus(res[0]),)
                 mybuffer = (TPCANChannelInformation * res[1])()
 
+            elif (
+                Parameter == PCAN_ACCEPTANCE_FILTER_11BIT
+                or PCAN_ACCEPTANCE_FILTER_29BIT
+            ):
+                mybuffer = c_int64(0)
+
             else:
                 mybuffer = c_int(0)
 
             res = self.__m_dllBasic.CAN_GetValue(
                 Channel, Parameter, byref(mybuffer), sizeof(mybuffer)
             )
             if Parameter == PCAN_ATTACHED_CHANNELS:
@@ -987,15 +1011,14 @@
             logger.error("Exception on PCANBasic.GetValue")
             raise
 
     # Returns a descriptive text of a given TPCANStatus
     # error code, in any desired language
     #
     def SetValue(self, Channel, Parameter, Buffer):
-
         """Returns a descriptive text of a given TPCANStatus error
         code, in any desired language
 
         Remarks:
           Parameters can be present or not according with the kind
           of Hardware (PCAN Channel) being used. If a parameter is not available,
           a PCAN_ERROR_ILLPARAMTYPE error will be returned.
@@ -1012,28 +1035,32 @@
         try:
             if (
                 Parameter == PCAN_LOG_LOCATION
                 or Parameter == PCAN_LOG_TEXT
                 or Parameter == PCAN_TRACE_LOCATION
             ):
                 mybuffer = create_string_buffer(256)
+            elif (
+                Parameter == PCAN_ACCEPTANCE_FILTER_11BIT
+                or PCAN_ACCEPTANCE_FILTER_29BIT
+            ):
+                mybuffer = c_int64(0)
             else:
                 mybuffer = c_int(0)
 
             mybuffer.value = Buffer
             res = self.__m_dllBasic.CAN_SetValue(
                 Channel, Parameter, byref(mybuffer), sizeof(mybuffer)
             )
             return TPCANStatus(res)
         except:
             logger.error("Exception on PCANBasic.SetValue")
             raise
 
     def GetErrorText(self, Error, Language=0):
-
         """Configures or sets a PCAN Channel value
 
         Remarks:
 
           The current languages available for translation are:
           Neutral (0x00), German (0x07), English (0x09), Spanish (0x0A),
           Italian (0x10) and French (0x0C)
@@ -1054,15 +1081,14 @@
             res = self.__m_dllBasic.CAN_GetErrorText(Error, Language, byref(mybuffer))
             return TPCANStatus(res), mybuffer.value
         except:
             logger.error("Exception on PCANBasic.GetErrorText")
             raise
 
     def LookUpChannel(self, Parameters):
-
         """Finds a PCAN-Basic channel that matches with the given parameters
 
         Remarks:
 
           The return value of this method is a 2-tuple, where
           the first value is the result (TPCANStatus) of the method and
           the second one a TPCANHandle value
```

### Comparing `python-can-4.1.0a2/can/interfaces/pcan/pcan.py` & `python-can-4.2.0rc0/can/interfaces/pcan/pcan.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,118 +1,129 @@
 """
 Enable basic CAN over a PCAN USB device.
 """
-
 import logging
+import platform
 import time
 from datetime import datetime
-import platform
-
-from typing import Optional
+from typing import Any, List, Optional, Tuple, Union
 
 from packaging import version
 
-from ...message import Message
-from ...bus import BusABC, BusState
-from ...util import len2dlc, dlc2len
-from ...exceptions import CanError, CanOperationError, CanInitializationError
-
+from can import (
+    BitTiming,
+    BitTimingFd,
+    BusABC,
+    BusState,
+    CanError,
+    CanInitializationError,
+    CanOperationError,
+    Message,
+)
+from can.util import check_or_adjust_timing_clock, dlc2len, len2dlc
 
 from .basic import (
-    PCAN_BITRATES,
-    PCAN_FD_PARAMETER_LIST,
-    PCAN_CHANNEL_NAMES,
-    PCAN_NONEBUS,
-    PCAN_BAUD_500K,
-    PCAN_TYPE_ISA,
-    PCANBasic,
-    PCAN_ERROR_OK,
+    FEATURE_FD_CAPABLE,
+    IS_LINUX,
+    IS_WINDOWS,
     PCAN_ALLOW_ERROR_FRAMES,
-    PCAN_PARAMETER_ON,
-    PCAN_RECEIVE_EVENT,
     PCAN_API_VERSION,
+    PCAN_ATTACHED_CHANNELS,
+    PCAN_BAUD_500K,
+    PCAN_BITRATES,
+    PCAN_BUSOFF_AUTORESET,
+    PCAN_CHANNEL_AVAILABLE,
+    PCAN_CHANNEL_CONDITION,
+    PCAN_CHANNEL_FEATURES,
+    PCAN_CHANNEL_IDENTIFYING,
+    PCAN_CHANNEL_NAMES,
     PCAN_DEVICE_NUMBER,
-    PCAN_ERROR_QRCVEMPTY,
-    PCAN_ERROR_BUSLIGHT,
+    PCAN_DICT_STATUS,
     PCAN_ERROR_BUSHEAVY,
-    PCAN_MESSAGE_EXTENDED,
-    PCAN_MESSAGE_RTR,
-    PCAN_MESSAGE_FD,
+    PCAN_ERROR_BUSLIGHT,
+    PCAN_ERROR_OK,
+    PCAN_ERROR_QRCVEMPTY,
+    PCAN_FD_PARAMETER_LIST,
+    PCAN_LANBUS1,
+    PCAN_LISTEN_ONLY,
     PCAN_MESSAGE_BRS,
-    PCAN_MESSAGE_ESI,
     PCAN_MESSAGE_ERRFRAME,
+    PCAN_MESSAGE_ESI,
+    PCAN_MESSAGE_EXTENDED,
+    PCAN_MESSAGE_FD,
+    PCAN_MESSAGE_RTR,
     PCAN_MESSAGE_STANDARD,
-    TPCANMsgFD,
-    TPCANMsg,
-    PCAN_CHANNEL_IDENTIFYING,
-    PCAN_LISTEN_ONLY,
+    PCAN_NONEBUS,
     PCAN_PARAMETER_OFF,
-    TPCANHandle,
+    PCAN_PARAMETER_ON,
+    PCAN_PCCBUS1,
     PCAN_PCIBUS1,
+    PCAN_RECEIVE_EVENT,
+    PCAN_TYPE_ISA,
     PCAN_USBBUS1,
-    PCAN_PCCBUS1,
-    PCAN_LANBUS1,
-    PCAN_CHANNEL_CONDITION,
-    PCAN_CHANNEL_AVAILABLE,
-    PCAN_CHANNEL_FEATURES,
-    FEATURE_FD_CAPABLE,
-    PCAN_DICT_STATUS,
-    PCAN_BUSOFF_AUTORESET,
+    VALID_PCAN_CAN_CLOCKS,
+    VALID_PCAN_FD_CLOCKS,
+    PCANBasic,
+    TPCANBaudrate,
+    TPCANChannelInformation,
+    TPCANHandle,
+    TPCANMsg,
+    TPCANMsgFD,
 )
 
-
 # Set up logging
 log = logging.getLogger("can.pcan")
 
 MIN_PCAN_API_VERSION = version.parse("4.2.0")
 
-
 try:
     # use the "uptime" library if available
     import uptime
 
     # boottime() and fromtimestamp() are timezone offset, so the difference is not.
     if uptime.boottime() is None:
         boottimeEpoch = 0
     else:
         boottimeEpoch = (uptime.boottime() - datetime.fromtimestamp(0)).total_seconds()
 except ImportError as error:
     log.warning(
         "uptime library not available, timestamps are relative to boot time and not to Epoch UTC",
-        exc_info=True,
     )
     boottimeEpoch = 0
 
-try:
-    # Try builtin Python 3 Windows API
-    from _overlapped import CreateEvent
-    from _winapi import WaitForSingleObject, WAIT_OBJECT_0, INFINITE
+HAS_EVENTS = False
 
-    HAS_EVENTS = True
-except ImportError:
+if IS_WINDOWS:
     try:
-        # Try pywin32 package
-        from win32event import CreateEvent
-        from win32event import WaitForSingleObject, WAIT_OBJECT_0, INFINITE
+        # Try builtin Python 3 Windows API
+        from _overlapped import CreateEvent
+        from _winapi import INFINITE, WAIT_OBJECT_0, WaitForSingleObject
 
         HAS_EVENTS = True
     except ImportError:
-        # Use polling instead
-        HAS_EVENTS = False
+        pass
+
+elif IS_LINUX:
+    try:
+        import select
+
+        HAS_EVENTS = True
+    except Exception:
+        pass
 
 
 class PcanBus(BusABC):
     def __init__(
         self,
-        channel="PCAN_USBBUS1",
-        device_id=None,
-        state=BusState.ACTIVE,
-        bitrate=500000,
-        *args,
-        **kwargs,
+        channel: str = "PCAN_USBBUS1",
+        device_id: Optional[int] = None,
+        state: BusState = BusState.ACTIVE,
+        timing: Optional[Union[BitTiming, BitTimingFd]] = None,
+        bitrate: int = 500000,
+        **kwargs: Any,
     ):
         """A PCAN USB interface to CAN.
 
         On top of the usual :class:`~can.Bus` methods provided,
         the PCAN interface includes the :meth:`flash`
         and :meth:`status` methods.
 
@@ -129,14 +140,26 @@
             first one that matches the parameter value. If no device is found,
             an exception is raised.
 
         :param can.bus.BusState state:
             BusState of the channel.
             Default is ACTIVE
 
+        :param timing:
+            An instance of :class:`~can.BitTiming` or :class:`~can.BitTimingFd`
+            to specify the bit timing parameters for the PCAN interface. If this parameter
+            is provided, it takes precedence over all other timing-related parameters.
+            If this parameter is not provided, the bit timing parameters can be specified
+            using the `bitrate` parameter for standard CAN or the `fd`, `f_clock`,
+            `f_clock_mhz`, `nom_brp`, `nom_tseg1`, `nom_tseg2`, `nom_sjw`, `data_brp`,
+            `data_tseg1`, `data_tseg2`, and `data_sjw` parameters for CAN FD.
+            Note that the `f_clock` value of the `timing` instance must be 8_000_000
+            for standard CAN or any of the following values for CAN FD: 20_000_000,
+            24_000_000, 30_000_000, 40_000_000, 60_000_000, 80_000_000.
+
         :param int bitrate:
             Bitrate of channel in bit/s.
             Default is 500 kbit/s.
             Ignored if using CanFD.
 
         :param bool fd:
             Should the Bus be initialized in CAN-FD mode.
@@ -214,56 +237,66 @@
         """
         self.m_objPCANBasic = PCANBasic()
 
         if device_id is not None:
             channel = self._find_channel_by_dev_id(device_id)
 
             if channel is None:
-                err_msg = "Cannot find a channel with ID {:08x}".format(device_id)
+                err_msg = f"Cannot find a channel with ID {device_id:08x}"
                 raise ValueError(err_msg)
 
         self.channel_info = str(channel)
-        self.fd = kwargs.get("fd", False)
-        pcan_bitrate = PCAN_BITRATES.get(bitrate, PCAN_BAUD_500K)
+        self.fd = isinstance(timing, BitTimingFd) if timing else kwargs.get("fd", False)
 
         hwtype = PCAN_TYPE_ISA
         ioport = 0x02A0
         interrupt = 11
 
         if not isinstance(channel, int):
             channel = PCAN_CHANNEL_NAMES[channel]
 
         self.m_PcanHandle = channel
 
         self.check_api_version()
 
-        if state is BusState.ACTIVE or state is BusState.PASSIVE:
+        if state in [BusState.ACTIVE, BusState.PASSIVE]:
             self.state = state
         else:
             raise ValueError("BusState must be Active or Passive")
 
-        if self.fd:
-            f_clock_val = kwargs.get("f_clock", None)
-            if f_clock_val is None:
-                f_clock = "{}={}".format("f_clock_mhz", kwargs.get("f_clock_mhz", None))
-            else:
-                f_clock = "{}={}".format("f_clock", kwargs.get("f_clock", None))
-
-            fd_parameters_values = [f_clock] + [
-                "{}={}".format(key, kwargs.get(key, None))
-                for key in PCAN_FD_PARAMETER_LIST
-                if kwargs.get(key, None) is not None
+        if isinstance(timing, BitTiming):
+            timing = check_or_adjust_timing_clock(timing, VALID_PCAN_CAN_CLOCKS)
+            pcan_bitrate = TPCANBaudrate(timing.btr0 << 8 | timing.btr1)
+            result = self.m_objPCANBasic.Initialize(
+                self.m_PcanHandle, pcan_bitrate, hwtype, ioport, interrupt
+            )
+        elif self.fd:
+            if isinstance(timing, BitTimingFd):
+                timing = check_or_adjust_timing_clock(
+                    timing, sorted(VALID_PCAN_FD_CLOCKS, reverse=True)
+                )
+                # We dump the timing parameters into the kwargs because they have equal names
+                # as the kwargs parameters and this saves us one additional code path
+                kwargs.update(timing)
+
+            clock_param = "f_clock" if "f_clock" in kwargs else "f_clock_mhz"
+            fd_parameters_values = [
+                f"{key}={kwargs[key]}"
+                for key in (clock_param,) + PCAN_FD_PARAMETER_LIST
+                if key in kwargs
             ]
 
-            self.fd_bitrate = " ,".join(fd_parameters_values).encode("ascii")
+            self.fd_bitrate = ", ".join(fd_parameters_values).encode("ascii")
 
             result = self.m_objPCANBasic.InitializeFD(
                 self.m_PcanHandle, self.fd_bitrate
             )
+
         else:
+            pcan_bitrate = PCAN_BITRATES.get(bitrate, PCAN_BAUD_500K)
             result = self.m_objPCANBasic.Initialize(
                 self.m_PcanHandle, pcan_bitrate, hwtype, ioport, interrupt
             )
 
         if result != PCAN_ERROR_OK:
             raise PcanCanInitializationError(self._get_formatted_error(result))
 
@@ -274,34 +307,40 @@
         if result != PCAN_ERROR_OK:
             if platform.system() != "Darwin":
                 raise PcanCanInitializationError(self._get_formatted_error(result))
             else:
                 # TODO Remove Filter when MACCan actually supports it:
                 #  https://github.com/mac-can/PCBUSB-Library/
                 log.debug(
-                    "Ignoring error. PCAN_ALLOW_ERROR_FRAMES is still unsupported by OSX Library PCANUSB v0.10"
+                    "Ignoring error. PCAN_ALLOW_ERROR_FRAMES is still unsupported by OSX Library PCANUSB v0.11.2"
                 )
 
         if kwargs.get("auto_reset", False):
             result = self.m_objPCANBasic.SetValue(
                 self.m_PcanHandle, PCAN_BUSOFF_AUTORESET, PCAN_PARAMETER_ON
             )
 
             if result != PCAN_ERROR_OK:
                 raise PcanCanInitializationError(self._get_formatted_error(result))
 
         if HAS_EVENTS:
-            self._recv_event = CreateEvent(None, 0, 0, None)
-            result = self.m_objPCANBasic.SetValue(
-                self.m_PcanHandle, PCAN_RECEIVE_EVENT, self._recv_event
-            )
+            if IS_WINDOWS:
+                self._recv_event = CreateEvent(None, 0, 0, None)
+                result = self.m_objPCANBasic.SetValue(
+                    self.m_PcanHandle, PCAN_RECEIVE_EVENT, self._recv_event
+                )
+            elif IS_LINUX:
+                result, self._recv_event = self.m_objPCANBasic.GetValue(
+                    self.m_PcanHandle, PCAN_RECEIVE_EVENT
+                )
+
             if result != PCAN_ERROR_OK:
                 raise PcanCanInitializationError(self._get_formatted_error(result))
 
-        super().__init__(channel=channel, state=state, bitrate=bitrate, *args, **kwargs)
+        super().__init__(channel=channel, state=state, bitrate=bitrate, **kwargs)
 
     def _find_channel_by_dev_id(self, device_id):
         """
         Iterate over all possible channels to find a channel that matches the device
         ID. This method is somewhat brute force, but the Basic API only offers a
         suitable API call since V4.4.0.
 
@@ -346,15 +385,15 @@
         stsReturn = self.m_objPCANBasic.GetErrorText(error, 0x9)
         if stsReturn[0] != PCAN_ERROR_OK:
             strings = []
 
             for b in bits(error):
                 stsReturn = self.m_objPCANBasic.GetErrorText(b, 0x9)
                 if stsReturn[0] != PCAN_ERROR_OK:
-                    text = "An error occurred. Error-code's text ({0:X}h) couldn't be retrieved".format(
+                    text = "An error occurred. Error-code's text ({:X}h) couldn't be retrieved".format(
                         error
                     )
                 else:
                     text = stsReturn[1].decode("utf-8", errors="replace")
 
                 strings.append(text)
 
@@ -433,92 +472,104 @@
             ):
                 raise ValueError()
         except ValueError:
             log.error("Invalid value '%s' for device number.", device_number)
             return False
         return True
 
-    def _recv_internal(self, timeout):
-
-        if HAS_EVENTS:
-            # We will utilize events for the timeout handling
-            timeout_ms = int(timeout * 1000) if timeout is not None else INFINITE
-        elif timeout is not None:
-            # Calculate max time
-            end_time = time.perf_counter() + timeout
-
-        # log.debug("Trying to read a msg")
+    def _recv_internal(
+        self, timeout: Optional[float]
+    ) -> Tuple[Optional[Message], bool]:
+        end_time = time.time() + timeout if timeout is not None else None
 
-        result = None
-        while result is None:
+        while True:
             if self.fd:
-                result = self.m_objPCANBasic.ReadFD(self.m_PcanHandle)
+                result, pcan_msg, pcan_timestamp = self.m_objPCANBasic.ReadFD(
+                    self.m_PcanHandle
+                )
             else:
-                result = self.m_objPCANBasic.Read(self.m_PcanHandle)
-            if result[0] == PCAN_ERROR_QRCVEMPTY:
-                if HAS_EVENTS:
-                    result = None
-                    val = WaitForSingleObject(self._recv_event, timeout_ms)
-                    if val != WAIT_OBJECT_0:
-                        return None, False
-                elif timeout is not None and time.perf_counter() >= end_time:
-                    return None, False
+                result, pcan_msg, pcan_timestamp = self.m_objPCANBasic.Read(
+                    self.m_PcanHandle
+                )
+
+            if result == PCAN_ERROR_OK:
+                # message received
+                break
+
+            if result == PCAN_ERROR_QRCVEMPTY:
+                # receive queue is empty, wait or return on timeout
+
+                if end_time is None:
+                    time_left: Optional[float] = None
+                    timed_out = False
                 else:
-                    result = None
+                    time_left = max(0.0, end_time - time.time())
+                    timed_out = time_left == 0.0
+
+                if timed_out:
+                    return None, False
+
+                if not HAS_EVENTS:
+                    # polling mode
                     time.sleep(0.001)
-            elif result[0] & (PCAN_ERROR_BUSLIGHT | PCAN_ERROR_BUSHEAVY):
-                log.warning(self._get_formatted_error(result[0]))
-                return None, False
-            elif result[0] != PCAN_ERROR_OK:
-                raise PcanCanOperationError(self._get_formatted_error(result[0]))
-
-        theMsg = result[1]
-        itsTimeStamp = result[2]
-
-        # log.debug("Received a message")
-
-        is_extended_id = (
-            theMsg.MSGTYPE & PCAN_MESSAGE_EXTENDED.value
-        ) == PCAN_MESSAGE_EXTENDED.value
-        is_remote_frame = (
-            theMsg.MSGTYPE & PCAN_MESSAGE_RTR.value
-        ) == PCAN_MESSAGE_RTR.value
-        is_fd = (theMsg.MSGTYPE & PCAN_MESSAGE_FD.value) == PCAN_MESSAGE_FD.value
-        bitrate_switch = (
-            theMsg.MSGTYPE & PCAN_MESSAGE_BRS.value
-        ) == PCAN_MESSAGE_BRS.value
-        error_state_indicator = (
-            theMsg.MSGTYPE & PCAN_MESSAGE_ESI.value
-        ) == PCAN_MESSAGE_ESI.value
-        is_error_frame = (
-            theMsg.MSGTYPE & PCAN_MESSAGE_ERRFRAME.value
-        ) == PCAN_MESSAGE_ERRFRAME.value
+                    continue
+
+                if IS_WINDOWS:
+                    # Windows with event
+                    if time_left is None:
+                        time_left_ms = INFINITE
+                    else:
+                        time_left_ms = int(time_left * 1000)
+                    _ret = WaitForSingleObject(self._recv_event, time_left_ms)
+                    if _ret == WAIT_OBJECT_0:
+                        continue
+
+                elif IS_LINUX:
+                    # Linux with event
+                    recv, _, _ = select.select([self._recv_event], [], [], time_left)
+                    if self._recv_event in recv:
+                        continue
+
+            elif result & (PCAN_ERROR_BUSLIGHT | PCAN_ERROR_BUSHEAVY):
+                log.warning(self._get_formatted_error(result))
+
+            else:
+                raise PcanCanOperationError(self._get_formatted_error(result))
+
+            return None, False
+
+        is_extended_id = bool(pcan_msg.MSGTYPE & PCAN_MESSAGE_EXTENDED.value)
+        is_remote_frame = bool(pcan_msg.MSGTYPE & PCAN_MESSAGE_RTR.value)
+        is_fd = bool(pcan_msg.MSGTYPE & PCAN_MESSAGE_FD.value)
+        bitrate_switch = bool(pcan_msg.MSGTYPE & PCAN_MESSAGE_BRS.value)
+        error_state_indicator = bool(pcan_msg.MSGTYPE & PCAN_MESSAGE_ESI.value)
+        is_error_frame = bool(pcan_msg.MSGTYPE & PCAN_MESSAGE_ERRFRAME.value)
 
         if self.fd:
-            dlc = dlc2len(theMsg.DLC)
-            timestamp = boottimeEpoch + (itsTimeStamp.value / (1000.0 * 1000.0))
+            dlc = dlc2len(pcan_msg.DLC)
+            timestamp = boottimeEpoch + (pcan_timestamp.value / (1000.0 * 1000.0))
         else:
-            dlc = theMsg.LEN
+            dlc = pcan_msg.LEN
             timestamp = boottimeEpoch + (
                 (
-                    itsTimeStamp.micros
-                    + 1000 * itsTimeStamp.millis
-                    + 0x100000000 * 1000 * itsTimeStamp.millis_overflow
+                    pcan_timestamp.micros
+                    + 1000 * pcan_timestamp.millis
+                    + 0x100000000 * 1000 * pcan_timestamp.millis_overflow
                 )
                 / (1000.0 * 1000.0)
             )
 
         rx_msg = Message(
             timestamp=timestamp,
-            arbitration_id=theMsg.ID,
+            arbitration_id=pcan_msg.ID,
             is_extended_id=is_extended_id,
             is_remote_frame=is_remote_frame,
             is_error_frame=is_error_frame,
             dlc=dlc,
-            data=theMsg.DATA[:dlc],
+            data=pcan_msg.DATA[:dlc],
             is_fd=is_fd,
             bitrate_switch=bitrate_switch,
             error_state_indicator=error_state_indicator,
         )
 
         return rx_msg, False
 
@@ -589,14 +640,17 @@
         """
         self.m_objPCANBasic.SetValue(
             self.m_PcanHandle, PCAN_CHANNEL_IDENTIFYING, bool(flash)
         )
 
     def shutdown(self):
         super().shutdown()
+        if HAS_EVENTS and IS_LINUX:
+            self.m_objPCANBasic.SetValue(self.m_PcanHandle, PCAN_RECEIVE_EVENT, 0)
+
         self.m_objPCANBasic.Uninitialize(self.m_PcanHandle)
 
     @property
     def state(self):
         return self._state
 
     @state.setter
@@ -620,15 +674,43 @@
     @staticmethod
     def _detect_available_configs():
         channels = []
         try:
             library_handle = PCANBasic()
         except OSError:
             return channels
+
         interfaces = []
+
+        if platform.system() != "Darwin":
+            res, value = library_handle.GetValue(PCAN_NONEBUS, PCAN_ATTACHED_CHANNELS)
+            if res != PCAN_ERROR_OK:
+                return interfaces
+            channel_information: List[TPCANChannelInformation] = list(value)
+            for channel in channel_information:
+                # find channel name in PCAN_CHANNEL_NAMES by value
+                channel_name = next(
+                    _channel_name
+                    for _channel_name, channel_id in PCAN_CHANNEL_NAMES.items()
+                    if channel_id.value == channel.channel_handle
+                )
+                channel_config = {
+                    "interface": "pcan",
+                    "channel": channel_name,
+                    "supports_fd": bool(channel.device_features & FEATURE_FD_CAPABLE),
+                    "controller_number": channel.controller_number,
+                    "device_features": channel.device_features,
+                    "device_id": channel.device_id,
+                    "device_name": channel.device_name.decode("latin-1"),
+                    "device_type": channel.device_type,
+                    "channel_condition": channel.channel_condition,
+                }
+                interfaces.append(channel_config)
+            return interfaces
+
         for i in range(16):
             interfaces.append(
                 {
                     "id": TPCANHandle(PCAN_PCIBUS1.value + i),
                     "name": "PCAN_PCIBUS" + str(i + 1),
                 }
             )
```

### Comparing `python-can-4.1.0a2/can/interfaces/robotell.py` & `python-can-4.2.0rc0/can/interfaces/robotell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Interface for Chinese Robotell compatible interfaces (win32/linux).
 """
 
 import io
-import time
 import logging
+import time
 from typing import Optional
 
 from can import BusABC, Message
+
 from ..exceptions import CanInterfaceNotImplementedError, CanOperationError
 
 logger = logging.getLogger(__name__)
 
 try:
     import serial
 except ImportError:
@@ -392,11 +393,11 @@
             return None
         sn2 = self._readconfig(self._CAN_READ_SERIAL2, timeout)
         if sn2 is None:
             return None
 
         serial = ""
         for idx in range(0, 8, 2):
-            serial += "{:02X}{:02X}-".format(sn1[idx], sn1[idx + 1])
+            serial += f"{sn1[idx]:02X}{sn1[idx + 1]:02X}-"
         for idx in range(0, 4, 2):
-            serial += "{:02X}{:02X}-".format(sn2[idx], sn2[idx + 1])
+            serial += f"{sn2[idx]:02X}{sn2[idx + 1]:02X}-"
         return serial[:-1]
```

### Comparing `python-can-4.1.0a2/can/interfaces/seeedstudio/seeedstudio.py` & `python-can-4.2.0rc0/can/interfaces/seeedstudio/seeedstudio.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 To Support the Seeed USB-Can analyzer interface. The device will appear
 as a serial port, for example "/dev/ttyUSB0" on Linux machines
 or "COM1" on Windows.
 https://www.seeedstudio.com/USB-CAN-Analyzer-p-2888.html
 SKU 114991193
 """
 
+import io
 import logging
 import struct
-import io
 from time import time
 
 import can
 from can import BusABC, Message
 
 logger = logging.getLogger("seeedbus")
```

### Comparing `python-can-4.1.0a2/can/interfaces/serial/serial_can.py` & `python-can-4.2.0rc0/can/interfaces/serial/serial_can.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 See the interface documentation for the format being used.
 """
 
 import io
 import logging
 import struct
-from typing import Any, List, Tuple, Optional
+from typing import Any, List, Optional, Tuple
 
-from can import BusABC, Message
 from can import (
-    CanInterfaceNotImplementedError,
+    BusABC,
     CanInitializationError,
+    CanInterfaceNotImplementedError,
     CanOperationError,
     CanTimeoutError,
+    Message,
 )
 from can.typechecking import AutoDetectedConfig
 
 logger = logging.getLogger("can.serial")
 
 try:
     import serial
@@ -171,15 +172,14 @@
                 Flags like ``is_extended_id``, ``is_remote_frame`` and ``is_error_frame``
                 will not be set over this function, the flags in the return
                 message are the default values.
         """
         try:
             rx_byte = self._ser.read()
             if rx_byte and ord(rx_byte) == 0xAA:
-
                 s = self._ser.read(4)
                 timestamp = struct.unpack("<I", s)[0]
                 dlc = ord(self._ser.read())
                 if dlc > 8:
                     raise ValueError("received DLC may not exceed 8 bytes")
 
                 s = self._ser.read(4)
```

### Comparing `python-can-4.1.0a2/can/interfaces/slcan.py` & `python-can-4.2.0rc0/can/interfaces/slcan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
 Interface for slcan compatible interfaces (win32/linux).
 """
 
-from typing import Any, Optional, Tuple
-
 import io
-import time
 import logging
+import time
+from typing import Any, Optional, Tuple
+
+from can import BusABC, Message, typechecking
 
-from can import BusABC, Message
 from ..exceptions import (
-    CanInterfaceNotImplementedError,
     CanInitializationError,
+    CanInterfaceNotImplementedError,
     CanOperationError,
     error_check,
 )
-from can import typechecking
-
 
 logger = logging.getLogger(__name__)
 
 try:
     import serial
 except ImportError:
     logger.warning(
@@ -60,14 +58,15 @@
         self,
         channel: typechecking.ChannelStr,
         ttyBaudrate: int = 115200,
         bitrate: Optional[int] = None,
         btr: Optional[str] = None,
         sleep_after_open: float = _SLEEP_AFTER_SERIAL_OPEN,
         rtscts: bool = False,
+        timeout: float = 0.001,
         **kwargs: Any,
     ) -> None:
         """
         :param str channel:
             port of underlying serial or usb device (e.g. ``/dev/ttyUSB0``, ``COM8``, ...)
             Must not be empty. Can also end with ``@115200`` (or similarly) to specify the baudrate.
         :param int ttyBaudrate:
@@ -78,15 +77,16 @@
             BTR register value to set custom can speed
         :param poll_interval:
             Poll interval in seconds when reading messages
         :param sleep_after_open:
             Time to wait in seconds after opening serial connection
         :param rtscts:
             turn hardware handshake (RTS/CTS) on and off
-
+        :param timeout:
+            Timeout for the serial or usb device in seconds (default 0.001)
         :raise ValueError: if both ``bitrate`` and ``btr`` are set or the channel is invalid
         :raise CanInterfaceNotImplementedError: if the serial module is missing
         :raise CanInitializationError: if the underlying serial connection could not be established
         """
         if serial is None:
             raise CanInterfaceNotImplementedError("The serial module is not installed")
 
@@ -94,15 +94,18 @@
             raise ValueError("Must specify a serial port.")
         if "@" in channel:
             (channel, baudrate) = channel.split("@")
             ttyBaudrate = int(baudrate)
 
         with error_check(exception_type=CanInitializationError):
             self.serialPortOrig = serial.serial_for_url(
-                channel, baudrate=ttyBaudrate, rtscts=rtscts
+                channel,
+                baudrate=ttyBaudrate,
+                rtscts=rtscts,
+                timeout=timeout,
             )
 
         self._buffer = bytearray()
 
         time.sleep(sleep_after_open)
 
         with error_check(exception_type=CanInitializationError):
@@ -146,87 +149,72 @@
 
     def _write(self, string: str) -> None:
         with error_check("Could not write to serial device"):
             self.serialPortOrig.write(string.encode() + self.LINE_TERMINATOR)
             self.serialPortOrig.flush()
 
     def _read(self, timeout: Optional[float]) -> Optional[str]:
+        _timeout = serial.Timeout(timeout)
 
         with error_check("Could not read from serial device"):
-            # first read what is already in receive buffer
-            while self.serialPortOrig.in_waiting:
-                self._buffer += self.serialPortOrig.read()
-            # if we still don't have a complete message, do a blocking read
-            start = time.time()
-            time_left = timeout
-            while not (
-                ord(self._OK) in self._buffer or ord(self._ERROR) in self._buffer
-            ):
-                self.serialPortOrig.timeout = time_left
-                byte = self.serialPortOrig.read()
-                if byte:
-                    self._buffer += byte
-                # if timeout is None, try indefinitely
-                if timeout is None:
-                    continue
-                # try next one only if there still is time, and with
-                # reduced timeout
-                else:
-                    time_left = timeout - (time.time() - start)
-                    if time_left > 0:
-                        continue
+            while True:
+                # Due to accessing `serialPortOrig.in_waiting` too often will reduce the performance.
+                # We read the `serialPortOrig.in_waiting` only once here.
+                in_waiting = self.serialPortOrig.in_waiting
+                for _ in range(max(1, in_waiting)):
+                    new_byte = self.serialPortOrig.read(size=1)
+                    if new_byte:
+                        self._buffer.extend(new_byte)
                     else:
-                        return None
+                        break
+
+                    if new_byte in (self._ERROR, self._OK):
+                        string = self._buffer.decode()
+                        self._buffer.clear()
+                        return string
+
+                if _timeout.expired():
+                    break
 
-        # return first message
-        for i in range(len(self._buffer)):
-            if self._buffer[i] == ord(self._OK) or self._buffer[i] == ord(self._ERROR):
-                string = self._buffer[: i + 1].decode()
-                del self._buffer[: i + 1]
-                break
-        return string
+            return None
 
     def flush(self) -> None:
-        del self._buffer[:]
+        self._buffer.clear()
         with error_check("Could not flush"):
-            while self.serialPortOrig.in_waiting:
-                self.serialPortOrig.read()
+            self.serialPortOrig.reset_input_buffer()
 
     def open(self) -> None:
         self._write("O")
 
     def close(self) -> None:
         self._write("C")
 
     def _recv_internal(
         self, timeout: Optional[float]
     ) -> Tuple[Optional[Message], bool]:
-
         canId = None
         remote = False
         extended = False
-        frame = []
+        data = None
 
         string = self._read(timeout)
 
         if not string:
             pass
         elif string[0] == "T":
             # extended frame
             canId = int(string[1:9], 16)
             dlc = int(string[9])
             extended = True
-            for i in range(0, dlc):
-                frame.append(int(string[10 + i * 2 : 12 + i * 2], 16))
+            data = bytearray.fromhex(string[10 : 10 + dlc * 2])
         elif string[0] == "t":
             # normal frame
             canId = int(string[1:4], 16)
             dlc = int(string[4])
-            for i in range(0, dlc):
-                frame.append(int(string[5 + i * 2 : 7 + i * 2], 16))
+            data = bytearray.fromhex(string[5 : 5 + dlc * 2])
         elif string[0] == "r":
             # remote frame
             canId = int(string[1:4], 16)
             dlc = int(string[4])
             remote = True
         elif string[0] == "R":
             # remote extended frame
@@ -238,33 +226,33 @@
         if canId is not None:
             msg = Message(
                 arbitration_id=canId,
                 is_extended_id=extended,
                 timestamp=time.time(),  # Better than nothing...
                 is_remote_frame=remote,
                 dlc=dlc,
-                data=frame,
+                data=data,
             )
             return msg, False
         return None, False
 
     def send(self, msg: Message, timeout: Optional[float] = None) -> None:
         if timeout != self.serialPortOrig.write_timeout:
             self.serialPortOrig.write_timeout = timeout
         if msg.is_remote_frame:
             if msg.is_extended_id:
-                sendStr = "R%08X%d" % (msg.arbitration_id, msg.dlc)
+                sendStr = f"R{msg.arbitration_id:08X}{msg.dlc:d}"
             else:
-                sendStr = "r%03X%d" % (msg.arbitration_id, msg.dlc)
+                sendStr = f"r{msg.arbitration_id:03X}{msg.dlc:d}"
         else:
             if msg.is_extended_id:
-                sendStr = "T%08X%d" % (msg.arbitration_id, msg.dlc)
+                sendStr = f"T{msg.arbitration_id:08X}{msg.dlc:d}"
             else:
-                sendStr = "t%03X%d" % (msg.arbitration_id, msg.dlc)
-            sendStr += "".join(["%02X" % b for b in msg.data])
+                sendStr = f"t{msg.arbitration_id:03X}{msg.dlc:d}"
+            sendStr += msg.data.hex().upper()
         self._write(sendStr)
 
     def shutdown(self) -> None:
         super().shutdown()
         self.close()
         with error_check("Could not close serial socket"):
             self.serialPortOrig.close()
@@ -291,64 +279,40 @@
             WHERE
             int hw_version is the hardware version or None on timeout
             int sw_version is the software version or None on timeout
         """
         cmd = "V"
         self._write(cmd)
 
-        start = time.time()
-        time_left = timeout
-        while True:
-            string = self._read(time_left)
-
-            if not string:
-                pass
-            elif string[0] == cmd and len(string) == 6:
-                # convert ASCII coded version
-                hw_version = int(string[1:3])
-                sw_version = int(string[3:5])
-                return hw_version, sw_version
-            # if timeout is None, try indefinitely
-            if timeout is None:
-                continue
-            # try next one only if there still is time, and with
-            # reduced timeout
-            else:
-                time_left = timeout - (time.time() - start)
-                if time_left > 0:
-                    continue
-                else:
-                    return None, None
+        string = self._read(timeout)
+
+        if not string:
+            pass
+        elif string[0] == cmd and len(string) == 6:
+            # convert ASCII coded version
+            hw_version = int(string[1:3])
+            sw_version = int(string[3:5])
+            return hw_version, sw_version
+
+        return None, None
 
     def get_serial_number(self, timeout: Optional[float]) -> Optional[str]:
         """Get serial number of the slcan interface.
 
         :param timeout:
             seconds to wait for serial number or :obj:`None` to wait indefinitely
 
         :return:
             :obj:`None` on timeout or a :class:`str` object.
         """
         cmd = "N"
         self._write(cmd)
 
-        start = time.time()
-        time_left = timeout
-        while True:
-            string = self._read(time_left)
-
-            if not string:
-                pass
-            elif string[0] == cmd and len(string) == 6:
-                serial_number = string[1:-1]
-                return serial_number
-            # if timeout is None, try indefinitely
-            if timeout is None:
-                continue
-            # try next one only if there still is time, and with
-            # reduced timeout
-            else:
-                time_left = timeout - (time.time() - start)
-                if time_left > 0:
-                    continue
-                else:
-                    return None
+        string = self._read(timeout)
+
+        if not string:
+            pass
+        elif string[0] == cmd and len(string) == 6:
+            serial_number = string[1:-1]
+            return serial_number
+
+        return None
```

### Comparing `python-can-4.1.0a2/can/interfaces/socketcan/constants.py` & `python-can-4.2.0rc0/can/interfaces/socketcan/constants.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/can/interfaces/socketcan/socketcan.py` & `python-can-4.2.0rc0/can/interfaces/socketcan/socketcan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 """
 The main module of the socketcan interface containing most user-facing classes and methods
 along some internal methods.
 
 At the end of the file the usage of the internal methods is shown.
 """
 
-from typing import Dict, List, Optional, Sequence, Tuple, Type, Union
-
-import logging
 import ctypes
 import ctypes.util
+import errno
+import logging
 import select
 import socket
 import struct
-import time
 import threading
-import errno
+import time
+from typing import Dict, List, Optional, Sequence, Tuple, Type, Union
 
 log = logging.getLogger(__name__)
 log_tx = log.getChild("tx")
 log_rx = log.getChild("rx")
 
 try:
-    import fcntl
-except ImportError:
-    log.error("fcntl not available on this platform")
-
-
-try:
     from socket import CMSG_SPACE
 
     CMSG_SPACE_available = True
 except ImportError:
     CMSG_SPACE_available = False
     log.error("socket.CMSG_SPACE not available on this platform")
 
 
 import can
-from can import Message, BusABC
+from can import BusABC, Message
 from can.broadcastmanager import (
+    LimitedDurationCyclicSendTaskABC,
     ModifiableCyclicTaskABC,
     RestartableCyclicTaskABC,
-    LimitedDurationCyclicSendTaskABC,
 )
+from can.interfaces.socketcan import constants
+from can.interfaces.socketcan.utils import find_available_interfaces, pack_filters
 from can.typechecking import CanFilters
-from can.interfaces.socketcan.constants import *  # CAN_RAW, CAN_*_FLAG
-from can.interfaces.socketcan.utils import pack_filters, find_available_interfaces
 
 
 # Setup BCM struct
 def bcm_header_factory(
     fields: List[Tuple[str, Union[Type[ctypes.c_uint32], Type[ctypes.c_long]]]],
     alignment: int = 8,
 ):
@@ -64,15 +57,15 @@
         field_alignment = ctypes.alignment(field[1])
         field_size = ctypes.sizeof(field[1])
 
         # If the current stride index isn't a multiple of the alignment
         # requirements of this field, then we must add padding bytes until we
         # are aligned
         while curr_stride % field_alignment != 0:
-            results.append(("pad_{}".format(pad_index), ctypes.c_uint8))
+            results.append((f"pad_{pad_index}", ctypes.c_uint8))
             pad_index += 1
             curr_stride += 1
 
         # Now can it fit?
         # Example: If this is 8 bytes and the type requires 4 bytes alignment
         # then we can only fit when we're starting at 0. Otherwise, we will
         # split across 2 strides.
@@ -80,15 +73,15 @@
         # | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
         results.append(field)
         curr_stride += field_size
 
     # Add trailing padding to align to a multiple of the largest scalar member
     # in the structure
     while curr_stride % alignment != 0:
-        results.append(("pad_{}".format(pad_index), ctypes.c_uint8))
+        results.append((f"pad_{pad_index}", ctypes.c_uint8))
         pad_index += 1
         curr_stride += 1
 
     return type("BcmMsgHead", (ctypes.Structure,), {"_fields_": results})
 
 
 # The fields definition is taken from the C struct definitions in
@@ -173,17 +166,17 @@
         __u8    __res1;  /* reserved / padding */
         __u8    data[CANFD_MAX_DLEN] __attribute__((aligned(8)));
     };
     """
     can_id = _compose_arbitration_id(msg)
     flags = 0
     if msg.bitrate_switch:
-        flags |= CANFD_BRS
+        flags |= constants.CANFD_BRS
     if msg.error_state_indicator:
-        flags |= CANFD_ESI
+        flags |= constants.CANFD_ESI
     max_len = 64 if msg.is_fd else 8
     data = bytes(msg.data).ljust(max_len, b"\x00")
     return CAN_FRAME_HEADER_STRUCT.pack(can_id, msg.dlc, flags) + data
 
 
 def build_bcm_header(
     opcode: int,
@@ -207,33 +200,33 @@
         can_id=can_id,
         nframes=nframes,
     )
     return ctypes.string_at(ctypes.addressof(result), ctypes.sizeof(result))
 
 
 def build_bcm_tx_delete_header(can_id: int, flags: int) -> bytes:
-    opcode = CAN_BCM_TX_DELETE
+    opcode = constants.CAN_BCM_TX_DELETE
     return build_bcm_header(opcode, flags, 0, 0, 0, 0, 0, can_id, 1)
 
 
 def build_bcm_transmit_header(
     can_id: int,
     count: int,
     initial_period: float,
     subsequent_period: float,
     msg_flags: int,
     nframes: int = 1,
 ) -> bytes:
-    opcode = CAN_BCM_TX_SETUP
+    opcode = constants.CAN_BCM_TX_SETUP
 
-    flags = msg_flags | SETTIMER | STARTTIMER
+    flags = msg_flags | constants.SETTIMER | constants.STARTTIMER
 
     if initial_period > 0:
         # Note `TX_COUNTEVT` creates the message TX_EXPIRED when count expires
-        flags |= TX_COUNTEVT
+        flags |= constants.TX_COUNTEVT
 
     def split_time(value: float) -> Tuple[int, int]:
         """Given seconds as a float, return whole seconds and microseconds"""
         seconds = int(value)
         microseconds = int(1e6 * (value - seconds))
         return seconds, microseconds
 
@@ -250,28 +243,30 @@
         ival2_usec,
         can_id,
         nframes,
     )
 
 
 def build_bcm_update_header(can_id: int, msg_flags: int, nframes: int = 1) -> bytes:
-    return build_bcm_header(CAN_BCM_TX_SETUP, msg_flags, 0, 0, 0, 0, 0, can_id, nframes)
+    return build_bcm_header(
+        constants.CAN_BCM_TX_SETUP, msg_flags, 0, 0, 0, 0, 0, can_id, nframes
+    )
 
 
 def dissect_can_frame(frame: bytes) -> Tuple[int, int, int, bytes]:
     can_id, can_dlc, flags = CAN_FRAME_HEADER_STRUCT.unpack_from(frame)
-    if len(frame) != CANFD_MTU:
+    if len(frame) != constants.CANFD_MTU:
         # Flags not valid in non-FD frames
         flags = 0
     return can_id, can_dlc, flags, frame[8 : 8 + can_dlc]
 
 
 def create_bcm_socket(channel: str) -> socket.socket:
     """create a broadcast manager socket and connect to the given interface"""
-    s = socket.socket(PF_CAN, socket.SOCK_DGRAM, CAN_BCM)
+    s = socket.socket(constants.PF_CAN, socket.SOCK_DGRAM, constants.CAN_BCM)
     s.connect((channel,))
     return s
 
 
 def send_bcm(bcm_socket: socket.socket, data: bytes) -> int:
     """
     Send raw frame to a BCM socket and handle errors.
@@ -293,21 +288,21 @@
         raise can.CanOperationError(base + specific_message, error.errno) from error
 
 
 def _compose_arbitration_id(message: Message) -> int:
     can_id = message.arbitration_id
     if message.is_extended_id:
         log.debug("sending an extended id type message")
-        can_id |= CAN_EFF_FLAG
+        can_id |= constants.CAN_EFF_FLAG
     if message.is_remote_frame:
         log.debug("requesting a remote frame")
-        can_id |= CAN_RTR_FLAG
+        can_id |= constants.CAN_RTR_FLAG
     if message.is_error_frame:
         log.debug("sending error frame")
-        can_id |= CAN_ERR_FLAG
+        can_id |= constants.CAN_ERR_FLAG
     return can_id
 
 
 class CyclicSendTask(
     LimitedDurationCyclicSendTaskABC, ModifiableCyclicTaskABC, RestartableCyclicTaskABC
 ):
     """
@@ -350,15 +345,15 @@
         self._tx_setup(self.messages)
 
     def _tx_setup(
         self, messages: Sequence[Message], raise_if_task_exists: bool = True
     ) -> None:
         # Create a low level packed frame to pass to the kernel
         body = bytearray()
-        self.flags = CAN_FD_FRAME if messages[0].is_fd else 0
+        self.flags = constants.CAN_FD_FRAME if messages[0].is_fd else 0
 
         if self.duration:
             count = int(self.duration / self.period)
             ival1 = self.period
             ival2 = 0.0
         else:
             count = 0
@@ -376,26 +371,26 @@
         log.debug("Sending BCM command")
         send_bcm(self.bcm_socket, header + body)
 
     def _check_bcm_task(self) -> None:
         # Do a TX_READ on a task ID, and check if we get EINVAL. If so,
         # then we are referring to a CAN message with an existing ID
         check_header = build_bcm_header(
-            opcode=CAN_BCM_TX_READ,
+            opcode=constants.CAN_BCM_TX_READ,
             flags=0,
             count=0,
             ival1_seconds=0,
             ival1_usec=0,
             ival2_seconds=0,
             ival2_usec=0,
             can_id=self.task_id,
             nframes=0,
         )
         log.debug(
-            f"Reading properties of (cyclic) transmission task id={self.task_id}",
+            "Reading properties of (cyclic) transmission task id=%d", self.task_id
         )
         try:
             self.bcm_socket.send(check_header)
         except OSError as error:
             if error.errno != errno.EINVAL:
                 raise can.CanOperationError("failed to check", error.errno) from error
             else:
@@ -491,15 +486,15 @@
         send_bcm(self.bcm_socket, header + body)
 
 
 def create_socket() -> socket.socket:
     """Creates a raw CAN socket. The socket will
     be returned unbound to any interface.
     """
-    sock = socket.socket(PF_CAN, socket.SOCK_RAW, CAN_RAW)
+    sock = socket.socket(constants.PF_CAN, socket.SOCK_RAW, constants.CAN_RAW)
 
     log.info("Created a socket")
 
     return sock
 
 
 def bind_socket(sock: socket.socket, channel: str = "can0") -> None:
@@ -530,50 +525,50 @@
         Find out which channel the message comes from.
 
     :return: The received message, or None on failure.
     """
     # Fetching the Arb ID, DLC and Data
     try:
         cf, ancillary_data, msg_flags, addr = sock.recvmsg(
-            CANFD_MTU, RECEIVED_ANCILLARY_BUFFER_SIZE
+            constants.CANFD_MTU, RECEIVED_ANCILLARY_BUFFER_SIZE
         )
         if get_channel:
             channel = addr[0] if isinstance(addr, tuple) else addr
         else:
             channel = None
     except OSError as error:
         raise can.CanOperationError(f"Error receiving: {error.strerror}", error.errno)
 
     can_id, can_dlc, flags, data = dissect_can_frame(cf)
 
     # Fetching the timestamp
     assert len(ancillary_data) == 1, "only requested a single extra field"
     cmsg_level, cmsg_type, cmsg_data = ancillary_data[0]
     assert (
-        cmsg_level == socket.SOL_SOCKET and cmsg_type == SO_TIMESTAMPNS
+        cmsg_level == socket.SOL_SOCKET and cmsg_type == constants.SO_TIMESTAMPNS
     ), "received control message type that was not requested"
     # see https://man7.org/linux/man-pages/man3/timespec.3.html -> struct timespec for details
     seconds, nanoseconds = RECEIVED_TIMESTAMP_STRUCT.unpack_from(cmsg_data)
     if nanoseconds >= 1e9:
         raise can.CanOperationError(
             f"Timestamp nanoseconds field was out of range: {nanoseconds} not less than 1e9"
         )
     timestamp = seconds + nanoseconds * 1e-9
 
     # EXT, RTR, ERR flags -> boolean attributes
     #   /* special address description flags for the CAN_ID */
     #   #define CAN_EFF_FLAG 0x80000000U /* EFF/SFF is set in the MSB */
     #   #define CAN_RTR_FLAG 0x40000000U /* remote transmission request */
     #   #define CAN_ERR_FLAG 0x20000000U /* error frame */
-    is_extended_frame_format = bool(can_id & CAN_EFF_FLAG)
-    is_remote_transmission_request = bool(can_id & CAN_RTR_FLAG)
-    is_error_frame = bool(can_id & CAN_ERR_FLAG)
-    is_fd = len(cf) == CANFD_MTU
-    bitrate_switch = bool(flags & CANFD_BRS)
-    error_state_indicator = bool(flags & CANFD_ESI)
+    is_extended_frame_format = bool(can_id & constants.CAN_EFF_FLAG)
+    is_remote_transmission_request = bool(can_id & constants.CAN_RTR_FLAG)
+    is_error_frame = bool(can_id & constants.CAN_ERR_FLAG)
+    is_fd = len(cf) == constants.CANFD_MTU
+    bitrate_switch = bool(flags & constants.CANFD_BRS)
+    error_state_indicator = bool(flags & constants.CANFD_ESI)
 
     # Section 4.7.1: MSG_DONTROUTE: set when the received frame was created on the local host.
     is_rx = not bool(msg_flags & socket.MSG_DONTROUTE)
 
     if is_extended_frame_format:
         # log.debug("CAN: Extended")
         # TODO does this depend on SFF or EFF?
@@ -621,16 +616,16 @@
         fd: bool = False,
         can_filters: Optional[CanFilters] = None,
         ignore_rx_error_frames=False,
         **kwargs,
     ) -> None:
         """Creates a new socketcan bus.
 
-        If setting some socket options fails, an error will be printed but no exception will be thrown.
-        This includes enabling:
+        If setting some socket options fails, an error will be printed
+        but no exception will be thrown. This includes enabling:
 
             - that own messages should be received,
             - CAN-FD frames and
             - error frames.
 
         :param channel:
             The can interface name with which to create this bus.
@@ -652,56 +647,64 @@
         :param can_filters:
             See :meth:`can.BusABC.set_filters`.
         :param ignore_rx_error_frames:
             If incoming error frames should be discarded.
         """
         self.socket = create_socket()
         self.channel = channel
-        self.channel_info = "socketcan channel '%s'" % channel
+        self.channel_info = f"socketcan channel '{channel}'"
         self._bcm_sockets: Dict[str, socket.socket] = {}
         self._is_filtered = False
         self._task_id = 0
         self._task_id_guard = threading.Lock()
 
         # set the local_loopback parameter
         try:
             self.socket.setsockopt(
-                SOL_CAN_RAW, CAN_RAW_LOOPBACK, 1 if local_loopback else 0
+                constants.SOL_CAN_RAW,
+                constants.CAN_RAW_LOOPBACK,
+                1 if local_loopback else 0,
             )
         except OSError as error:
             log.error("Could not set local loopback flag(%s)", error)
 
         # set the receive_own_messages parameter
         try:
             self.socket.setsockopt(
-                SOL_CAN_RAW, CAN_RAW_RECV_OWN_MSGS, 1 if receive_own_messages else 0
+                constants.SOL_CAN_RAW,
+                constants.CAN_RAW_RECV_OWN_MSGS,
+                1 if receive_own_messages else 0,
             )
         except OSError as error:
             log.error("Could not receive own messages (%s)", error)
 
         # enable CAN-FD frames if desired
         if fd:
             try:
-                self.socket.setsockopt(SOL_CAN_RAW, CAN_RAW_FD_FRAMES, 1)
+                self.socket.setsockopt(
+                    constants.SOL_CAN_RAW, constants.CAN_RAW_FD_FRAMES, 1
+                )
             except OSError as error:
                 log.error("Could not enable CAN-FD frames (%s)", error)
 
         if not ignore_rx_error_frames:
             # enable error frames
             try:
-                self.socket.setsockopt(SOL_CAN_RAW, CAN_RAW_ERR_FILTER, 0x1FFFFFFF)
+                self.socket.setsockopt(
+                    constants.SOL_CAN_RAW, constants.CAN_RAW_ERR_FILTER, 0x1FFFFFFF
+                )
             except OSError as error:
                 log.error("Could not enable error frames (%s)", error)
 
         # enable nanosecond resolution timestamping
         # we can always do this since
-        #  1) is is guaranteed to be at least as precise as without
+        #  1) it is guaranteed to be at least as precise as without
         #  2) it is available since Linux 2.6.22, and CAN support was only added afterward
         #     so this is always supported by the kernel
-        self.socket.setsockopt(socket.SOL_SOCKET, SO_TIMESTAMPNS, 1)
+        self.socket.setsockopt(socket.SOL_SOCKET, constants.SO_TIMESTAMPNS, 1)
 
         bind_socket(self.socket, channel)
         kwargs.update(
             {
                 "receive_own_messages": receive_own_messages,
                 "fd": fd,
                 "local_loopback": local_loopback,
@@ -826,15 +829,17 @@
         .. note::
 
             Note the duration before the messages stop being sent may not
             be exactly the same as the duration specified by the user. In
             general the message will be sent at the given rate until at
             least *duration* seconds.
         """
-        msgs = LimitedDurationCyclicSendTaskABC._check_and_convert_messages(msgs)
+        msgs = LimitedDurationCyclicSendTaskABC._check_and_convert_messages(  # pylint: disable=protected-access
+            msgs
+        )
 
         msgs_channel = str(msgs[0].channel) if msgs[0].channel else None
         bcm_socket = self._get_bcm_socket(msgs_channel or self.channel)
         task_id = self._get_next_task_id()
         task = CyclicSendTask(bcm_socket, task_id, msgs, period, duration)
         return task
 
@@ -846,15 +851,17 @@
     def _get_bcm_socket(self, channel: str) -> socket.socket:
         if channel not in self._bcm_sockets:
             self._bcm_sockets[channel] = create_bcm_socket(self.channel)
         return self._bcm_sockets[channel]
 
     def _apply_filters(self, filters: Optional[can.typechecking.CanFilters]) -> None:
         try:
-            self.socket.setsockopt(SOL_CAN_RAW, CAN_RAW_FILTER, pack_filters(filters))
+            self.socket.setsockopt(
+                constants.SOL_CAN_RAW, constants.CAN_RAW_FILTER, pack_filters(filters)
+            )
         except OSError as error:
             # fall back to "software filtering" (= not in kernel)
             self._is_filtered = False
             log.error(
                 "Setting filters failed; falling back to software filtering (not in kernel): %s",
                 error,
             )
@@ -895,12 +902,10 @@
         event.wait()
         sender_socket = create_socket()
         bind_socket(sender_socket, "vcan0")
         msg = Message(arbitration_id=0x01, data=b"\x01\x02\x03")
         sender_socket.send(build_can_frame(msg))
         print("Sender sent a message.")
 
-    import threading
-
     e = threading.Event()
     threading.Thread(target=receiver, args=(e,)).start()
     threading.Thread(target=sender, args=(e,)).start()
```

### Comparing `python-can-4.1.0a2/can/interfaces/socketcan/utils.py` & `python-can-4.2.0rc0/can/interfaces/socketcan/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 Defines common socketcan functions.
 """
 
 import errno
+import json
 import logging
 import os
-import re
 import struct
 import subprocess
-from typing import cast, Iterable, Optional
+from typing import List, Optional, cast
 
-from can.interfaces.socketcan.constants import CAN_EFF_FLAG
 from can import typechecking
+from can.interfaces.socketcan.constants import CAN_EFF_FLAG
 
 log = logging.getLogger(__name__)
 
 
 def pack_filters(can_filters: Optional[typechecking.CanFilters] = None) -> bytes:
     if can_filters is None:
         # Pass all messages
         can_filters = [{"can_id": 0, "can_mask": 0}]
 
-    can_filter_fmt = "={}I".format(2 * len(can_filters))
+    can_filter_fmt = f"={2 * len(can_filters)}I"
     filter_data = []
     for can_filter in can_filters:
         can_id = can_filter["can_id"]
         can_mask = can_filter["can_mask"]
         if "extended" in can_filter:
             can_filter = cast(typechecking.CanFilterExtended, can_filter)
             # Match on either 11-bit OR 29-bit messages instead of both
@@ -34,42 +34,44 @@
                 can_id |= CAN_EFF_FLAG
         filter_data.append(can_id)
         filter_data.append(can_mask)
 
     return struct.pack(can_filter_fmt, *filter_data)
 
 
-_PATTERN_CAN_INTERFACE = re.compile(r"(sl|v|vx)?can\d+")
+def find_available_interfaces() -> List[str]:
+    """Returns the names of all open can/vcan interfaces
 
-
-def find_available_interfaces() -> Iterable[str]:
-    """Returns the names of all open can/vcan interfaces using
-    the ``ip link list`` command. If the lookup fails, an error
+    The function calls the ``ip link list`` command. If the lookup fails, an error
     is logged to the console and an empty list is returned.
+
+    :return: The list of available and active CAN interfaces or an empty list of the command failed
     """
 
     try:
-        # adding "type vcan" would exclude physical can devices
-        command = ["ip", "-o", "link", "list", "up"]
-        output = subprocess.check_output(command, universal_newlines=True)
+        command = ["ip", "-json", "link", "list", "up"]
+        output_str = subprocess.check_output(command, text=True)
+    except Exception:  # pylint: disable=broad-except
+        # subprocess.CalledProcessError is too specific
+        log.exception("failed to fetch opened can devices from ip link")
+        return []
 
-    except Exception as e:  # subprocess.CalledProcessError is too specific
-        log.error("failed to fetch opened can devices: %s", e)
+    try:
+        output_json = json.loads(output_str)
+    except json.JSONDecodeError:
+        log.exception("Failed to parse ip link JSON output: %s", output_str)
         return []
 
-    else:
-        # log.debug("find_available_interfaces(): output=\n%s", output)
-        # output contains some lines like "1: vcan42: <NOARP,UP,LOWER_UP> ..."
-        # extract the "vcan42" of each line
-        interfaces = [line.split(": ", 3)[1] for line in output.splitlines()]
-        log.debug(
-            "find_available_interfaces(): detected these interfaces (before filtering): %s",
-            interfaces,
-        )
-        return filter(_PATTERN_CAN_INTERFACE.match, interfaces)
+    log.debug(
+        "find_available_interfaces(): detected these interfaces (before filtering): %s",
+        output_json,
+    )
+
+    interfaces = [i["ifname"] for i in output_json if i["link_type"] == "can"]
+    return interfaces
 
 
 def error_code_to_str(code: Optional[int]) -> str:
     """
     Converts a given error code (errno) to a useful and human readable string.
 
     :param code: a possibly invalid/unknown error code
```

### Comparing `python-can-4.1.0a2/can/interfaces/socketcand/socketcand.py` & `python-can-4.2.0rc0/can/interfaces/socketcand/socketcand.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,52 +3,63 @@
 see https://github.com/linux-can/socketcand
 
 Authors: Marvin Seiler, Gerrit Telkamp
 
 Copyright (C) 2021  DOMOLOGIC GmbH
 http://www.domologic.de
 """
-import can
-import socket
-import select
 import logging
+import select
+import socket
 import time
 import traceback
 from collections import deque
 
+import can
+
 log = logging.getLogger(__name__)
 
 
 def convert_ascii_message_to_can_message(ascii_msg: str) -> can.Message:
     if not ascii_msg.startswith("< frame ") or not ascii_msg.endswith(" >"):
         log.warning(f"Could not parse ascii message: {ascii_msg}")
         return None
     else:
         # frame_string = ascii_msg.removeprefix("< frame ").removesuffix(" >")
         frame_string = ascii_msg[8:-2]
         parts = frame_string.split(" ", 3)
         can_id, timestamp = int(parts[0], 16), float(parts[1])
+        is_ext = len(parts[0]) != 3
 
         data = bytearray.fromhex(parts[2])
         can_dlc = len(data)
         can_message = can.Message(
-            timestamp=timestamp, arbitration_id=can_id, data=data, dlc=can_dlc
+            timestamp=timestamp,
+            arbitration_id=can_id,
+            data=data,
+            dlc=can_dlc,
+            is_extended_id=is_ext,
+            is_rx=True,
         )
         return can_message
 
 
 def convert_can_message_to_ascii_message(can_message: can.Message) -> str:
     # Note: socketcan bus adds extended flag, remote_frame_flag & error_flag to id
     # not sure if that is necessary here
     can_id = can_message.arbitration_id
+    if can_message.is_extended_id:
+        can_id_string = f"{(can_id&0x1FFFFFFF):08X}"
+    else:
+        can_id_string = f"{(can_id&0x7FF):03X}"
     # Note: seems like we cannot add CANFD_BRS (bitrate_switch) and CANFD_ESI (error_state_indicator) flags
     data = can_message.data
     length = can_message.dlc
-    bytes_string = " ".join("{:x}".format(x) for x in data[0:length])
-    return f"< send {can_id:X} {length:X} {bytes_string} >"
+    bytes_string = " ".join(f"{x:x}" for x in data[0:length])
+    return f"< send {can_id_string} {length:X} {bytes_string} >"
 
 
 def connect_to_server(s, host, port):
     timeout_ms = 10000
     now = time.time() * 1000
     end_time = now + timeout_ms
     while now < end_time:
@@ -66,14 +77,16 @@
 class SocketCanDaemonBus(can.BusABC):
     def __init__(self, channel, host, port, can_filters=None, **kwargs):
         self.__host = host
         self.__port = port
         self.__socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.__message_buffer = deque()
         self.__receive_buffer = ""  # i know string is not the most efficient here
+        self.channel = channel
+        self.channel_info = f"socketcand on {channel}@{host}:{port}"
         connect_to_server(self.__socket, self.__host, self.__port)
         self._expect_msg("< hi >")
 
         log.info(
             f"SocketCanDaemonBus: connected with address {self.__socket.getsockname()}"
         )
         self._tcp_send(f"< open {channel} >")
@@ -135,14 +148,15 @@
                 single_message = buffer_view[start : end + 1]
                 parsed_can_message = convert_ascii_message_to_can_message(
                     single_message
                 )
                 if parsed_can_message is None:
                     log.warning(f"Invalid Frame: {single_message}")
                 else:
+                    parsed_can_message.channel = self.channel
                     self.__message_buffer.append(parsed_can_message)
                 buffer_view = buffer_view[end + 1 :]
 
             self.__receive_buffer = self.__receive_buffer[
                 chars_processed_successfully + 1 :
             ]
             can_message = (
@@ -166,9 +180,9 @@
             raise can.CanError(f"{msg} message expected!")
 
     def send(self, msg, timeout=None):
         ascii_msg = convert_can_message_to_ascii_message(msg)
         self._tcp_send(ascii_msg)
 
     def shutdown(self):
-        self.stop_all_periodic_tasks()
+        super().shutdown()
         self.__socket.close()
```

### Comparing `python-can-4.1.0a2/can/interfaces/systec/constants.py` & `python-can-4.2.0rc0/can/interfaces/systec/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from ctypes import c_ubyte as BYTE, c_ushort as WORD, c_ulong as DWORD
+from ctypes import c_ubyte as BYTE
+from ctypes import c_ulong as DWORD
+from ctypes import c_ushort as WORD
 
 #: Maximum number of modules that are supported.
 MAX_MODULES = 64
 
 #: Maximum number of applications that can use the USB-CAN-library.
 MAX_INSTANCES = 64
```

### Comparing `python-can-4.1.0a2/can/interfaces/systec/exceptions.py` & `python-can-4.2.0rc0/can/interfaces/systec/exceptions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from abc import ABC, abstractmethod
 from typing import Dict
 
-from abc import ABC, abstractmethod
+from can import CanError
 
 from .constants import ReturnCode
-from can import CanError
 
 
 class UcanException(CanError, ABC):
     """Base class for USB can errors."""
 
     def __init__(self, result, func, arguments):
         self.result = result
```

### Comparing `python-can-4.1.0a2/can/interfaces/systec/structures.py` & `python-can-4.2.0rc0/can/interfaces/systec/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,24 @@
-from ctypes import Structure, POINTER, sizeof
+import os
+from ctypes import POINTER, Structure, sizeof
+from ctypes import (
+    c_long as BOOL,
+)
 from ctypes import (
     c_ubyte as BYTE,
-    c_ushort as WORD,
+)
+from ctypes import (
     c_ulong as DWORD,
-    c_long as BOOL,
+)
+from ctypes import (
+    c_ushort as WORD,
+)
+from ctypes import (
     c_void_p as LPVOID,
 )
-import os
 
 # Workaround for Unix based platforms to be able to load structures for testing, etc...
 if os.name == "nt":
     from ctypes import WINFUNCTYPE as FUNCTYPE
 else:
     from ctypes import CFUNCTYPE as FUNCTYPE
```

### Comparing `python-can-4.1.0a2/can/interfaces/systec/ucan.py` & `python-can-4.2.0rc0/can/interfaces/systec/ucan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import logging
 import sys
-
 from ctypes import byref
 from ctypes import c_wchar_p as LPWSTR
 
 from ...exceptions import CanInterfaceNotImplementedError
-
 from .constants import *
-from .structures import *
 from .exceptions import *
+from .structures import *
 
 log = logging.getLogger("can.systec")
 
 
 def check_valid_rx_can_msg(result):
     """
     Checks if function :meth:`UcanServer.read_can_msg` returns a valid CAN message.
```

### Comparing `python-can-4.1.0a2/can/interfaces/systec/ucanbus.py` & `python-can-4.2.0rc0/can/interfaces/systec/ucanbus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from threading import Event
 
 from can import BusABC, BusState, Message
-from ...exceptions import CanError, CanInitializationError, CanOperationError
 
+from ...exceptions import CanError, CanInitializationError, CanOperationError
 from .constants import *
-from .structures import *
 from .exceptions import UcanException
+from .structures import *
 from .ucan import UcanServer
 
 log = logging.getLogger("can.systec")
 
 
 class Ucan(UcanServer):
     """
@@ -130,15 +130,15 @@
         if kwargs.get("tx_buffer_entries"):
             self._params["tx_buffer_entries"] = int(kwargs.get("tx_buffer_entries"))
 
         try:
             self._ucan.init_hardware(device_number=device_number)
             self._ucan.init_can(self.channel, **self._params)
             hw_info_ex, _, _ = self._ucan.get_hardware_info()
-            self.channel_info = "%s, S/N %s, CH %s, BTR %s" % (
+            self.channel_info = "{}, S/N {}, CH {}, BTR {}".format(
                 self._ucan.get_product_code_message(hw_info_ex.product_code),
                 hw_info_ex.serial,
                 self.channel,
                 self._ucan.get_baudrate_message(self.BITRATES[bitrate]),
             )
         except UcanException as exception:
             raise CanInitializationError() from exception
```

### Comparing `python-can-4.1.0a2/can/interfaces/udp_multicast/bus.py` & `python-can-4.2.0rc0/can/interfaces/udp_multicast/bus.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 log = logging.getLogger(__name__)
 
 import can
 from can import BusABC
 from can.typechecking import AutoDetectedConfig
 
-from .utils import pack_message, unpack_message, check_msgpack_installed
-
+from .utils import check_msgpack_installed, pack_message, unpack_message
 
 # see socket.getaddrinfo()
 IPv4_ADDRESS_INFO = Tuple[str, int]  # address, port
 IPv6_ADDRESS_INFO = Tuple[str, int, int, int]  # address, port, flowinfo, scope_id
 IP_ADDRESS_INFO = Union[IPv4_ADDRESS_INFO, IPv6_ADDRESS_INFO]
 
 # Additional constants for the interaction with Unix kernels
@@ -235,15 +234,14 @@
         """
         # create the UDP socket
         # this might already fail but then there is nothing to clean up
         sock = socket.socket(address_family, socket.SOCK_DGRAM)
 
         # configure the socket
         try:
-
             # set hop limit / TTL
             ttl_as_binary = struct.pack("@I", self.hop_limit)
             if self.ip_version == 4:
                 sock.setsockopt(
                     socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, ttl_as_binary
                 )
             else:
```

### Comparing `python-can-4.1.0a2/can/interfaces/udp_multicast/utils.py` & `python-can-4.2.0rc0/can/interfaces/udp_multicast/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
 Defines common functions.
 """
 
-from typing import Any
-from typing import Dict
-from typing import Optional
+from typing import Any, Dict, Optional
 
-from can import Message
-from can import CanInterfaceNotImplementedError
+from can import CanInterfaceNotImplementedError, Message
 from can.typechecking import ReadableBytesLike
 
 try:
     import msgpack
 except ImportError:
     msgpack = None
```

### Comparing `python-can-4.1.0a2/can/interfaces/usb2can/serial_selector.py` & `python-can-4.2.0rc0/can/interfaces/usb2can/serial_selector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 """
 
 import logging
 from typing import List
 
+log = logging.getLogger("can.usb2can")
+
 try:
     import win32com.client
 except ImportError:
-    logging.warning("win32com.client module required for usb2can")
+    log.warning("win32com.client module required for usb2can")
     raise
 
 
 def WMIDateStringToDate(dtmDate) -> str:
     if dtmDate[4] == 0:
         strDateTime = dtmDate[5] + "/"
     else:
@@ -43,15 +45,17 @@
 def find_serial_devices(serial_matcher: str = "") -> List[str]:
     """
     Finds a list of USB devices where the serial number (partially) matches the given string.
 
     :param serial_matcher:
         only device IDs starting with this string are returned
     """
-    objWMIService = win32com.client.Dispatch("WbemScripting.SWbemLocator")
-    objSWbemServices = objWMIService.ConnectServer(".", "root\\cimv2")
-    query = "SELECT * FROM CIM_LogicalDevice where Name LIKE '%USB2CAN%'"
-    devices = objSWbemServices.ExecQuery(query)
-    serial_numbers = [device.DeviceID.split("\\")[-1] for device in devices]
+    serial_numbers = []
+    wmi = win32com.client.GetObject("winmgmts:")
+    for usb_controller in wmi.InstancesOf("Win32_USBControllerDevice"):
+        usb_device = wmi.Get(usb_controller.Dependent)
+        if "USB2CAN" in usb_device.Name:
+            serial_numbers.append(usb_device.DeviceID.split("\\")[-1])
+
     if serial_matcher:
         return [sn for sn in serial_numbers if serial_matcher in sn]
     return serial_numbers
```

### Comparing `python-can-4.1.0a2/can/interfaces/usb2can/usb2canInterface.py` & `python-can-4.2.0rc0/can/interfaces/usb2can/usb2canInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 This interface is for Windows only, otherwise use SocketCAN.
 """
 
 import logging
 from ctypes import byref
 from typing import Optional
 
-from can import BusABC, Message, CanInitializationError, CanOperationError
-from .usb2canabstractionlayer import Usb2CanAbstractionLayer, CanalMsg, CanalError
+from can import BusABC, CanInitializationError, CanOperationError, Message
+
+from .serial_selector import find_serial_devices
 from .usb2canabstractionlayer import (
     IS_ERROR_FRAME,
-    IS_REMOTE_FRAME,
     IS_ID_TYPE,
+    IS_REMOTE_FRAME,
+    CanalError,
+    CanalMsg,
+    Usb2CanAbstractionLayer,
 )
-from .serial_selector import find_serial_devices
 
 # Set up logging
 log = logging.getLogger("can.usb2can")
 
 
 def message_convert_tx(msg):
     message_tx = CanalMsg()
@@ -95,15 +98,14 @@
         dll: str = "usb2can.dll",
         flags: int = 0x00000008,
         *_,
         bitrate: int = 500000,
         serial: Optional[str] = None,
         **kwargs,
     ):
-
         self.can = Usb2CanAbstractionLayer(dll)
 
         # get the serial number of the device
         device_id = serial or channel
 
         # search for a serial number if the device_id is None or empty
         if not device_id:
@@ -130,15 +132,14 @@
         else:
             status = self.can.send(self.handle, byref(tx))
 
         if status != CanalError.SUCCESS:
             raise CanOperationError("could not send message", error_code=status)
 
     def _recv_internal(self, timeout):
-
         messagerx = CanalMsg()
 
         if timeout == 0:
             status = self.can.receive(self.handle, byref(messagerx))
 
         else:
             time = 0 if timeout is None else int(timeout * 1000)
```

### Comparing `python-can-4.1.0a2/can/interfaces/usb2can/usb2canabstractionlayer.py` & `python-can-4.2.0rc0/can/interfaces/usb2can/usb2canabstractionlayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 This wrapper is for windows or direct access via CANAL API.
 Socket CAN is recommended under Unix/Linux systems.
 """
 
+import logging
 from ctypes import *
 from enum import IntEnum
-import logging
 
 import can
+
 from ...exceptions import error_check
 from ...typechecking import StringPathLike
 
 log = logging.getLogger("can.usb2can")
 
 # type definitions
 flags_t = c_ulong
```

### Comparing `python-can-4.1.0a2/can/interfaces/vector/canlib.py` & `python-can-4.2.0rc0/can/interfaces/vector/canlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,60 +4,68 @@
 Authors: Julien Grave <grave.jul@gmail.com>, Christian Sandberg
 """
 
 # Import Standard Python Modules
 # ==============================
 import ctypes
 import logging
-import time
 import os
+import time
 from types import ModuleType
 from typing import (
+    Any,
+    Callable,
+    Dict,
     List,
     NamedTuple,
     Optional,
-    Tuple,
     Sequence,
+    Tuple,
     Union,
-    Any,
-    Dict,
-    Callable,
     cast,
 )
 
 WaitForSingleObject: Optional[Callable[[int, int], int]]
 INFINITE: Optional[int]
 try:
     # Try builtin Python 3 Windows API
-    from _winapi import WaitForSingleObject, INFINITE  # type: ignore
+    from _winapi import INFINITE, WaitForSingleObject  # type: ignore
 
     HAS_EVENTS = True
 except ImportError:
     WaitForSingleObject, INFINITE = None, None
     HAS_EVENTS = False
 
 # Import Modules
 # ==============
-from can import BusABC, Message, CanInterfaceNotImplementedError, CanInitializationError
+from can import (
+    BitTiming,
+    BitTimingFd,
+    BusABC,
+    CanInitializationError,
+    CanInterfaceNotImplementedError,
+    Message,
+)
+from can.typechecking import AutoDetectedConfig, CanFilters
 from can.util import (
-    len2dlc,
-    dlc2len,
+    check_or_adjust_timing_clock,
     deprecated_args_alias,
+    dlc2len,
+    len2dlc,
     time_perfcounter_correlation,
 )
-from can.typechecking import AutoDetectedConfig, CanFilters
 
 # Define Module Logger
 # ====================
 LOG = logging.getLogger(__name__)
 
 # Import Vector API modules
 # =========================
+from . import xlclass, xldefine
 from .exceptions import VectorError, VectorInitializationError, VectorOperationError
-from . import xldefine, xlclass
 
 # Import safely Vector API module for Travis tests
 xldriver: Optional[ModuleType] = None
 try:
     from . import xldriver
 except Exception as exc:
     LOG.warning("Could not import vxlapi: %s", exc)
@@ -71,21 +79,26 @@
         tseg1Abr="tseg1_abr",
         tseg2Abr="tseg2_abr",
         sjwDbr="sjw_dbr",
         tseg1Dbr="tseg1_dbr",
         tseg2Dbr="tseg2_dbr",
     )
 
-    @deprecated_args_alias(**deprecated_args)
+    @deprecated_args_alias(
+        deprecation_start="4.0.0",
+        deprecation_end="5.0.0",
+        **deprecated_args,
+    )
     def __init__(
         self,
         channel: Union[int, Sequence[int], str],
         can_filters: Optional[CanFilters] = None,
         poll_interval: float = 0.01,
         receive_own_messages: bool = False,
+        timing: Optional[Union[BitTiming, BitTimingFd]] = None,
         bitrate: Optional[int] = None,
         rx_queue_size: int = 2**14,
         app_name: Optional[str] = "CANalyzer",
         serial: Optional[int] = None,
         fd: bool = False,
         data_bitrate: Optional[int] = None,
         sjw_abr: int = 2,
@@ -100,14 +113,24 @@
         :param channel:
             The channel indexes to create this bus with.
             Can also be a single integer or a comma separated string.
         :param can_filters:
             See :class:`can.BusABC`.
         :param receive_own_messages:
             See :class:`can.BusABC`.
+        :param timing:
+            An instance of :class:`~can.BitTiming` or :class:`~can.BitTimingFd`
+            to specify the bit timing parameters for the VectorBus interface. The
+            `f_clock` value of the timing instance must be set to 8_000_000 (8MHz)
+            or 16_000_000 (16MHz) for CAN 2.0 or 80_000_000 (80MHz) for CAN FD.
+            If this parameter is provided, it takes precedence over all other
+            timing-related parameters.
+            Otherwise, the bit timing can be specified using the following parameters:
+            `bitrate` for standard CAN or `fd`, `data_bitrate`, `sjw_abr`, `tseg1_abr`,
+            `tseg2_abr`, `sjw_dbr`, `tseg1_dbr`, and `tseg2_dbr` for CAN FD.
         :param poll_interval:
             Poll interval in seconds.
         :param bitrate:
             Bitrate in bits/s.
         :param rx_queue_size:
             Number of messages in receive queue (power of 2).
             CAN: range `16…32768`
@@ -140,15 +163,16 @@
 
         :raise ~can.exceptions.CanInterfaceNotImplementedError:
             If the current operating system is not supported or the driver could not be loaded.
         :raise ~can.exceptions.CanInitializationError:
             If the bus could not be set up.
             This may or may not be a :class:`~can.interfaces.vector.VectorInitializationError`.
         """
-        if os.name != "nt" and not kwargs.get("_testing", False):
+        self.__testing = kwargs.get("_testing", False)
+        if os.name != "nt" and not self.__testing:
             raise CanInterfaceNotImplementedError(
                 f"The Vector interface is only supported on Windows, "
                 f'but you are running "{os.name}"'
             )
 
         if xldriver is None:
             raise CanInterfaceNotImplementedError("The Vector API has not been loaded")
@@ -167,23 +191,23 @@
             self.channels = [int(ch) for ch in channel]
         else:
             raise TypeError(
                 f"Invalid type for parameter 'channel': {type(channel).__name__}"
             )
 
         self._app_name = app_name.encode() if app_name is not None else b""
-        self.channel_info = "Application %s: %s" % (
+        self.channel_info = "Application {}: {}".format(
             app_name,
             ", ".join(f"CAN {ch + 1}" for ch in self.channels),
         )
 
         channel_configs = get_channel_configs()
 
         self.mask = 0
-        self.fd = fd
+        self.fd = isinstance(timing, BitTimingFd) if timing else fd
         self.channel_masks: Dict[int, int] = {}
         self.index_to_channel: Dict[int, int] = {}
 
         for channel in self.channels:
             channel_index = self._find_global_channel_idx(
                 channel=channel,
                 serial=serial,
@@ -195,20 +219,20 @@
             channel_mask = 1 << channel_index
             self.channel_masks[channel] = channel_mask
             self.index_to_channel[channel_index] = channel
             self.mask |= channel_mask
 
         permission_mask = xlclass.XLaccess()
         # Set mask to request channel init permission if needed
-        if bitrate or fd:
+        if bitrate or fd or timing:
             permission_mask.value = self.mask
 
         interface_version = (
             xldefine.XL_InterfaceVersion.XL_INTERFACE_VERSION_V4
-            if fd
+            if self.fd
             else xldefine.XL_InterfaceVersion.XL_INTERFACE_VERSION
         )
 
         self.port_handle = xlclass.XLportHandle(xldefine.XL_INVALID_PORTHANDLE)
         self.xldriver.xlOpenPort(
             self.port_handle,
             self._app_name,
@@ -224,74 +248,43 @@
             "Open Port: PortHandle: %d, PermissionMask: 0x%X",
             self.port_handle.value,
             permission_mask.value,
         )
 
         # set CAN settings
         for channel in self.channels:
-            if self._has_init_access(channel):
-                if fd:
-                    self._set_bitrate_canfd(
-                        channel=channel,
-                        bitrate=bitrate,
-                        data_bitrate=data_bitrate,
-                        sjw_abr=sjw_abr,
-                        tseg1_abr=tseg1_abr,
-                        tseg2_abr=tseg2_abr,
-                        sjw_dbr=sjw_dbr,
-                        tseg1_dbr=tseg1_dbr,
-                        tseg2_dbr=tseg2_dbr,
-                    )
-                elif bitrate:
-                    self._set_bitrate_can(channel=channel, bitrate=bitrate)
-
-        # Check CAN settings
-        for channel in self.channels:
-            if kwargs.get("_testing", False):
-                # avoid check if xldriver is mocked for testing
-                break
-
-            bus_params = self._read_bus_params(channel)
-            if fd:
-                _canfd = bus_params.canfd
-                if not all(
-                    [
-                        bus_params.bus_type is xldefine.XL_BusTypes.XL_BUS_TYPE_CAN,
-                        _canfd.can_op_mode
-                        & xldefine.XL_CANFD_BusParams_CanOpMode.XL_BUS_PARAMS_CANOPMODE_CANFD,
-                        _canfd.bitrate == bitrate if bitrate else True,
-                        _canfd.sjw_abr == sjw_abr if bitrate else True,
-                        _canfd.tseg1_abr == tseg1_abr if bitrate else True,
-                        _canfd.tseg2_abr == tseg2_abr if bitrate else True,
-                        _canfd.data_bitrate == data_bitrate if data_bitrate else True,
-                        _canfd.sjw_dbr == sjw_dbr if data_bitrate else True,
-                        _canfd.tseg1_dbr == tseg1_dbr if data_bitrate else True,
-                        _canfd.tseg2_dbr == tseg2_dbr if data_bitrate else True,
-                    ]
-                ):
-                    raise CanInitializationError(
-                        f"The requested CAN FD settings could not be set for channel {channel}. "
-                        f"Another application might have set incompatible settings. "
-                        f"These are the currently active settings: {_canfd._asdict()}"
-                    )
-            else:
-                _can = bus_params.can
-                if not all(
-                    [
-                        bus_params.bus_type is xldefine.XL_BusTypes.XL_BUS_TYPE_CAN,
-                        _can.can_op_mode
-                        & xldefine.XL_CANFD_BusParams_CanOpMode.XL_BUS_PARAMS_CANOPMODE_CAN20,
-                        _can.bitrate == bitrate if bitrate else True,
-                    ]
-                ):
-                    raise CanInitializationError(
-                        f"The requested CAN settings could not be set for channel {channel}. "
-                        f"Another application might have set incompatible settings. "
-                        f"These are the currently active settings: {_can._asdict()}"
-                    )
+            if isinstance(timing, BitTiming):
+                timing = check_or_adjust_timing_clock(timing, [16_000_000, 8_000_000])
+                self._set_bit_timing(
+                    channel=channel,
+                    timing=timing,
+                )
+            elif isinstance(timing, BitTimingFd):
+                timing = check_or_adjust_timing_clock(timing, [80_000_000])
+                self._set_bit_timing_fd(
+                    channel=channel,
+                    timing=timing,
+                )
+            elif fd:
+                self._set_bit_timing_fd(
+                    channel=channel,
+                    timing=BitTimingFd.from_bitrate_and_segments(
+                        f_clock=80_000_000,
+                        nom_bitrate=bitrate or 500_000,
+                        nom_tseg1=tseg1_abr,
+                        nom_tseg2=tseg2_abr,
+                        nom_sjw=sjw_abr,
+                        data_bitrate=data_bitrate or bitrate or 500_000,
+                        data_tseg1=tseg1_dbr,
+                        data_tseg2=tseg2_dbr,
+                        data_sjw=sjw_dbr,
+                    ),
+                )
+            elif bitrate:
+                self._set_bitrate(channel=channel, bitrate=bitrate)
 
         # Enable/disable TX receipts
         tx_receipts = 1 if receive_own_messages else 0
         self.xldriver.xlCanSetChannelMode(self.port_handle, self.mask, tx_receipts, 0)
 
         if HAS_EVENTS:
             self.event_handle = xlclass.XLhandle()
@@ -336,27 +329,29 @@
         self,
         channel: int,
         serial: Optional[int],
         app_name: Optional[str],
         channel_configs: List["VectorChannelConfig"],
     ) -> int:
         if serial is not None:
-            hw_type: Optional[xldefine.XL_HardwareType] = None
+            serial_found = False
             for channel_config in channel_configs:
                 if channel_config.serial_number != serial:
                     continue
 
-                hw_type = xldefine.XL_HardwareType(channel_config.hw_type)
+                serial_found = True
                 if channel_config.hw_channel == channel:
                     return channel_config.channel_index
 
-            if hw_type is None:
+            if not serial_found:
                 err_msg = f"No interface with serial {serial} found."
             else:
-                err_msg = f"Channel {channel} not found on interface {hw_type.name} ({serial})."
+                err_msg = (
+                    f"Channel {channel} not found on interface with serial {serial}."
+                )
             raise CanInitializationError(
                 err_msg, error_code=xldefine.XL_Status.XL_ERR_HW_NOT_PRESENT
             )
 
         if app_name:
             hw_type, hw_index, hw_channel = self.get_application_config(
                 app_name, channel
@@ -398,106 +393,208 @@
             if vcc.channel_mask == channel_mask:
                 return vcc.bus_params
 
         raise CanInitializationError(
             f"Channel configuration for channel {channel} not found."
         )
 
-    def _set_bitrate_can(
+    def _set_bitrate(self, channel: int, bitrate: int) -> None:
+        # set parameters if channel has init access
+        if self._has_init_access(channel):
+            self.xldriver.xlCanSetChannelBitrate(
+                self.port_handle,
+                self.channel_masks[channel],
+                bitrate,
+            )
+            LOG.info("xlCanSetChannelBitrate: baudr.=%u", bitrate)
+
+        if not self.__testing:
+            self._check_can_settings(
+                channel=channel,
+                bitrate=bitrate,
+            )
+
+    def _set_bit_timing(self, channel: int, timing: BitTiming) -> None:
+        # set parameters if channel has init access
+        if self._has_init_access(channel):
+            if timing.f_clock == 8_000_000:
+                self.xldriver.xlCanSetChannelParamsC200(
+                    self.port_handle,
+                    self.channel_masks[channel],
+                    timing.btr0,
+                    timing.btr1,
+                )
+                LOG.info(
+                    "xlCanSetChannelParamsC200: BTR0=%#02x, BTR1=%#02x",
+                    timing.btr0,
+                    timing.btr1,
+                )
+            elif timing.f_clock == 16_000_000:
+                chip_params = xlclass.XLchipParams()
+                chip_params.bitRate = timing.bitrate
+                chip_params.sjw = timing.sjw
+                chip_params.tseg1 = timing.tseg1
+                chip_params.tseg2 = timing.tseg2
+                chip_params.sam = timing.nof_samples
+                self.xldriver.xlCanSetChannelParams(
+                    self.port_handle,
+                    self.channel_masks[channel],
+                    chip_params,
+                )
+                LOG.info(
+                    "xlCanSetChannelParams: baudr.=%u, sjwAbr=%u, tseg1Abr=%u, tseg2Abr=%u",
+                    chip_params.bitRate,
+                    chip_params.sjw,
+                    chip_params.tseg1,
+                    chip_params.tseg2,
+                )
+            else:
+                raise CanInitializationError(
+                    f"timing.f_clock must be 8_000_000 or 16_000_000 (is {timing.f_clock})"
+                )
+
+        if not self.__testing:
+            self._check_can_settings(
+                channel=channel,
+                bitrate=timing.bitrate,
+                sample_point=timing.sample_point,
+            )
+
+    def _set_bit_timing_fd(
         self,
         channel: int,
-        bitrate: int,
-        sjw: Optional[int] = None,
-        tseg1: Optional[int] = None,
-        tseg2: Optional[int] = None,
-        sam: int = 1,
+        timing: BitTimingFd,
     ) -> None:
-        kwargs = [sjw, tseg1, tseg2]
-        if any(kwargs) and not all(kwargs):
-            raise ValueError(
-                f"Either all of sjw, tseg1, tseg2 must be set or none of them."
-            )
-
         # set parameters if channel has init access
-        if any(kwargs):
-            chip_params = xlclass.XLchipParams()
-            chip_params.bitRate = bitrate
-            chip_params.sjw = sjw
-            chip_params.tseg1 = tseg1
-            chip_params.tseg2 = tseg2
-            chip_params.sam = sam
-            self.xldriver.xlCanSetChannelParams(
-                self.port_handle,
-                self.channel_masks[channel],
-                chip_params,
+        if self._has_init_access(channel):
+            canfd_conf = xlclass.XLcanFdConf()
+            canfd_conf.arbitrationBitRate = timing.nom_bitrate
+            canfd_conf.sjwAbr = timing.nom_sjw
+            canfd_conf.tseg1Abr = timing.nom_tseg1
+            canfd_conf.tseg2Abr = timing.nom_tseg2
+            canfd_conf.dataBitRate = timing.data_bitrate
+            canfd_conf.sjwDbr = timing.data_sjw
+            canfd_conf.tseg1Dbr = timing.data_tseg1
+            canfd_conf.tseg2Dbr = timing.data_tseg2
+            self.xldriver.xlCanFdSetConfiguration(
+                self.port_handle, self.channel_masks[channel], canfd_conf
             )
             LOG.info(
-                "xlCanSetChannelParams: baudr.=%u, sjwAbr=%u, tseg1Abr=%u, tseg2Abr=%u",
-                chip_params.bitRate,
-                chip_params.sjw,
-                chip_params.tseg1,
-                chip_params.tseg2,
+                "xlCanFdSetConfiguration.: ABaudr.=%u, DBaudr.=%u",
+                canfd_conf.arbitrationBitRate,
+                canfd_conf.dataBitRate,
             )
-        else:
-            self.xldriver.xlCanSetChannelBitrate(
-                self.port_handle,
-                self.channel_masks[channel],
-                bitrate,
+            LOG.info(
+                "xlCanFdSetConfiguration.: sjwAbr=%u, tseg1Abr=%u, tseg2Abr=%u",
+                canfd_conf.sjwAbr,
+                canfd_conf.tseg1Abr,
+                canfd_conf.tseg2Abr,
+            )
+            LOG.info(
+                "xlCanFdSetConfiguration.: sjwDbr=%u, tseg1Dbr=%u, tseg2Dbr=%u",
+                canfd_conf.sjwDbr,
+                canfd_conf.tseg1Dbr,
+                canfd_conf.tseg2Dbr,
+            )
+
+        if not self.__testing:
+            self._check_can_settings(
+                channel=channel,
+                bitrate=timing.nom_bitrate,
+                sample_point=timing.nom_sample_point,
+                fd=True,
+                data_bitrate=timing.data_bitrate,
+                data_sample_point=timing.data_sample_point,
             )
-            LOG.info("xlCanSetChannelBitrate: baudr.=%u", bitrate)
 
-    def _set_bitrate_canfd(
+    def _check_can_settings(
         self,
         channel: int,
-        bitrate: Optional[int] = None,
+        bitrate: int,
+        sample_point: Optional[float] = None,
+        fd: bool = False,
         data_bitrate: Optional[int] = None,
-        sjw_abr: int = 2,
-        tseg1_abr: int = 6,
-        tseg2_abr: int = 3,
-        sjw_dbr: int = 2,
-        tseg1_dbr: int = 6,
-        tseg2_dbr: int = 3,
+        data_sample_point: Optional[float] = None,
     ) -> None:
-        # set parameters if channel has init access
-        canfd_conf = xlclass.XLcanFdConf()
-        if bitrate:
-            canfd_conf.arbitrationBitRate = int(bitrate)
-        else:
-            canfd_conf.arbitrationBitRate = 500_000
-        canfd_conf.sjwAbr = int(sjw_abr)
-        canfd_conf.tseg1Abr = int(tseg1_abr)
-        canfd_conf.tseg2Abr = int(tseg2_abr)
-        if data_bitrate:
-            canfd_conf.dataBitRate = int(data_bitrate)
-        else:
-            canfd_conf.dataBitRate = int(canfd_conf.arbitrationBitRate)
-        canfd_conf.sjwDbr = int(sjw_dbr)
-        canfd_conf.tseg1Dbr = int(tseg1_dbr)
-        canfd_conf.tseg2Dbr = int(tseg2_dbr)
-        self.xldriver.xlCanFdSetConfiguration(
-            self.port_handle, self.channel_masks[channel], canfd_conf
-        )
-        LOG.info(
-            "xlCanFdSetConfiguration.: ABaudr.=%u, DBaudr.=%u",
-            canfd_conf.arbitrationBitRate,
-            canfd_conf.dataBitRate,
-        )
-        LOG.info(
-            "xlCanFdSetConfiguration.: sjwAbr=%u, tseg1Abr=%u, tseg2Abr=%u",
-            canfd_conf.sjwAbr,
-            canfd_conf.tseg1Abr,
-            canfd_conf.tseg2Abr,
-        )
-        LOG.info(
-            "xlCanFdSetConfiguration.: sjwDbr=%u, tseg1Dbr=%u, tseg2Dbr=%u",
-            canfd_conf.sjwDbr,
-            canfd_conf.tseg1Dbr,
-            canfd_conf.tseg2Dbr,
+        """Compare requested CAN settings to active settings in driver."""
+        bus_params = self._read_bus_params(channel)
+        # use canfd even if fd==False, bus_params.can and bus_params.canfd are a C union
+        bus_params_data = bus_params.canfd
+        settings_acceptable = True
+
+        # check bus type
+        settings_acceptable &= (
+            bus_params.bus_type is xldefine.XL_BusTypes.XL_BUS_TYPE_CAN
         )
 
+        # check CAN operation mode
+        if fd:
+            settings_acceptable &= bool(
+                bus_params_data.can_op_mode
+                & xldefine.XL_CANFD_BusParams_CanOpMode.XL_BUS_PARAMS_CANOPMODE_CANFD
+            )
+        elif bus_params_data.can_op_mode != 0:  # can_op_mode is always 0 for cancaseXL
+            settings_acceptable &= bool(
+                bus_params_data.can_op_mode
+                & xldefine.XL_CANFD_BusParams_CanOpMode.XL_BUS_PARAMS_CANOPMODE_CAN20
+            )
+
+        # check bitrates
+        if bitrate:
+            settings_acceptable &= (
+                abs(bus_params_data.bitrate - bitrate) < bitrate / 256
+            )
+        if fd and data_bitrate:
+            settings_acceptable &= (
+                abs(bus_params_data.data_bitrate - data_bitrate) < data_bitrate / 256
+            )
+
+        # check sample points
+        if sample_point:
+            nom_sample_point_act = (
+                100
+                * (1 + bus_params_data.tseg1_abr)
+                / (1 + bus_params_data.tseg1_abr + bus_params_data.tseg2_abr)
+            )
+            settings_acceptable &= (
+                abs(nom_sample_point_act - sample_point) < 2.0  # 2 percent tolerance
+            )
+        if fd and data_sample_point:
+            data_sample_point_act = (
+                100
+                * (1 + bus_params_data.tseg1_dbr)
+                / (1 + bus_params_data.tseg1_dbr + bus_params_data.tseg2_dbr)
+            )
+            settings_acceptable &= (
+                abs(data_sample_point_act - data_sample_point)
+                < 2.0  # 2 percent tolerance
+            )
+
+        if not settings_acceptable:
+            # The error message depends on the currently active CAN settings.
+            # If the active operation mode is CAN FD, show the active CAN FD timings,
+            # otherwise show CAN 2.0 timings.
+            if bool(
+                bus_params_data.can_op_mode
+                & xldefine.XL_CANFD_BusParams_CanOpMode.XL_BUS_PARAMS_CANOPMODE_CANFD
+            ):
+                active_settings = bus_params.canfd._asdict()
+                active_settings["can_op_mode"] = "CAN FD"
+            else:
+                active_settings = bus_params.can._asdict()
+                active_settings["can_op_mode"] = "CAN 2.0"
+            settings_string = ", ".join(
+                [f"{key}: {val}" for key, val in active_settings.items()]
+            )
+            raise CanInitializationError(
+                f"The requested settings could not be set for channel {channel}. "
+                f"Another application might have set incompatible settings. "
+                f"These are the currently active settings: {settings_string}."
+            )
+
     def _apply_filters(self, filters: Optional[CanFilters]) -> None:
         if filters:
             # Only up to one filter per ID type allowed
             if len(filters) == 1 or (
                 len(filters) == 2
                 and filters[0].get("extended") != filters[1].get("extended")
             ):
@@ -829,15 +926,15 @@
             raise CanInterfaceNotImplementedError("The Vector API has not been loaded")
 
         xldriver.xlPopupHwConfig(ctypes.c_char_p(), ctypes.c_uint(wait_for_finish))
 
     @staticmethod
     def get_application_config(
         app_name: str, app_channel: int
-    ) -> Tuple[xldefine.XL_HardwareType, int, int]:
+    ) -> Tuple[Union[int, xldefine.XL_HardwareType], int, int]:
         """Retrieve information for an application in Vector Hardware Configuration.
 
         :param app_name:
             The name of the application.
         :param app_channel:
             The channel of the application.
         :return:
@@ -869,21 +966,21 @@
                 error_code=e.error_code,
                 error_string=(
                     f"Vector HW Config: Channel '{app_channel}' of "
                     f"application '{app_name}' is not assigned to any interface"
                 ),
                 function="xlGetApplConfig",
             ) from None
-        return xldefine.XL_HardwareType(hw_type.value), hw_index.value, hw_channel.value
+        return _hw_type(hw_type.value), hw_index.value, hw_channel.value
 
     @staticmethod
     def set_application_config(
         app_name: str,
         app_channel: int,
-        hw_type: xldefine.XL_HardwareType,
+        hw_type: Union[int, xldefine.XL_HardwareType],
         hw_index: int,
         hw_channel: int,
         **kwargs: Any,
     ) -> None:
         """Modify the application settings in Vector Hardware Configuration.
 
         This method can also be used with a channel config dictionary::
@@ -969,15 +1066,15 @@
     canfd: VectorCanFdParams
 
 
 class VectorChannelConfig(NamedTuple):
     """NamedTuple which contains the channel properties from Vector XL API."""
 
     name: str
-    hw_type: xldefine.XL_HardwareType
+    hw_type: Union[int, xldefine.XL_HardwareType]
     hw_index: int
     hw_channel: int
     channel_index: int
     channel_mask: int
     channel_capabilities: xldefine.XL_ChannelCapabilities
     channel_bus_capabilities: xldefine.XL_BusCapabilities
     is_on_bus: bool
@@ -1042,15 +1139,15 @@
         return []
 
     channel_list: List[VectorChannelConfig] = []
     for i in range(driver_config.channelCount):
         xlcc: xlclass.XLchannelConfig = driver_config.channel[i]
         vcc = VectorChannelConfig(
             name=xlcc.name.decode(),
-            hw_type=xldefine.XL_HardwareType(xlcc.hwType),
+            hw_type=_hw_type(xlcc.hwType),
             hw_index=xlcc.hwIndex,
             hw_channel=xlcc.hwChannel,
             channel_index=xlcc.channelIndex,
             channel_mask=xlcc.channelMask,
             channel_capabilities=xldefine.XL_ChannelCapabilities(
                 xlcc.channelCapabilities
             ),
@@ -1062,7 +1159,15 @@
             connected_bus_type=xldefine.XL_BusTypes(xlcc.connectedBusType),
             serial_number=xlcc.serialNumber,
             article_number=xlcc.articleNumber,
             transceiver_name=xlcc.transceiverName.decode(),
         )
         channel_list.append(vcc)
     return channel_list
+
+
+def _hw_type(hw_type: int) -> Union[int, xldefine.XL_HardwareType]:
+    try:
+        return xldefine.XL_HardwareType(hw_type)
+    except ValueError:
+        LOG.warning(f'Unknown XL_HardwareType value "{hw_type}"')
+        return hw_type
```

### Comparing `python-can-4.1.0a2/can/interfaces/vector/exceptions.py` & `python-can-4.2.0rc0/can/interfaces/vector/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/can/interfaces/vector/xlclass.py` & `python-can-4.2.0rc0/can/interfaces/vector/xlclass.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/can/interfaces/vector/xldefine.py` & `python-can-4.2.0rc0/can/interfaces/vector/xldefine.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Definition of constants for vxlapi.
 """
 
 # Import Python Modules
 # ==============================
 from enum import IntEnum, IntFlag
 
-
 MAX_MSG_LEN = 8
 XL_CAN_MAX_DATA_LEN = 64
 XL_INVALID_PORTHANDLE = -1
 
 
 class XL_AC_Flags(IntEnum):
     XL_ACTIVATE_NONE = 0
@@ -285,16 +284,19 @@
     XL_HWTYPE_VN1611 = 63
     XL_HWTYPE_VN5240 = 64
     XL_HWTYPE_VN5610 = 65
     XL_HWTYPE_VN5620 = 66
     XL_HWTYPE_VN7570 = 67
     XL_HWTYPE_VN5650 = 68
     XL_HWTYPE_IPCLIENT = 69
+    XL_HWTYPE_VN5611 = 70
     XL_HWTYPE_IPSERVER = 71
+    XL_HWTYPE_VN5612 = 72
     XL_HWTYPE_VX1121 = 73
+    XL_HWTYPE_VN5601 = 74
     XL_HWTYPE_VX1131 = 75
     XL_HWTYPE_VT6204 = 77
     XL_HWTYPE_VN1630_LOG = 79
     XL_HWTYPE_VN7610 = 81
     XL_HWTYPE_VN7572 = 83
     XL_HWTYPE_VN8972 = 85
     XL_HWTYPE_VN0601 = 87
@@ -313,14 +315,16 @@
     XL_HWTYPE_VT6104A = 108
     XL_HWTYPE_VN5430 = 109
     XL_HWTYPE_VTSSERVICE = 110
     XL_HWTYPE_VN1530 = 112
     XL_HWTYPE_VN1531 = 113
     XL_HWTYPE_VX1161A = 114
     XL_HWTYPE_VX1161B = 115
+    XL_HWTYPE_VGNSS = 116
+    XL_HWTYPE_VXLAPINIC = 118
     XL_MAX_HWTYPE = 120
 
 
 class XL_SyncPulseSource(IntEnum):
     XL_SYNC_PULSE_EXTERNAL = 0
     XL_SYNC_PULSE_OUR = 1
     XL_SYNC_PULSE_OUR_SHARED = 2
```

### Comparing `python-can-4.1.0a2/can/interfaces/vector/xldriver.py` & `python-can-4.2.0rc0/can/interfaces/vector/xldriver.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 """
 
 # Import Standard Python Modules
 # ==============================
 import ctypes
 import logging
 import platform
-from .exceptions import VectorOperationError, VectorInitializationError
+
+from .exceptions import VectorInitializationError, VectorOperationError
 
 # Define Module Logger
 # ====================
 LOG = logging.getLogger(__name__)
 
 # Vector XL API Definitions
 # =========================
@@ -197,15 +198,25 @@
 xlCanSetChannelParams = _xlapi_dll.xlCanSetChannelParams
 xlCanSetChannelParams.argtypes = [
     xlclass.XLportHandle,
     xlclass.XLaccess,
     ctypes.POINTER(xlclass.XLchipParams),
 ]
 xlCanSetChannelParams.restype = xlclass.XLstatus
-xlCanSetChannelParams.errcheck = check_status_operation
+xlCanSetChannelParams.errcheck = check_status_initialization
+
+xlCanSetChannelParamsC200 = _xlapi_dll.xlCanSetChannelParamsC200
+xlCanSetChannelParamsC200.argtypes = [
+    xlclass.XLportHandle,
+    xlclass.XLaccess,
+    ctypes.c_ubyte,
+    ctypes.c_ubyte,
+]
+xlCanSetChannelParams.restype = xlclass.XLstatus
+xlCanSetChannelParams.errcheck = check_status_initialization
 
 xlCanTransmit = _xlapi_dll.xlCanTransmit
 xlCanTransmit.argtypes = [
     xlclass.XLportHandle,
     xlclass.XLaccess,
     ctypes.POINTER(ctypes.c_uint),
     ctypes.POINTER(xlclass.XLevent),
```

### Comparing `python-can-4.1.0a2/can/interfaces/virtual.py` & `python-can-4.2.0rc0/can/interfaces/virtual.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 This module implements an OS and hardware independent
 virtual CAN interface for testing purposes.
 
 Any VirtualBus instances connecting to the same channel
 and reside in the same process will receive the same messages.
 """
 
-from typing import Any, Dict, List, Optional, Tuple, TYPE_CHECKING
-
-from copy import deepcopy
 import logging
-import time
 import queue
-from threading import RLock
+import time
+from copy import deepcopy
 from random import randint
+from threading import RLock
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 from can import CanOperationError
 from can.bus import BusABC
 from can.message import Message
 from can.typechecking import AutoDetectedConfig
 
 logger = logging.getLogger(__name__)
@@ -70,15 +69,14 @@
         self.channel_id = channel
         self.channel_info = f"Virtual bus channel {self.channel_id}"
         self.receive_own_messages = receive_own_messages
         self.preserve_timestamps = preserve_timestamps
         self._open = True
 
         with channels_lock:
-
             # Create a new channel if one does not exist
             if self.channel_id not in channels:
                 channels[self.channel_id] = []
             self.channel = channels[self.channel_id]
 
             self.queue: queue.Queue[Message] = queue.Queue(rx_queue_size)
             self.channel.append(self.queue)
```

### Comparing `python-can-4.1.0a2/can/io/asc.py` & `python-can-4.2.0rc0/can/io/asc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
 Contains handling of ASC logging files.
 
 Example .asc files:
-    - https://bitbucket.org/tobylorenz/vector_asc/src/47556e1a6d32c859224ca62d075e1efcc67fa690/src/Vector/ASC/tests/unittests/data/CAN_Log_Trigger_3_2.asc?at=master&fileviewer=file-view-default
+    - https://bitbucket.org/tobylorenz/vector_asc/src/master/src/Vector/ASC/tests/unittests/data/
     - under `test/data/logfile.asc`
 """
+import logging
 import re
-from typing import Any, Generator, List, Optional, Dict, Union, TextIO
-
-from datetime import datetime
 import time
-import logging
+from datetime import datetime
+from typing import Any, Dict, Generator, List, Optional, TextIO, Union
 
 from ..message import Message
-from ..util import channel2int, len2dlc, dlc2len
-from .generic import FileIOMessageWriter, MessageReader
 from ..typechecking import StringPathLike
-
+from ..util import channel2int, dlc2len, len2dlc
+from .generic import FileIOMessageWriter, MessageReader
 
 CAN_MSG_EXT = 0x80000000
 CAN_ID_MASK = 0x1FFFFFFF
 BASE_HEX = 16
 BASE_DEC = 10
 
 logger = logging.getLogger("can.io.asc")
@@ -35,15 +33,14 @@
     file: TextIO
 
     def __init__(
         self,
         file: Union[StringPathLike, TextIO],
         base: str = "hex",
         relative_timestamp: bool = True,
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or as file-like object to read from
                      If this is a file-like object, is has to opened in text
                      read mode, not binary read mode.
         :param base: Select the base(hex or dec) of id and data.
@@ -89,31 +86,30 @@
                 self.start_time = (
                     0.0
                     if self.relative_timestamp
                     else self._datetime_to_timestamp(self.date)
                 )
                 continue
 
-            elif base_match:
+            if base_match:
                 base = base_match.group("base")
                 timestamp_format = base_match.group("timestamp_format")
                 self.base = base
                 self._converted_base = self._check_base(self.base)
                 self.timestamps_format = timestamp_format or "absolute"
                 continue
 
-            elif comment_match:
+            if comment_match:
                 continue
 
-            elif events_match:
+            if events_match:
                 self.internal_events_logged = events_match.group("no_events") is None
                 break
 
-            else:
-                break
+            break
 
     @staticmethod
     def _datetime_to_timestamp(datetime_string: str) -> float:
         # ugly locale independent solution
         month_map = {
             "Jan": 1,
             "Feb": 2,
@@ -172,15 +168,14 @@
         for byte in data[:data_length]:
             frame.append(int(byte, self._converted_base))
         msg_kwargs["data"] = frame
 
     def _process_classic_can_frame(
         self, line: str, msg_kwargs: Dict[str, Any]
     ) -> Message:
-
         # CAN error frame
         if line.strip()[0:10].lower() == "errorframe":
             # Error Frame
             msg_kwargs["is_error_frame"] = True
         else:
             abr_id_str, direction, rest_of_message = line.split(None, 2)
             msg_kwargs["is_rx"] = direction == "Rx"
@@ -350,15 +345,14 @@
     FORMAT_DATE = "%a %b %d %I:%M:%S.{} %p %Y"
     FORMAT_EVENT = "{timestamp: 9.6f} {message}\n"
 
     def __init__(
         self,
         file: Union[StringPathLike, TextIO],
         channel: int = 1,
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or as file-like object to write to
                      If this is a file-like object, is has to opened in text
                      write mode, not binary write mode.
         :param channel: a default channel to use when the message does not
@@ -422,15 +416,14 @@
         # turn into relative timestamps if necessary
         if timestamp >= self.started:
             timestamp -= self.started
         line = self.FORMAT_EVENT.format(timestamp=timestamp, message=message)
         self.file.write(line)
 
     def on_message_received(self, msg: Message) -> None:
-
         if msg.is_error_frame:
             self.log_event(f"{self.channel}  ErrorFrame", msg.timestamp)
             return
         if msg.is_remote_frame:
             dtype = f"r {msg.dlc:x}"  # New after v8.5
             data: List[str] = []
         else:
```

### Comparing `python-can-4.1.0a2/can/io/blf.py` & `python-can-4.2.0rc0/can/io/blf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 
 The file starts with a header. The rest is one or more "log containers"
 which consists of a header and some zlib compressed data, usually up to 128 kB
 of uncompressed data each. This data contains the actual CAN messages and other
 objects types.
 """
 
-import struct
-import zlib
 import datetime
-import time
 import logging
-from typing import List, BinaryIO, Generator, Union, Tuple, Optional, cast, Any
+import struct
+import time
+import zlib
+from typing import Any, BinaryIO, Generator, List, Optional, Tuple, Union, cast
 
 from ..message import Message
-from ..util import len2dlc, dlc2len, channel2int
 from ..typechecking import StringPathLike
+from ..util import channel2int, dlc2len, len2dlc
 from .generic import FileIOMessageWriter, MessageReader
 
-
 TSystemTime = Tuple[int, int, int, int, int, int, int, int]
 
 
 class BLFParseError(Exception):
     """BLF file could not be parsed correctly."""
 
 
@@ -142,15 +141,14 @@
     """
 
     file: BinaryIO
 
     def __init__(
         self,
         file: Union[StringPathLike, BinaryIO],
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or as file-like object to read from
                      If this is a file-like object, is has to opened in binary
                      read mode, not text read mode.
         """
@@ -371,15 +369,14 @@
 
     def __init__(
         self,
         file: Union[StringPathLike, BinaryIO],
         append: bool = False,
         channel: int = 1,
         compression_level: int = -1,
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or as file-like object to write to
                      If this is a file-like object, is has to opened in mode "wb+".
         :param channel:
             Default channel to log as if not specified by the interface.
```

### Comparing `python-can-4.1.0a2/can/io/canutils.py` & `python-can-4.2.0rc0/can/io/canutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 This module works with CAN data in ASCII log files (*.log).
 It is is compatible with "candump -L" from the canutils program
 (https://github.com/linux-can/can-utils).
 """
 
 import logging
-from typing import Generator, TextIO, Union, Any
+from typing import Any, Generator, TextIO, Union
 
 from can.message import Message
-from .generic import FileIOMessageWriter, MessageReader
+
 from ..typechecking import StringPathLike
+from .generic import FileIOMessageWriter, MessageReader
 
 log = logging.getLogger("can.io.canutils")
 
 CAN_MSG_EXT = 0x80000000
 CAN_ERR_FLAG = 0x20000000
 CAN_ERR_BUSERROR = 0x00000080
 CAN_ERR_DLC = 8
@@ -33,27 +34,25 @@
     """
 
     file: TextIO
 
     def __init__(
         self,
         file: Union[StringPathLike, TextIO],
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or as file-like object to read from
                      If this is a file-like object, is has to opened in text
                      read mode, not binary read mode.
         """
         super().__init__(file, mode="r")
 
     def __iter__(self) -> Generator[Message, None, None]:
         for line in self.file:
-
             # skip empty lines
             temp = line.strip()
             if not temp:
                 continue
 
             channel_string: str
             if temp[-2:].lower() in (" r", " t"):
@@ -133,15 +132,14 @@
     """
 
     def __init__(
         self,
         file: Union[StringPathLike, TextIO],
         channel: str = "vcan0",
         append: bool = False,
-        *args: Any,
         **kwargs: Any,
     ):
         """
         :param file: a path-like object or as file-like object to write to
                      If this is a file-like object, is has to opened in text
                      write mode, not binary write mode.
         :param channel: a default channel to use when the message does not
@@ -166,22 +164,22 @@
         else:
             timestamp = msg.timestamp
 
         channel = msg.channel if msg.channel is not None else self.channel
         if isinstance(channel, int) or isinstance(channel, str) and channel.isdigit():
             channel = f"can{channel}"
 
-        framestr = "(%f) %s" % (timestamp, channel)
+        framestr = f"({timestamp:f}) {channel}"
 
         if msg.is_error_frame:
-            framestr += " %08X#" % (CAN_ERR_FLAG | CAN_ERR_BUSERROR)
+            framestr += f" {CAN_ERR_FLAG | CAN_ERR_BUSERROR:08X}#"
         elif msg.is_extended_id:
-            framestr += " %08X#" % (msg.arbitration_id)
+            framestr += f" {msg.arbitration_id:08X}#"
         else:
-            framestr += " %03X#" % (msg.arbitration_id)
+            framestr += f" {msg.arbitration_id:03X}#"
 
         if msg.is_error_frame:
             eol = "\n"
         else:
             eol = " R\n" if msg.is_rx else " T\n"
 
         if msg.is_remote_frame:
@@ -189,11 +187,11 @@
         else:
             if msg.is_fd:
                 fd_flags = 0
                 if msg.bitrate_switch:
                     fd_flags |= CANFD_BRS
                 if msg.error_state_indicator:
                     fd_flags |= CANFD_ESI
-                framestr += "#%X" % fd_flags
+                framestr += f"#{fd_flags:X}"
             framestr += f"{msg.data.hex().upper()}{eol}"
 
         self.file.write(framestr)
```

### Comparing `python-can-4.1.0a2/can/io/csv.py` & `python-can-4.2.0rc0/can/io/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 TODO: This module could use https://docs.python.org/2/library/csv.html#module-csv
       to allow different delimiters for writing, special escape chars to circumvent
       the base64 encoding and use csv.Sniffer to automatically deduce the delimiters
       of a CSV file.
 """
 
-from base64 import b64encode, b64decode
-from typing import TextIO, Generator, Union, Any
+from base64 import b64decode, b64encode
+from typing import Any, Generator, TextIO, Union
 
 from can.message import Message
-from .generic import FileIOMessageWriter, MessageReader
+
 from ..typechecking import StringPathLike
+from .generic import FileIOMessageWriter, MessageReader
 
 
 class CSVReader(MessageReader):
     """Iterator over CAN messages from a .csv file that was
     generated by :class:`~can.CSVWriter` or that uses the same
     format as described there. Assumes that there is a header
     and thus skips the first line.
@@ -27,15 +28,14 @@
     """
 
     file: TextIO
 
     def __init__(
         self,
         file: Union[StringPathLike, TextIO],
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or as file-like object to read from
                      If this is a file-like object, is has to opened in text
                      read mode, not binary read mode.
         """
@@ -46,15 +46,14 @@
         try:
             next(self.file)
         except StopIteration:
             # don't crash on a file with only a header
             return
 
         for line in self.file:
-
             timestamp, arbitration_id, extended, remote, error, dlc, data = line.split(
                 ","
             )
 
             yield Message(
                 timestamp=float(timestamp),
                 is_remote_frame=(remote == "1"),
@@ -91,15 +90,14 @@
 
     file: TextIO
 
     def __init__(
         self,
         file: Union[StringPathLike, TextIO],
         append: bool = False,
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object or a file-like object to write to.
                      If this is a file-like object, is has to open in text
                      write mode, not binary write mode.
         :param bool append: if set to `True` messages are appended to
```

### Comparing `python-can-4.1.0a2/can/io/generic.py` & `python-can-4.2.0rc0/can/io/generic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 """Contains generic base classes for file IO."""
-
+import locale
 from abc import ABCMeta
+from types import TracebackType
 from typing import (
-    Optional,
-    cast,
+    Any,
+    ContextManager,
     Iterable,
+    Optional,
     Type,
-    ContextManager,
-    Any,
+    cast,
 )
+
 from typing_extensions import Literal
-from types import TracebackType
 
-import can
-import can.typechecking
+from .. import typechecking
+from ..listener import Listener
+from ..message import Message
 
 
 class BaseIOHandler(ContextManager, metaclass=ABCMeta):
     """A generic file handler that can be used for reading and writing.
 
     Can be used as a context manager.
 
     :attr file:
         the file-like object that is kept internally, or `None` if none
         was opened
     """
 
-    file: Optional[can.typechecking.FileLike]
+    file: Optional[typechecking.FileLike]
 
     def __init__(
         self,
-        file: Optional[can.typechecking.AcceptedIOType],
+        file: Optional[typechecking.AcceptedIOType],
         mode: str = "rt",
-        *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         """
         :param file: a path-like object to open a file, a file-like object
                      to be used as a file or `None` to not use a file at all
         :param mode: the mode that should be used to open the file, see
                      :func:`open`, ignored if *file* is `None`
         """
         if file is None or (hasattr(file, "read") and hasattr(file, "write")):
             # file is None or some file-like object
-            self.file = cast(Optional[can.typechecking.FileLike], file)
+            self.file = cast(Optional[typechecking.FileLike], file)
         else:
+            encoding: Optional[str] = (
+                None
+                if "b" in mode
+                else kwargs.get("encoding", locale.getpreferredencoding(False))
+            )
             # pylint: disable=consider-using-with
             # file is some path-like object
             self.file = cast(
-                can.typechecking.FileLike,
-                open(cast(can.typechecking.StringPathLike, file), mode),
+                typechecking.FileLike,
+                open(cast(typechecking.StringPathLike, file), mode, encoding=encoding),
             )
 
         # for multiple inheritance
         super().__init__()
 
     def __enter__(self) -> "BaseIOHandler":
         return self
@@ -70,41 +76,34 @@
     def stop(self) -> None:
         """Closes the underlying file-like object and flushes it, if it was opened in write mode."""
         if self.file is not None:
             # this also implies a flush()
             self.file.close()
 
 
-# pylint: disable=abstract-method,too-few-public-methods
-class MessageWriter(BaseIOHandler, can.Listener, metaclass=ABCMeta):
+class MessageWriter(BaseIOHandler, Listener, metaclass=ABCMeta):
     """The base class for all writers."""
 
-    file: Optional[can.typechecking.FileLike]
+    file: Optional[typechecking.FileLike]
 
 
-# pylint: disable=abstract-method,too-few-public-methods
 class FileIOMessageWriter(MessageWriter, metaclass=ABCMeta):
     """A specialized base class for all writers with file descriptors."""
 
-    file: can.typechecking.FileLike
+    file: typechecking.FileLike
 
     def __init__(
-        self,
-        file: can.typechecking.AcceptedIOType,
-        mode: str = "wt",
-        *args: Any,
-        **kwargs: Any
+        self, file: typechecking.AcceptedIOType, mode: str = "wt", **kwargs: Any
     ) -> None:
         # Not possible with the type signature, but be verbose for user-friendliness
         if file is None:
             raise ValueError("The given file cannot be None")
 
-        super().__init__(file, mode)
+        super().__init__(file, mode, **kwargs)
 
     def file_size(self) -> int:
         """Return an estimate of the current file size in bytes."""
         return self.file.tell()
 
 
-# pylint: disable=too-few-public-methods
-class MessageReader(BaseIOHandler, Iterable[can.Message], metaclass=ABCMeta):
+class MessageReader(BaseIOHandler, Iterable[Message], metaclass=ABCMeta):
     """The base class for all readers."""
```

### Comparing `python-can-4.1.0a2/can/io/logger.py` & `python-can-4.2.0rc0/can/io/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """
 See the :class:`Logger` class.
 """
 
+import gzip
 import os
 import pathlib
 from abc import ABC, abstractmethod
 from datetime import datetime
-import gzip
-from typing import Any, Optional, Callable, Type, Tuple, cast, Dict, Set
-
 from types import TracebackType
+from typing import Any, Callable, Dict, Optional, Set, Tuple, Type, cast
 
-from typing_extensions import Literal
 from pkg_resources import iter_entry_points
+from typing_extensions import Literal
 
-from ..message import Message
 from ..listener import Listener
-from .generic import BaseIOHandler, FileIOMessageWriter, MessageWriter
+from ..message import Message
+from ..typechecking import AcceptedIOType, FileLike, StringPathLike
 from .asc import ASCWriter
 from .blf import BLFWriter
 from .canutils import CanutilsLogWriter
 from .csv import CSVWriter
-from .sqlite import SqliteWriter
+from .generic import BaseIOHandler, FileIOMessageWriter, MessageWriter
+from .mf4 import MF4Writer
 from .printer import Printer
+from .sqlite import SqliteWriter
 from .trc import TRCWriter
-from ..typechecking import StringPathLike, FileLike, AcceptedIOType
 
 
-class Logger(MessageWriter):  # pylint: disable=abstract-method
+class Logger(MessageWriter):
     """
     Logs CAN messages to a file.
 
     The format is determined from the file suffix which can be one of:
       * .asc: :class:`can.ASCWriter`
       * .blf :class:`can.BLFWriter`
       * .csv: :class:`can.CSVWriter`
       * .db: :class:`can.SqliteWriter`
       * .log :class:`can.CanutilsLogWriter`
       * .trc :class:`can.TRCWriter`
       * .txt :class:`can.Printer`
+      * .mf4 :class:`can.MF4Writer` (optional, depends on asammdf)
 
     Any of these formats can be used with gzip compression by appending
     the suffix .gz (e.g. filename.asc.gz). However, third-party tools might not
     be able to read these files.
 
     The **filename** may also be *None*, to fall back to :class:`can.Printer`.
 
@@ -56,57 +57,61 @@
     fetched_plugins = False
     message_writers: Dict[str, Type[MessageWriter]] = {
         ".asc": ASCWriter,
         ".blf": BLFWriter,
         ".csv": CSVWriter,
         ".db": SqliteWriter,
         ".log": CanutilsLogWriter,
+        ".mf4": MF4Writer,
         ".trc": TRCWriter,
         ".txt": Printer,
     }
 
     @staticmethod
     def __new__(  # type: ignore
-        cls: Any, filename: Optional[StringPathLike], *args: Any, **kwargs: Any
+        cls: Any, filename: Optional[StringPathLike], **kwargs: Any
     ) -> MessageWriter:
         """
-        :param filename: the filename/path of the file to write to,
-                         may be a path-like object or None to
-                         instantiate a :class:`~can.Printer`
-        :raises ValueError: if the filename's suffix is of an unknown file type
+        :param filename:
+            the filename/path of the file to write to,
+            may be a path-like object or None to
+            instantiate a :class:`~can.Printer`
+        :raises ValueError:
+            if the filename's suffix is of an unknown file type
         """
         if filename is None:
-            return Printer(*args, **kwargs)
+            return Printer(**kwargs)
 
         if not Logger.fetched_plugins:
             Logger.message_writers.update(
                 {
                     writer.name: writer.load()
                     for writer in iter_entry_points("can.io.message_writer")
                 }
             )
             Logger.fetched_plugins = True
 
         suffix = pathlib.PurePath(filename).suffix.lower()
 
         file_or_filename: AcceptedIOType = filename
         if suffix == ".gz":
-            suffix, file_or_filename = Logger.compress(filename, *args, **kwargs)
+            suffix, file_or_filename = Logger.compress(filename, **kwargs)
 
         try:
-            return Logger.message_writers[suffix](file_or_filename, *args, **kwargs)
+            LoggerType = Logger.message_writers[suffix]
+            if LoggerType is None:
+                raise ValueError(f'failed to import logger for extension "{suffix}"')
+            return LoggerType(file=file_or_filename, **kwargs)
         except KeyError:
             raise ValueError(
                 f'No write support for this unknown log format "{suffix}"'
             ) from None
 
     @staticmethod
-    def compress(
-        filename: StringPathLike, *args: Any, **kwargs: Any
-    ) -> Tuple[str, FileLike]:
+    def compress(filename: StringPathLike, **kwargs: Any) -> Tuple[str, FileLike]:
         """
         Return the suffix and io object of the decompressed file.
         File will automatically recompress upon close.
         """
         real_suffix = pathlib.Path(filename).suffixes[-2].lower()
         if real_suffix in (".blf", ".db"):
             raise ValueError(
@@ -150,19 +155,18 @@
     #: delegates to this callable. The parameters passed to the callable are those
     #: passed to :meth:`~BaseRotatingLogger.rotate`.
     rotator: Optional[Callable[[StringPathLike, StringPathLike], None]] = None
 
     #: An integer counter to track the number of rollovers.
     rollover_count: int = 0
 
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         Listener.__init__(self)
-        BaseIOHandler.__init__(self, None)
+        BaseIOHandler.__init__(self, file=None)
 
-        self.writer_args = args
         self.writer_kwargs = kwargs
 
         # Expected to be set by the subclass
         self._writer: FileIOMessageWriter = None  # type: ignore
 
     @property
     def writer(self) -> FileIOMessageWriter:
@@ -180,15 +184,15 @@
 
         :param default_name:
             The default name for the log file.
         """
         if not callable(self.namer):
             return default_name
 
-        return self.namer(default_name)
+        return self.namer(default_name)  # pylint: disable=not-callable
 
     def rotate(self, source: StringPathLike, dest: StringPathLike) -> None:
         """When rotating, rotate the current log.
 
         The default implementation calls the :attr:`rotator` attribute of the
         handler, if it's callable, passing the `source` and `dest` arguments to
         it. If the attribute isn't callable (the default is :obj:`None`), the source
@@ -201,15 +205,15 @@
             The destination filename. This is normally
             what the source is rotated to, e.g. `"test_#001.log"`.
         """
         if not callable(self.rotator):
             if os.path.exists(source):
                 os.rename(source, dest)
         else:
-            self.rotator(source, dest)
+            self.rotator(source, dest)  # pylint: disable=not-callable
 
     def on_message_received(self, msg: Message) -> None:
         """This method is called to handle the given message.
 
         :param msg:
             the delivered message
         """
@@ -230,21 +234,21 @@
             The log file format is defined by the suffix of `filename`.
         :return:
             An instance of a writer class.
         """
         suffix = "".join(pathlib.Path(filename).suffixes[-2:]).lower()
 
         if suffix in self._supported_formats:
-            logger = Logger(filename, *self.writer_args, **self.writer_kwargs)
+            logger = Logger(filename=filename, **self.writer_kwargs)
             if isinstance(logger, FileIOMessageWriter):
                 return logger
             elif isinstance(logger, Printer) and logger.file is not None:
                 return cast(FileIOMessageWriter, logger)
 
-        raise Exception(
+        raise ValueError(
             f'The log format "{suffix}" '
             f"is not supported by {self.__class__.__name__}. "
             f"{self.__class__.__name__} supports the following formats: "
             f"{', '.join(self._supported_formats)}"
         )
 
     def stop(self) -> None:
@@ -319,26 +323,25 @@
 
     _supported_formats = {".asc", ".blf", ".csv", ".log", ".txt"}
 
     def __init__(
         self,
         base_filename: StringPathLike,
         max_bytes: int = 0,
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param base_filename:
             A path-like object for the base filename. The log file format is defined by
             the suffix of `base_filename`.
         :param max_bytes:
             The size threshold at which a new log file shall be created. If set to 0, no
             rollover will be performed.
         """
-        super().__init__(*args, **kwargs)
+        super().__init__(**kwargs)
 
         self.base_filename = os.path.abspath(base_filename)
         self.max_bytes = max_bytes
 
         self._writer = self._get_new_writer(self.base_filename)
 
     def should_rollover(self, msg: Message) -> bool:
```

### Comparing `python-can-4.1.0a2/can/io/player.py` & `python-can-4.2.0rc0/can/io/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """
 This module contains the generic :class:`LogReader` as
 well as :class:`MessageSync` which plays back messages
-in the recorded order an time intervals.
+in the recorded order and time intervals.
 """
 import gzip
 import pathlib
 import time
 import typing
 
 from pkg_resources import iter_entry_points
 
-from .generic import MessageReader
+from ..message import Message
+from ..typechecking import AcceptedIOType, FileLike, StringPathLike
 from .asc import ASCReader
 from .blf import BLFReader
 from .canutils import CanutilsLogReader
 from .csv import CSVReader
+from .generic import MessageReader
+from .mf4 import MF4Reader
 from .sqlite import SqliteReader
 from .trc import TRCReader
-from ..typechecking import StringPathLike, FileLike, AcceptedIOType
-from ..message import Message
 
 
 class LogReader(MessageReader):
     """
     Replay logged CAN messages from a file.
 
     The format is determined from the file suffix which can be one of:
       * .asc
       * .blf
       * .csv
       * .db
       * .log
+      * .mf4 (optional, depends on asammdf)
       * .trc
 
     Gzip compressed files can be used as long as the original
     files suffix is one of the above (e.g. filename.asc.gz).
 
 
     Exposes a simple iterator interface, to use simply:
@@ -48,28 +50,28 @@
 
     .. note::
         This class itself is just a dispatcher, and any positional an keyword
         arguments are passed on to the returned instance.
     """
 
     fetched_plugins = False
-    message_readers: typing.Dict[str, typing.Type[MessageReader]] = {
+    message_readers: typing.Dict[str, typing.Optional[typing.Type[MessageReader]]] = {
         ".asc": ASCReader,
         ".blf": BLFReader,
         ".csv": CSVReader,
         ".db": SqliteReader,
         ".log": CanutilsLogReader,
+        ".mf4": MF4Reader,
         ".trc": TRCReader,
     }
 
     @staticmethod
     def __new__(  # type: ignore
         cls: typing.Any,
         filename: StringPathLike,
-        *args: typing.Any,
         **kwargs: typing.Any,
     ) -> MessageReader:
         """
         :param filename: the filename/path of the file to read from
         :raises ValueError: if the filename's suffix is of an unknown file type
         """
         if not LogReader.fetched_plugins:
@@ -83,19 +85,22 @@
 
         suffix = pathlib.PurePath(filename).suffix.lower()
 
         file_or_filename: AcceptedIOType = filename
         if suffix == ".gz":
             suffix, file_or_filename = LogReader.decompress(filename)
         try:
-            return LogReader.message_readers[suffix](file_or_filename, *args, **kwargs)
+            ReaderType = LogReader.message_readers[suffix]
         except KeyError:
             raise ValueError(
                 f'No read support for this unknown log format "{suffix}"'
             ) from None
+        if ReaderType is None:
+            raise ImportError(f"failed to import reader for extension {suffix}")
+        return ReaderType(file=file_or_filename, **kwargs)
 
     @staticmethod
     def decompress(
         filename: StringPathLike,
     ) -> typing.Tuple[str, typing.Union[str, FileLike]]:
         """
         Return the suffix and io object of the decompressed file.
@@ -105,15 +110,15 @@
 
         return real_suffix, gzip.open(filename, mode)
 
     def __iter__(self) -> typing.Generator[Message, None, None]:
         raise NotImplementedError()
 
 
-class MessageSync:  # pylint: disable=too-few-public-methods
+class MessageSync:
     """
     Used to iterate over some given messages in the recorded time.
     """
 
     def __init__(
         self,
         messages: typing.Iterable[Message],
@@ -136,15 +141,14 @@
 
     def __iter__(self) -> typing.Generator[Message, None, None]:
         t_wakeup = playback_start_time = time.perf_counter()
         recorded_start_time = None
         t_skipped = 0.0
 
         for message in self.raw_messages:
-
             # Work out the correct wait time
             if self.timestamps:
                 if recorded_start_time is None:
                     recorded_start_time = message.timestamp
 
                 t_wakeup = playback_start_time + (
                     message.timestamp - t_skipped - recorded_start_time
```

### Comparing `python-can-4.1.0a2/can/io/printer.py` & `python-can-4.2.0rc0/can/io/printer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 This Listener simply prints to stdout / the terminal or a file.
 """
 
 import logging
-
-from typing import Optional, TextIO, Union, Any, cast
+from typing import Any, Optional, TextIO, Union, cast
 
 from ..message import Message
-from .generic import MessageWriter
 from ..typechecking import StringPathLike
+from .generic import MessageWriter
 
 log = logging.getLogger("can.io.printer")
 
 
 class Printer(MessageWriter):
     """
     The Printer class is a subclass of :class:`~can.Listener` which simply prints
@@ -25,15 +24,14 @@
 
     file: Optional[TextIO]
 
     def __init__(
         self,
         file: Optional[Union[StringPathLike, TextIO]] = None,
         append: bool = False,
-        *args: Any,
         **kwargs: Any
     ) -> None:
         """
         :param file: An optional path-like object or a file-like object to "print"
                      to instead of writing to standard out (stdout).
                      If this is a file-like object, is has to be opened in text
                      write mode, not binary write mode.
```

### Comparing `python-can-4.1.0a2/can/io/sqlite.py` & `python-can-4.2.0rc0/can/io/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Implements an SQL database writer and reader for storing CAN messages.
 
 .. note:: The database schema is given in the documentation of the loggers.
 """
 
-import time
-import threading
 import logging
 import sqlite3
-from typing import Generator, Any
+import threading
+import time
+from typing import Any, Generator
 
 from can.listener import BufferedReader
 from can.message import Message
-from .generic import MessageWriter, MessageReader
+
 from ..typechecking import StringPathLike
+from .generic import MessageReader, MessageWriter
 
 log = logging.getLogger("can.io.sqlite")
 
 
 class SqliteReader(MessageReader):
     """
     Reads recorded CAN messages from a simple SQL database.
@@ -32,15 +33,14 @@
     .. note:: The database schema is given in the documentation of the loggers.
     """
 
     def __init__(
         self,
         file: StringPathLike,
         table_name: str = "messages",
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a `str`  path like object that points
                      to the database file to use
         :param str table_name: the name of the table to look for the messages
 
@@ -134,15 +134,14 @@
     MAX_BUFFER_SIZE_BEFORE_WRITES = 500
     """Maximum number of messages to buffer before writing to the database"""
 
     def __init__(
         self,
         file: StringPathLike,
         table_name: str = "messages",
-        *args: Any,
         **kwargs: Any,
     ) -> None:
         """
         :param file: a `str` or path like object that points
                      to the database file to use
         :param str table_name: the name of the table to store messages in
```

### Comparing `python-can-4.1.0a2/can/io/trc.py` & `python-can-4.2.0rc0/can/io/trc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-# coding: utf-8
-
 """
 Reader and writer for can logging files in peak trc format
 
 See https://www.peak-system.com/produktcd/Pdf/English/PEAK_CAN_TRC_File_Format.pdf
 for file format description
 
 Version 1.1 will be implemented as it is most commonly used
 """  # noqa
 
-from typing import Generator, Optional, Union, TextIO
-from datetime import datetime, timedelta
-from enum import Enum
-from io import TextIOWrapper
-import os
+import io
 import logging
+import os
+from datetime import datetime, timedelta, timezone
+from enum import Enum
+from typing import Callable, Dict, Generator, List, Optional, TextIO, Union
 
 from ..message import Message
-from ..util import channel2int
-from .generic import FileIOMessageWriter, MessageReader
 from ..typechecking import StringPathLike
-
+from ..util import channel2int, dlc2len, len2dlc
+from .generic import FileIOMessageWriter, MessageReader
 
 logger = logging.getLogger("can.io.trc")
 
 
 class TRCFileVersion(Enum):
     UNKNOWN = 0
     V1_0 = 100
     V1_1 = 101
     V1_2 = 102
     V1_3 = 103
     V2_0 = 200
     V2_1 = 201
 
+    def __ge__(self, other):
+        if self.__class__ is other.__class__:
+            return self.value >= other.value
+        return NotImplemented
+
 
 class TRCReader(MessageReader):
     """
     Iterator of CAN messages from a TRC logging file.
     """
 
     file: TextIO
@@ -47,118 +49,176 @@
         file: Union[StringPathLike, TextIO],
     ) -> None:
         """
         :param file: a path-like object or as file-like object to read from
                      If this is a file-like object, is has to opened in text
                      read mode, not binary read mode.
         """
-        super(TRCReader, self).__init__(file, mode="r")
+        super().__init__(file, mode="r")
         self.file_version = TRCFileVersion.UNKNOWN
+        self.start_time: Optional[datetime] = None
+        self.columns: Dict[str, int] = {}
 
         if not self.file:
             raise ValueError("The given file cannot be None")
 
+        self._parse_cols: Callable[[List[str]], Optional[Message]] = lambda x: None
+
     def _extract_header(self):
+        line = ""
         for line in self.file:
             line = line.strip()
             if line.startswith(";$FILEVERSION"):
-                logger.debug(f"TRCReader: Found file version '{line}'")
+                logger.debug("TRCReader: Found file version '%s'", line)
                 try:
                     file_version = line.split("=")[1]
                     if file_version == "1.1":
                         self.file_version = TRCFileVersion.V1_1
+                    elif file_version == "2.0":
+                        self.file_version = TRCFileVersion.V2_0
                     elif file_version == "2.1":
                         self.file_version = TRCFileVersion.V2_1
                     else:
                         self.file_version = TRCFileVersion.UNKNOWN
                 except IndexError:
                     logger.debug("TRCReader: Failed to parse version")
+            elif line.startswith(";$STARTTIME"):
+                logger.debug("TRCReader: Found start time '%s'", line)
+                try:
+                    self.start_time = datetime(
+                        1899, 12, 30, tzinfo=timezone.utc
+                    ) + timedelta(days=float(line.split("=")[1]))
+                except IndexError:
+                    logger.debug("TRCReader: Failed to parse start time")
+            elif line.startswith(";$COLUMNS"):
+                logger.debug("TRCReader: Found columns '%s'", line)
+                try:
+                    columns = line.split("=")[1].split(",")
+                    self.columns = {column: columns.index(column) for column in columns}
+                except IndexError:
+                    logger.debug("TRCReader: Failed to parse columns")
             elif line.startswith(";"):
                 continue
             else:
                 break
 
+        if self.file_version >= TRCFileVersion.V1_1:
+            if self.start_time is None:
+                raise ValueError("File has no start time information")
+
+        if self.file_version >= TRCFileVersion.V2_0:
+            if not self.columns:
+                raise ValueError("File has no column information")
+
         if self.file_version == TRCFileVersion.UNKNOWN:
             logger.info(
                 "TRCReader: No file version was found, so version 1.0 is assumed"
             )
             self._parse_cols = self._parse_msg_V1_0
         elif self.file_version == TRCFileVersion.V1_0:
             self._parse_cols = self._parse_msg_V1_0
         elif self.file_version == TRCFileVersion.V1_1:
             self._parse_cols = self._parse_cols_V1_1
-        elif self.file_version == TRCFileVersion.V2_1:
-            self._parse_cols = self._parse_cols_V2_1
+        elif self.file_version in [TRCFileVersion.V2_0, TRCFileVersion.V2_1]:
+            self._parse_cols = self._parse_cols_V2_x
         else:
             raise NotImplementedError("File version not fully implemented for reading")
 
         return line
 
-    def _parse_msg_V1_0(self, cols):
+    def _parse_msg_V1_0(self, cols: List[str]) -> Optional[Message]:
         arbit_id = cols[2]
         if arbit_id == "FFFFFFFF":
             logger.info("TRCReader: Dropping bus info line")
             return None
 
         msg = Message()
         msg.timestamp = float(cols[1]) / 1000
         msg.arbitration_id = int(arbit_id, 16)
         msg.is_extended_id = len(arbit_id) > 4
         msg.channel = 1
         msg.dlc = int(cols[3])
         msg.data = bytearray([int(cols[i + 4], 16) for i in range(msg.dlc)])
         return msg
 
-    def _parse_msg_V1_1(self, cols):
+    def _parse_msg_V1_1(self, cols: List[str]) -> Optional[Message]:
         arbit_id = cols[3]
 
         msg = Message()
-        msg.timestamp = float(cols[1]) / 1000
+        if isinstance(self.start_time, datetime):
+            msg.timestamp = (
+                self.start_time + timedelta(milliseconds=float(cols[1]))
+            ).timestamp()
+        else:
+            msg.timestamp = float(cols[1]) / 1000
         msg.arbitration_id = int(arbit_id, 16)
         msg.is_extended_id = len(arbit_id) > 4
         msg.channel = 1
         msg.dlc = int(cols[4])
         msg.data = bytearray([int(cols[i + 5], 16) for i in range(msg.dlc)])
         msg.is_rx = cols[2] == "Rx"
         return msg
 
-    def _parse_msg_V2_1(self, cols):
+    def _parse_msg_V2_x(self, cols: List[str]) -> Optional[Message]:
+        type_ = cols[self.columns["T"]]
+        bus = self.columns.get("B", None)
+
+        if "l" in self.columns:
+            length = int(cols[self.columns["l"]])
+            dlc = len2dlc(length)
+        elif "L" in self.columns:
+            dlc = int(cols[self.columns["L"]])
+            length = dlc2len(dlc)
+        else:
+            raise ValueError("No length/dlc columns present.")
+
         msg = Message()
-        msg.timestamp = float(cols[1]) / 1000
-        msg.arbitration_id = int(cols[4], 16)
-        msg.is_extended_id = len(cols[4]) > 4
-        msg.channel = int(cols[3])
-        msg.dlc = int(cols[7])
-        msg.data = bytearray([int(cols[i + 8], 16) for i in range(msg.dlc)])
-        msg.is_rx = cols[5] == "Rx"
+        if isinstance(self.start_time, datetime):
+            msg.timestamp = (
+                self.start_time + timedelta(milliseconds=float(cols[self.columns["O"]]))
+            ).timestamp()
+        else:
+            msg.timestamp = float(cols[1]) / 1000
+        msg.arbitration_id = int(cols[self.columns["I"]], 16)
+        msg.is_extended_id = len(cols[self.columns["I"]]) > 4
+        msg.channel = int(cols[bus]) if bus is not None else 1
+        msg.dlc = dlc
+        msg.data = bytearray(
+            [int(cols[i + self.columns["D"]], 16) for i in range(length)]
+        )
+        msg.is_rx = cols[self.columns["d"]] == "Rx"
+        msg.is_fd = type_ in ["FD", "FB", "FE", "BI"]
+        msg.bitrate_switch = type_ in ["FB", " FE"]
+        msg.error_state_indicator = type_ in ["FE", "BI"]
+
         return msg
 
-    def _parse_cols_V1_1(self, cols):
+    def _parse_cols_V1_1(self, cols: List[str]) -> Optional[Message]:
         dtype = cols[2]
-        if dtype == "Tx" or dtype == "Rx":
+        if dtype in ("Tx", "Rx"):
             return self._parse_msg_V1_1(cols)
         else:
-            logger.info(f"TRCReader: Unsupported type '{dtype}'")
+            logger.info("TRCReader: Unsupported type '%s'", dtype)
             return None
 
-    def _parse_cols_V2_1(self, cols):
-        dtype = cols[2]
-        if dtype == "DT":
-            return self._parse_msg_V2_1(cols)
+    def _parse_cols_V2_x(self, cols: List[str]) -> Optional[Message]:
+        dtype = cols[self.columns["T"]]
+        if dtype in ["DT", "FD", "FB"]:
+            return self._parse_msg_V2_x(cols)
         else:
-            logger.info(f"TRCReader: Unsupported type '{dtype}'")
+            logger.info("TRCReader: Unsupported type '%s'", dtype)
             return None
 
-    def _parse_line(self, line):
-        logger.debug(f"TRCReader: Parse '{line}'")
+    def _parse_line(self, line: str) -> Optional[Message]:
+        logger.debug("TRCReader: Parse '%s'", line)
         try:
             cols = line.split()
             return self._parse_cols(cols)
         except IndexError:
-            logger.warning(f"TRCReader: Failed to parse message '{line}'")
+            logger.warning("TRCReader: Failed to parse message '%s'", line)
             return None
 
     def __iter__(self) -> Generator[Message, None, None]:
         first_line = self._extract_header()
 
         if first_line is not None:
             msg = self._parse_line(first_line)
@@ -207,91 +267,74 @@
         """
         :param file: a path-like object or as file-like object to write to
                      If this is a file-like object, is has to opened in text
                      write mode, not binary write mode.
         :param channel: a default channel to use when the message does not
                         have a channel set
         """
-        super(TRCWriter, self).__init__(file, mode="w")
+        super().__init__(file, mode="w")
         self.channel = channel
-        if type(file) is str:
-            self.filepath = os.path.abspath(file)
-        elif type(file) is TextIOWrapper:
-            self.filepath = "Unknown"
-            logger.warning("TRCWriter: Text mode io can result in wrong line endings")
-            logger.debug(
-                f"TRCWriter: Text mode io line ending setting: {file.newlines}"
-            )
+
+        if isinstance(self.file, io.TextIOWrapper):
+            self.file.reconfigure(newline="\r\n")
         else:
-            self.filepath = "Unknown"
+            raise TypeError("File must be opened in text mode.")
 
+        self.filepath = os.path.abspath(self.file.name)
         self.header_written = False
         self.msgnr = 0
         self.first_timestamp = None
         self.file_version = TRCFileVersion.V2_1
+        self._msg_fmt_string = self.FORMAT_MESSAGE_V1_0
         self._format_message = self._format_message_init
 
-    def _write_line(self, line: str) -> None:
-        self.file.write(line + "\r\n")
-
-    def _write_lines(self, lines: list) -> None:
-        for line in lines:
-            self._write_line(line)
-
-    def _write_header_V1_0(self, start_time: timedelta) -> None:
-        self._write_line(
-            ";##########################################################################"
-        )
-        self._write_line(f";   {self.filepath}")
-        self._write_line(";")
-        self._write_line(";    Generated by python-can TRCWriter")
-        self._write_line(f";    Start time: {start_time}")
-        self._write_line(";    PCAN-Net: N/A")
-        self._write_line(";")
-        self._write_line(";    Columns description:")
-        self._write_line(";    ~~~~~~~~~~~~~~~~~~~~~")
-        self._write_line(";    +-current number in actual sample")
-        self._write_line(";    |     +time offset of message (ms)")
-        self._write_line(";    |     |        +ID of message (hex)")
-        self._write_line(";    |     |        |    +data length code")
-        self._write_line(";    |     |        |    |  +data bytes (hex) ...")
-        self._write_line(";    |     |        |    |  |")
-        self._write_line(";----+- ---+--- ----+--- + -+ -- -- ...")
-
-    def _write_header_V2_1(self, header_time: timedelta, start_time: datetime) -> None:
-        milliseconds = int(
-            (header_time.seconds * 1000) + (header_time.microseconds / 1000)
-        )
-
-        self._write_line(";$FILEVERSION=2.1")
-        self._write_line(f";$STARTTIME={header_time.days}.{milliseconds}")
-        self._write_line(";$COLUMNS=N,O,T,B,I,d,R,L,D")
-        self._write_line(";")
-        self._write_line(f";   {self.filepath}")
-        self._write_line(";")
-        self._write_line(f";   Start time: {start_time}")
-        self._write_line(";   Generated by python-can TRCWriter")
-        self._write_line(
-            ";-------------------------------------------------------------------------------"
-        )
-        self._write_line(";   Bus   Name            Connection               Protocol")
-        self._write_line(";   N/A   N/A             N/A                      N/A")
-        self._write_line(
-            ";-------------------------------------------------------------------------------"
-        )
-        self._write_lines(
-            [
-                ";   Message   Time    Type    ID     Rx/Tx",
-                ";   Number    Offset  |  Bus  [hex]  |  Reserved",
-                ";   |         [ms]    |  |    |      |  |  Data Length Code",
-                ";   |         |       |  |    |      |  |  |    Data [hex] ...",
-                ";   |         |       |  |    |      |  |  |    |",
-                ";---+-- ------+------ +- +- --+----- +- +- +--- +- -- -- -- -- -- -- --",
-            ]
-        )
+    def _write_header_V1_0(self, start_time: datetime) -> None:
+        lines = [
+            ";##########################################################################",
+            f";   {self.filepath}",
+            ";",
+            ";    Generated by python-can TRCWriter",
+            f";    Start time: {start_time}",
+            ";    PCAN-Net: N/A",
+            ";",
+            ";    Columns description:",
+            ";    ~~~~~~~~~~~~~~~~~~~~~",
+            ";    +-current number in actual sample",
+            ";    |     +time offset of message (ms",
+            ";    |     |        +ID of message (hex",
+            ";    |     |        |    +data length code",
+            ";    |     |        |    |  +data bytes (hex ...",
+            ";    |     |        |    |  |",
+            ";----+- ---+--- ----+--- + -+ -- -- ...",
+        ]
+        self.file.writelines(line + "\n" for line in lines)
+
+    def _write_header_V2_1(self, start_time: datetime) -> None:
+        header_time = start_time - datetime(year=1899, month=12, day=30)
+        lines = [
+            ";$FILEVERSION=2.1",
+            f";$STARTTIME={header_time/timedelta(days=1)}",
+            ";$COLUMNS=N,O,T,B,I,d,R,L,D",
+            ";",
+            f";   {self.filepath}",
+            ";",
+            f";   Start time: {start_time}",
+            ";   Generated by python-can TRCWriter",
+            ";-------------------------------------------------------------------------------",
+            ";   Bus   Name            Connection               Protocol",
+            ";   N/A   N/A             N/A                      N/A",
+            ";-------------------------------------------------------------------------------",
+            ";   Message   Time    Type    ID     Rx/Tx",
+            ";   Number    Offset  |  Bus  [hex]  |  Reserved",
+            ";   |         [ms]    |  |    |      |  |  Data Length Code",
+            ";   |         |       |  |    |      |  |  |    Data [hex] ...",
+            ";   |         |       |  |    |      |  |  |    |",
+            ";---+-- ------+------ +- +- --+----- +- +- +--- +- -- -- -- -- -- -- --",
+        ]
+        self.file.writelines(line + "\n" for line in lines)
 
     def _format_message_by_format(self, msg, channel):
         if msg.is_extended_id:
             arb_id = f"{msg.arbitration_id:07X}"
         else:
             arb_id = f"{msg.arbitration_id:04X}"
 
@@ -314,35 +357,33 @@
             self._msg_fmt_string = self.FORMAT_MESSAGE_V1_0
         elif self.file_version == TRCFileVersion.V2_1:
             self._format_message = self._format_message_by_format
             self._msg_fmt_string = self.FORMAT_MESSAGE
         else:
             raise NotImplementedError("File format is not supported")
 
-        return self._format_message(msg, channel)
+        return self._format_message_by_format(msg, channel)
 
     def write_header(self, timestamp: float) -> None:
         # write start of file header
-        ref_time = datetime(year=1899, month=12, day=30)
-        start_time = datetime.now() + timedelta(seconds=timestamp)
-        header_time = start_time - ref_time
+        start_time = datetime.utcfromtimestamp(timestamp)
 
         if self.file_version == TRCFileVersion.V1_0:
-            self._write_header_V1_0(header_time)
+            self._write_header_V1_0(start_time)
         elif self.file_version == TRCFileVersion.V2_1:
-            self._write_header_V2_1(header_time, start_time)
+            self._write_header_V2_1(start_time)
         else:
             raise NotImplementedError("File format is not supported")
         self.header_written = True
 
     def log_event(self, message: str, timestamp: float) -> None:
         if not self.header_written:
             self.write_header(timestamp)
 
-        self._write_line(message)
+        self.file.write(message + "\n")
 
     def on_message_received(self, msg: Message) -> None:
         if self.first_timestamp is None:
             self.first_timestamp = msg.timestamp
 
         if msg.is_error_frame:
             logger.warning("TRCWriter: Logging error frames is not implemented")
```

### Comparing `python-can-4.1.0a2/can/listener.py` & `python-can-4.2.0rc0/can/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 This module contains the implementation of `can.Listener` and some readers.
 """
 
+import asyncio
 import sys
 import warnings
-import asyncio
 from abc import ABCMeta, abstractmethod
-from queue import SimpleQueue, Empty
-from typing import Any, AsyncIterator, Awaitable, Optional
+from queue import Empty, SimpleQueue
+from typing import Any, AsyncIterator, Optional
 
-from can.message import Message
 from can.bus import BusABC
+from can.message import Message
 
 
 class Listener(metaclass=ABCMeta):
     """The basic listener that can be called directly to handle some
     CAN message::
 
         listener = SomeListener()
@@ -122,15 +122,17 @@
             return None
 
     def stop(self) -> None:
         """Prohibits any more additions to this reader."""
         self.is_stopped = True
 
 
-class AsyncBufferedReader(Listener):  # pylint: disable=abstract-method
+class AsyncBufferedReader(
+    Listener, AsyncIterator[Message]
+):  # pylint: disable=abstract-method
     """A message buffer for use with :mod:`asyncio`.
 
     See :ref:`asyncio` for how to use with :class:`can.Notifier`.
 
     Can also be used as an asynchronous iterator::
 
         async for msg in reader:
@@ -170,9 +172,9 @@
         :return: The CAN message.
         """
         return await self.buffer.get()
 
     def __aiter__(self) -> AsyncIterator[Message]:
         return self
 
-    def __anext__(self) -> Awaitable[Message]:
-        return self.buffer.get()
+    async def __anext__(self) -> Message:
+        return await self.buffer.get()
```

### Comparing `python-can-4.1.0a2/can/logconvert.py` & `python-can-4.2.0rc0/can/logconvert.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Convert a log file from one format to another.
 """
 
-import sys
 import argparse
 import errno
+import sys
 
-from can import LogReader, Logger, SizedRotatingLogger
+from can import Logger, LogReader, SizedRotatingLogger
 
 
 class ArgumentParser(argparse.ArgumentParser):
     def error(self, message):
         self.print_help(sys.stderr)
         self.exit(errno.EINVAL, f"{self.prog}: error: {message}\n")
 
@@ -42,25 +42,24 @@
         type=str,
         help="Output filename. The type is dependent on the suffix, see can.Logger.",
     )
 
     args = parser.parse_args()
 
     with LogReader(args.input) as reader:
-
         if args.file_size:
             logger = SizedRotatingLogger(
                 base_filename=args.output, max_bytes=args.file_size
             )
         else:
             logger = Logger(filename=args.output)
 
         with logger:
             try:
-                for m in reader:  # pylint: disable=not-an-iterable
+                for m in reader:
                     logger(m)
             except KeyboardInterrupt:
                 sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `python-can-4.1.0a2/can/logger.py` & `python-can-4.2.0rc0/can/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import argparse
+import errno
 import re
 import sys
-import argparse
 from datetime import datetime
-import errno
-from typing import Any, Dict, List, Union, Sequence, Tuple
+from typing import Any, Dict, List, Sequence, Tuple, Union
 
 import can
 from can.io import BaseRotatingLogger
 from can.io.generic import MessageWriter
+from can.util import cast_from_string
+
 from . import Bus, BusState, Logger, SizedRotatingLogger
 from .typechecking import CanFilter, CanFilters
 
 
 def _create_base_argument_parser(parser: argparse.ArgumentParser) -> None:
     """Adds common options to an argument parser."""
 
@@ -54,15 +56,15 @@
         "to opening the bus with `Bus('vector', channel=1, app_name='MyCanApp')",
     )
 
 
 def _append_filter_argument(
     parser: Union[
         argparse.ArgumentParser,
-        argparse._ArgumentGroup,  # pylint: disable=protected-access
+        argparse._ArgumentGroup,
     ],
     *args: str,
     **kwargs: Any,
 ) -> None:
     """Adds the ``filter`` option to an argument parser."""
 
     parser.add_argument(
@@ -130,26 +132,15 @@
 
     def _split_arg(_arg: str) -> Tuple[str, str]:
         left, right = _arg.split("=", 1)
         return left.lstrip("--").replace("-", "_"), right
 
     args: Dict[str, Union[str, int, float, bool]] = {}
     for key, string_val in map(_split_arg, unknown_args):
-        if re.match(r"^[-+]?\d+$", string_val):
-            # value is integer
-            args[key] = int(string_val)
-        elif re.match(r"^[-+]?\d*\.\d+$", string_val):
-            # value is float
-            args[key] = float(string_val)
-        elif re.match(r"^(?:True|False)$", string_val):
-            # value is bool
-            args[key] = string_val == "True"
-        else:
-            # value is string
-            args[key] = string_val
+        args[key] = cast_from_string(string_val)
     return args
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(
         description="Log CAN traffic, printing messages to stdout or to a "
         "given file.",
```

### Comparing `python-can-4.1.0a2/can/message.py` & `python-can-4.2.0rc0/can/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 This module contains the implementation of :class:`can.Message`.
 
 .. note::
     Could use `@dataclass <https://docs.python.org/3.7/library/dataclasses.html>`__
     starting with Python 3.7.
 """
 
+from copy import deepcopy
+from math import isinf, isnan
 from typing import Optional
 
 from . import typechecking
 
-from copy import deepcopy
-from math import isinf, isnan
-
 
 class Message:  # pylint: disable=too-many-instance-attributes; OK for a dataclass
     """
     The :class:`~can.Message` object is used to represent CAN messages for
     sending, receiving and other purposes like converting between different
     logging formats.
 
@@ -224,17 +223,15 @@
             data=deepcopy(self.data, memo),
             is_fd=self.is_fd,
             is_rx=self.is_rx,
             bitrate_switch=self.bitrate_switch,
             error_state_indicator=self.error_state_indicator,
         )
 
-    def _check(
-        self,
-    ) -> None:  # pylint: disable=too-many-branches; it's still simple code
+    def _check(self) -> None:
         """Checks if the message parameters are valid.
 
         Assumes that the attribute types are already correct.
 
         :raises ValueError: If and only if one or more attributes are invalid
         """
```

### Comparing `python-can-4.1.0a2/can/notifier.py` & `python-can-4.2.0rc0/can/notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains the implementation of :class:`~can.Notifier`.
 """
 
 import asyncio
 import logging
 import threading
 import time
-from typing import Callable, Iterable, List, Optional, Union, Awaitable
+from typing import Awaitable, Callable, Iterable, List, Optional, Union
 
 from can.bus import BusABC
 from can.listener import Listener
 from can.message import Message
 
 logger = logging.getLogger("can.Notifier")
```

### Comparing `python-can-4.1.0a2/can/player.py` & `python-can-4.2.0rc0/can/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Replays CAN traffic saved with can.logger back
 to a CAN bus.
 
 Similar to canplayer in the can-utils package.
 """
 
-import sys
 import argparse
-from datetime import datetime
 import errno
-from typing import cast, Iterable
+import sys
+from datetime import datetime
+from typing import Iterable, cast
 
 from can import LogReader, Message, MessageSync
 
 from .logger import _create_base_argument_parser, _create_bus, _parse_additional_config
 
 
 def main() -> None:
@@ -83,15 +83,14 @@
 
     verbosity = results.verbosity
 
     error_frames = results.error_frames
 
     with _create_bus(results, **additional_config) as bus:
         with LogReader(results.infile, **additional_config) as reader:
-
             in_sync = MessageSync(
                 cast(Iterable[Message], reader),
                 timestamps=results.timestamps,
                 gap=results.gap,
                 skip=results.skip,
             )
```

### Comparing `python-can-4.1.0a2/can/thread_safe_bus.py` & `python-can-4.2.0rc0/can/thread_safe_bus.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     import_exc = None
 except ImportError as exc:
     ObjectProxy = object
     import_exc = exc
 
 from .interface import Bus
 
-
 try:
     from contextlib import nullcontext
 
 except ImportError:
 
     class nullcontext:  # type: ignore
         """A context manager that does nothing at all.
@@ -54,17 +53,15 @@
         if import_exc is not None:
             raise import_exc
 
         super().__init__(Bus(*args, **kwargs))
 
         # now, BusABC.send_periodic() does not need a lock anymore, but the
         # implementation still requires a context manager
-        # pylint: disable=protected-access
         self.__wrapped__._lock_send_periodic = nullcontext()
-        # pylint: enable=protected-access
 
         # init locks for sending and receiving separately
         self._lock_send = RLock()
         self._lock_recv = RLock()
 
     def recv(
         self, timeout=None, *args, **kwargs
```

### Comparing `python-can-4.1.0a2/can/typechecking.py` & `python-can-4.2.0rc0/can/typechecking.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 import typing
 
 if typing.TYPE_CHECKING:
     import os
 
 import typing_extensions
 
-CanFilter: typing_extensions = typing_extensions.TypedDict(
-    "CanFilter", {"can_id": int, "can_mask": int}
-)
-CanFilterExtended = typing_extensions.TypedDict(
-    "CanFilterExtended", {"can_id": int, "can_mask": int, "extended": bool}
-)
+
+class CanFilter(typing_extensions.TypedDict):
+    can_id: int
+    can_mask: int
+
+
+class CanFilterExtended(typing_extensions.TypedDict):
+    can_id: int
+    can_mask: int
+    extended: bool
+
+
 CanFilters = typing.Sequence[typing.Union[CanFilter, CanFilterExtended]]
 
 # TODO: Once buffer protocol support lands in typing, we should switch to that,
 # since can.message.Message attempts to call bytearray() on the given data, so
 # this should have the same typing info.
 #
 # See: https://github.com/python/typing/issues/593
@@ -31,12 +37,35 @@
 # Used by the IO module
 FileLike = typing.Union[typing.TextIO, typing.BinaryIO, gzip.GzipFile]
 StringPathLike = typing.Union[str, "os.PathLike[str]"]
 AcceptedIOType = typing.Union[FileLike, StringPathLike]
 
 BusConfig = typing.NewType("BusConfig", typing.Dict[str, typing.Any])
 
-AutoDetectedConfig = typing_extensions.TypedDict(
-    "AutoDetectedConfig", {"interface": str, "channel": Channel}
-)
+
+class AutoDetectedConfig(typing_extensions.TypedDict):
+    interface: str
+    channel: Channel
+
 
 ReadableBytesLike = typing.Union[bytes, bytearray, memoryview]
+
+
+class BitTimingDict(typing_extensions.TypedDict):
+    f_clock: int
+    brp: int
+    tseg1: int
+    tseg2: int
+    sjw: int
+    nof_samples: int
+
+
+class BitTimingFdDict(typing_extensions.TypedDict):
+    f_clock: int
+    nom_brp: int
+    nom_tseg1: int
+    nom_tseg2: int
+    nom_sjw: int
+    data_brp: int
+    data_tseg1: int
+    data_tseg2: int
+    data_sjw: int
```

### Comparing `python-can-4.1.0a2/can/util.py` & `python-can-4.2.0rc0/can/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 """
 Utilities and configuration file parsing.
 """
-
+import copy
 import functools
-import warnings
-from typing import Any, Callable, cast, Dict, Iterable, Tuple, Optional, Union
-from time import time, perf_counter, get_clock_info
 import json
+import logging
 import os
 import os.path
 import platform
 import re
-import logging
+import warnings
 from configparser import ConfigParser
+from time import get_clock_info, perf_counter, time
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import can
-from .interfaces import VALID_INTERFACES
+
 from . import typechecking
-from .exceptions import CanInterfaceNotImplementedError
+from .bit_timing import BitTiming, BitTimingFd
+from .exceptions import CanInitializationError, CanInterfaceNotImplementedError
+from .interfaces import VALID_INTERFACES
 
 log = logging.getLogger("can.util")
 
 # List of valid data lengths for a CAN FD message
 CAN_FD_DLC = [0, 1, 2, 3, 4, 5, 6, 7, 8, 12, 16, 20, 24, 32, 48, 64]
 
 REQUIRED_KEYS = ["interface", "channel"]
@@ -57,18 +69,18 @@
     config.optionxform = lambda entry: entry  # type: ignore
 
     if path is None:
         config.read([os.path.expanduser(path) for path in CONFIG_FILES])
     else:
         config.read(path)
 
-    _config = {}
+    _config: Dict[str, str] = {}
 
     if config.has_section(section):
-        _config.update(dict((key, val) for key, val in config.items(section)))
+        _config.update(config.items(section))
 
     return _config
 
 
 def load_environment_config(context: Optional[str] = None) -> Dict[str, str]:
     """
     Loads config dict from environmental variables (if set):
@@ -131,15 +143,15 @@
         Optional path to config file.
 
     :param config:
         A dict which may set the 'interface', and/or the 'channel', or neither.
         It may set other values that are passed through.
 
     :param context:
-        Extra 'context' pass to config sources. This can be use to section
+        Extra 'context' pass to config sources. This can be used to section
         other than 'default' in the configuration file.
 
     :return:
         A config dictionary that should contain 'interface' & 'channel'::
 
             {
                 'interface': 'python-can backend interface to use',
@@ -181,17 +193,20 @@
             cfg = cfg(context)
         # remove legacy operator (and copy to interface if not already present)
         if "bustype" in cfg:
             if "interface" not in cfg or not cfg["interface"]:
                 cfg["interface"] = cfg["bustype"]
             del cfg["bustype"]
         # copy all new parameters
-        for key in cfg:
+        for key, val in cfg.items():
             if key not in config:
-                config[key] = cfg[key]
+                if isinstance(val, str):
+                    config[key] = cast_from_string(val)
+                else:
+                    config[key] = cfg[key]
 
     bus_config = _create_bus_config(config)
     can.log.debug("can config: %s", bus_config)
     return bus_config
 
 
 def _create_bus_config(config: Dict[str, Any]) -> typechecking.BusConfig:
@@ -222,39 +237,35 @@
                 raise ValueError("Port config must be a number!")
         else:
             raise TypeError("Port config must be string or integer!")
 
         if not 0 < port < 65535:
             raise ValueError("Port config must be inside 0-65535 range!")
 
-    if "bitrate" in config:
-        config["bitrate"] = int(config["bitrate"])
+    if config.get("timing", None) is None:
+        try:
+            if set(typechecking.BitTimingFdDict.__annotations__).issubset(config):
+                config["timing"] = can.BitTimingFd(
+                    **{
+                        key: int(config[key])
+                        for key in typechecking.BitTimingFdDict.__annotations__
+                    }
+                )
+            elif set(typechecking.BitTimingDict.__annotations__).issubset(config):
+                config["timing"] = can.BitTiming(
+                    **{
+                        key: int(config[key])
+                        for key in typechecking.BitTimingDict.__annotations__
+                    }
+                )
+        except (ValueError, TypeError):
+            pass
+
     if "fd" in config:
-        config["fd"] = config["fd"] not in ("0", "False", "false", False)
-    if "data_bitrate" in config:
-        config["data_bitrate"] = int(config["data_bitrate"])
-
-    # Create bit timing configuration if given
-    timing_conf = {}
-    for key in (
-        "f_clock",
-        "brp",
-        "tseg1",
-        "tseg2",
-        "sjw",
-        "nof_samples",
-        "btr0",
-        "btr1",
-    ):
-        if key in config:
-            timing_conf[key] = int(str(config[key]), base=0)
-            del config[key]
-    if timing_conf:
-        timing_conf["bitrate"] = config["bitrate"]
-        config["timing"] = can.BitTiming(**timing_conf)
+        config["fd"] = config["fd"] not in (0, False)
 
     return cast(typechecking.BusConfig, config)
 
 
 def set_logging_level(level_name: str) -> None:
     """Set the logging level for the `"can"` logger.
 
@@ -310,57 +321,135 @@
     if isinstance(channel, str):
         match = re.match(r".*?(\d+)$", channel)
         if match:
             return int(match.group(1))
     return None
 
 
-def deprecated_args_alias(**aliases):
+def deprecated_args_alias(  # type: ignore
+    deprecation_start: str, deprecation_end: Optional[str] = None, **aliases
+):
     """Allows to rename/deprecate a function kwarg(s) and optionally
     have the deprecated kwarg(s) set as alias(es)
 
     Example::
 
-        @deprecated_args_alias(oldArg="new_arg", anotherOldArg="another_new_arg")
+        @deprecated_args_alias("1.2.0", oldArg="new_arg", anotherOldArg="another_new_arg")
         def library_function(new_arg, another_new_arg):
             pass
 
-        @deprecated_args_alias(oldArg="new_arg", obsoleteOldArg=None)
+        @deprecated_args_alias(
+            deprecation_start="1.2.0",
+            deprecation_end="3.0.0",
+            oldArg="new_arg",
+            obsoleteOldArg=None,
+        )
         def library_function(new_arg):
             pass
 
+    :param deprecation_start:
+        The *python-can* version, that introduced the :class:`DeprecationWarning`.
+    :param deprecation_end:
+        The *python-can* version, that marks the end of the deprecation period.
+    :param aliases:
+        keyword arguments, that map the deprecated argument names
+        to the new argument names or ``None``.
+
     """
 
     def deco(f):
         @functools.wraps(f)
         def wrapper(*args, **kwargs):
-            _rename_kwargs(f.__name__, kwargs, aliases)
+            _rename_kwargs(
+                func_name=f.__name__,
+                start=deprecation_start,
+                end=deprecation_end,
+                kwargs=kwargs,
+                aliases=aliases,
+            )
             return f(*args, **kwargs)
 
         return wrapper
 
     return deco
 
 
+T = TypeVar("T", BitTiming, BitTimingFd)
+
+
+def check_or_adjust_timing_clock(timing: T, valid_clocks: Iterable[int]) -> T:
+    """Adjusts the given timing instance to have an *f_clock* value that is within the
+    allowed values specified by *valid_clocks*. If the *f_clock* value of timing is
+    already within *valid_clocks*, then *timing* is returned unchanged.
+
+    :param timing:
+        The :class:`~can.BitTiming` or :class:`~can.BitTimingFd` instance to adjust.
+    :param valid_clocks:
+        An iterable of integers representing the valid *f_clock* values that the timing instance
+        can be changed to. The order of the values in *valid_clocks* determines the priority in
+        which they are tried, with earlier values being tried before later ones.
+    :return:
+        A new :class:`~can.BitTiming` or :class:`~can.BitTimingFd` instance with an
+        *f_clock* value within *valid_clocks*.
+    :raises ~can.exceptions.CanInitializationError:
+        If no compatible *f_clock* value can be found within *valid_clocks*.
+    """
+    if timing.f_clock in valid_clocks:
+        # create a copy so this function always returns a new instance
+        return copy.deepcopy(timing)
+
+    for clock in valid_clocks:
+        try:
+            # Try to use a different f_clock
+            adjusted_timing = timing.recreate_with_f_clock(clock)
+            warnings.warn(
+                f"Adjusted f_clock in {timing.__class__.__name__} from "
+                f"{timing.f_clock} to {adjusted_timing.f_clock}"
+            )
+            return adjusted_timing
+        except ValueError:
+            pass
+
+    raise CanInitializationError(
+        f"The specified timing.f_clock value {timing.f_clock} "
+        f"doesn't match any of the allowed device f_clock values: "
+        f"{', '.join([str(f) for f in valid_clocks])}"
+    ) from None
+
+
 def _rename_kwargs(
-    func_name: str, kwargs: Dict[str, str], aliases: Dict[str, str]
+    func_name: str,
+    start: str,
+    end: Optional[str],
+    kwargs: Dict[str, str],
+    aliases: Dict[str, str],
 ) -> None:
     """Helper function for `deprecated_args_alias`"""
     for alias, new in aliases.items():
         if alias in kwargs:
+            deprecation_notice = (
+                f"The '{alias}' argument is deprecated since python-can v{start}"
+            )
+            if end:
+                deprecation_notice += (
+                    f", and scheduled for removal in python-can v{end}"
+                )
+            deprecation_notice += "."
+
             value = kwargs.pop(alias)
             if new is not None:
-                warnings.warn(f"{alias} is deprecated; use {new}", DeprecationWarning)
+                deprecation_notice += f" Use '{new}' instead."
+
                 if new in kwargs:
                     raise TypeError(
-                        f"{func_name} received both {alias} (deprecated) and {new}"
+                        f"{func_name} received both '{alias}' (deprecated) and '{new}'."
                     )
                 kwargs[new] = value
-            else:
-                warnings.warn(f"{alias} is deprecated", DeprecationWarning)
+
+            warnings.warn(deprecation_notice, DeprecationWarning)
 
 
 def time_perfcounter_correlation() -> Tuple[float, float]:
     """Get the `perf_counter` value nearest to when time.time() is updated
 
     Computed if the default timer used by `time.time` on this platform has a resolution
     higher than 10μs, otherwise the current time and perf_counter is directly returned.
@@ -384,13 +473,35 @@
             if t1 != t0:
                 break
     else:
         return time(), perf_counter()
     return t1, performance_counter
 
 
+def cast_from_string(string_val: str) -> Union[str, int, float, bool]:
+    """Perform trivial type conversion from :class:`str` values.
+
+    :param string_val:
+        the string, that shall be converted
+    """
+    if re.match(r"^[-+]?\d+$", string_val):
+        # value is integer
+        return int(string_val)
+
+    if re.match(r"^[-+]?\d*\.\d+(?:e[-+]?\d+)?$", string_val):
+        # value is float
+        return float(string_val)
+
+    if re.match(r"^(?:True|False)$", string_val, re.IGNORECASE):
+        # value is bool
+        return string_val.lower() == "true"
+
+    # value is string
+    return string_val
+
+
 if __name__ == "__main__":
     print("Searching for configuration named:")
     print("\n".join(CONFIG_FILES))
     print()
     print("Settings:")
     print(load_config())
```

### Comparing `python-can-4.1.0a2/can/viewer.py` & `python-can-4.2.0rc0/can/viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,28 +26,29 @@
 import os
 import struct
 import sys
 import time
 from typing import Dict, List, Tuple, Union
 
 from can import __version__
+
 from .logger import (
-    _create_bus,
-    _parse_filters,
     _append_filter_argument,
     _create_base_argument_parser,
+    _create_bus,
     _parse_additional_config,
+    _parse_filters,
 )
 
-
-logger = logging.getLogger("can.serial")
+logger = logging.getLogger("can.viewer")
 
 try:
     import curses
-    from curses.ascii import ESC as KEY_ESC, SP as KEY_SPACE
+    from curses.ascii import ESC as KEY_ESC
+    from curses.ascii import SP as KEY_SPACE
 except ImportError:
     # Probably on Windows while windows-curses is not installed (e.g. in PyPy)
     logger.warning(
         "You won't be able to use the viewer program without curses installed!"
     )
     curses = None  # type: ignore
 
@@ -511,15 +512,15 @@
     # are divided by the value in order to convert from real units to raw integer values.
 
     data_structs: Dict[
         Union[int, Tuple[int, ...]], Union[struct.Struct, Tuple, None]
     ] = {}
     if parsed_args.decode:
         if os.path.isfile(parsed_args.decode[0]):
-            with open(parsed_args.decode[0], "r", encoding="utf-8") as f:
+            with open(parsed_args.decode[0], encoding="utf-8") as f:
                 structs = f.readlines()
         else:
             structs = parsed_args.decode
 
         for s in structs:
             tmp = s.rstrip("\n").split(":")
```

### Comparing `python-can-4.1.0a2/doc/asyncio.rst` & `python-can-4.2.0rc0/doc/asyncio.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/bcm.rst` & `python-can-4.2.0rc0/doc/bcm.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/bus.rst` & `python-can-4.2.0rc0/doc/bus.rst`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 .. code-block:: python
 
     filters = [
         {"can_id": 0x451, "can_mask": 0x7FF, "extended": False},
         {"can_id": 0xA0000, "can_mask": 0x1FFFFFFF, "extended": True},
     ]
-    bus = can.interface.Bus(channel="can0", bustype="socketcan", can_filters=filters)
+    bus = can.interface.Bus(channel="can0", interface="socketcan", can_filters=filters)
 
 
 See :meth:`~can.BusABC.set_filters` for the implementation.
 
 Bus API
 '''''''
```

### Comparing `python-can-4.1.0a2/doc/configuration.rst` & `python-can-4.2.0rc0/doc/configuration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     bus = Bus()
 
 
 You can also specify the interface and channel for each Bus instance::
 
     import can
 
-    bus = can.interface.Bus(bustype='socketcan', channel='vcan0', bitrate=500000)
+    bus = can.interface.Bus(interface='socketcan', channel='vcan0', bitrate=500000)
 
 
 Configuration File
 ------------------
 
 On Linux systems the config file is searched in the following paths:
```

### Comparing `python-can-4.1.0a2/doc/development.rst` & `python-can-4.2.0rc0/doc/development.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/history.rst` & `python-can-4.2.0rc0/doc/history.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/index.rst` & `python-can-4.2.0rc0/doc/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 **python-can** runs any where Python runs; from high powered computers
 with commercial `CAN to USB` devices right down to low powered devices running
 linux such as a BeagleBone or RaspberryPi.
 
 More concretely, some example uses of the library:
 
 * Passively logging what occurs on a CAN bus. For example monitoring a
-  commercial vehicle using its **OBD-II** port.
+  commercial vehicle using its `OBD-II port <https://en.wikipedia.org/wiki/On-board_diagnostics#OBD-II>`__.
 
 * Testing of hardware that interacts via CAN. Modules found in
   modern cars, motorcycles, boats, and even wheelchairs have had components tested
   from Python using this library.
 
 * Prototyping new hardware modules or software algorithms in-the-loop. Easily
   interact with an existing bus.
@@ -41,14 +41,15 @@
 
    installation
    configuration
    api
    interfaces
    virtual-interfaces
    plugin-interface
+   other-tools
    scripts
    development
    history
 
 
 Known Bugs
 ~~~~~~~~~~
```

### Comparing `python-can-4.1.0a2/doc/installation.rst` & `python-can-4.2.0rc0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/canalystii.rst` & `python-can-4.2.0rc0/doc/interfaces/canalystii.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/etas.rst` & `python-can-4.2.0rc0/doc/interfaces/etas.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/gs_usb.rst` & `python-can-4.2.0rc0/doc/interfaces/gs_usb.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 Usage: pass device ``index`` (starting from 0) if using automatic device detection:
 
 ::
 
     import can
 
-    bus = can.Bus(bustype="gs_usb", channel=dev.product, index=0, bitrate=250000)
+    bus = can.Bus(interface="gs_usb", channel=dev.product, index=0, bitrate=250000)
 
 Alternatively, pass ``bus`` and ``address`` to open a specific device. The parameters can be got by ``pyusb`` as shown below:
 
 .. code-block:: python
 
     import usb
     import can
 
     dev = usb.core.find(idVendor=0x1D50, idProduct=0x606F)
     bus = can.Bus(
-        bustype="gs_usb",
+        interface="gs_usb",
         channel=dev.product,
         bus=dev.bus,
         address=dev.address,
         bitrate=250000
     )
```

### Comparing `python-can-4.1.0a2/doc/interfaces/ixxat.rst` & `python-can-4.2.0rc0/doc/interfaces/ixxat.rst`

 * *Files 5% similar despite different names*

```diff
@@ -55,19 +55,28 @@
 VCI documentation, section "Message filters" for more info.
 
 List available devices
 ----------------------
 In case you have connected multiple IXXAT devices, you have to select them by using their unique hardware id.
 To get a list of all connected IXXAT you can use the function ``get_ixxat_hwids()`` as demonstrated below:
 
-    >>> from can.interfaces.ixxat import get_ixxat_hwids
-    >>> for hwid in get_ixxat_hwids():
-    ...     print("Found IXXAT with hardware id '%s'." % hwid)
-    Found IXXAT with hardware id 'HW441489'.
-    Found IXXAT with hardware id 'HW107422'.
+    .. testsetup:: ixxat
+
+        from unittest.mock import Mock
+        import can.interfaces.ixxat
+        assert hasattr(can.interfaces.ixxat, "get_ixxat_hwids")
+        can.interfaces.ixxat.get_ixxat_hwids = Mock(side_effect=lambda: ['HW441489', 'HW107422'])
+
+    .. doctest:: ixxat
+
+        >>> from can.interfaces.ixxat import get_ixxat_hwids
+        >>> for hwid in get_ixxat_hwids():
+        ...     print("Found IXXAT with hardware id '%s'." % hwid)
+        Found IXXAT with hardware id 'HW441489'.
+        Found IXXAT with hardware id 'HW107422'.
 
 
 Bus
 ---
 
 .. autoclass:: can.interfaces.ixxat.IXXATBus
     :members:
```

### Comparing `python-can-4.1.0a2/doc/interfaces/kvaser.rst` & `python-can-4.2.0rc0/doc/interfaces/kvaser.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/neousys.rst` & `python-can-4.2.0rc0/doc/interfaces/neousys.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/neovi.rst` & `python-can-4.2.0rc0/doc/interfaces/neovi.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/nican.rst` & `python-can-4.2.0rc0/doc/interfaces/nican.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/pcan.rst` & `python-can-4.2.0rc0/doc/interfaces/pcan.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/robotell.rst` & `python-can-4.2.0rc0/doc/interfaces/robotell.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/seeedstudio.rst` & `python-can-4.2.0rc0/doc/interfaces/seeedstudio.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ::
 
     can.interfaces.seeedstudio.SeeedBus
 
 A bus example::
 
-    bus = can.interface.Bus(bustype='seeedstudio', channel='/dev/ttyUSB0', bitrate=500000)
+    bus = can.interface.Bus(interface='seeedstudio', channel='/dev/ttyUSB0', bitrate=500000)
 
 
 
 Configuration
 -------------
 ::
```

### Comparing `python-can-4.1.0a2/doc/interfaces/serial.rst` & `python-can-4.2.0rc0/doc/interfaces/serial.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/slcan.rst` & `python-can-4.2.0rc0/doc/interfaces/slcan.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/socketcan.rst` & `python-can-4.2.0rc0/doc/interfaces/socketcan.rst`

 * *Files 4% similar despite different names*

```diff
@@ -173,20 +173,20 @@
 To spam a bus:
 
 .. code-block:: python
 
     import time
     import can
 
-    bustype = 'socketcan'
+    interface = 'socketcan'
     channel = 'vcan0'
 
     def producer(id):
         """:param id: Spam the bus with messages including the data id."""
-        bus = can.Bus(channel=channel, interface=bustype)
+        bus = can.Bus(channel=channel, interface=interface)
         for i in range(10):
             msg = can.Message(arbitration_id=0xc0ffee, data=[id, i, 0, 1, 3, 1, 4, 1], is_extended_id=False)
             bus.send(msg)
         
         time.sleep(1)
 
     producer(10)
```

### Comparing `python-can-4.1.0a2/doc/interfaces/socketcand.rst` & `python-can-4.2.0rc0/doc/interfaces/socketcand.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Here is a small example dumping all can messages received by a socketcand 
 daemon running on a remote Raspberry Pi:
 
 .. code-block:: python
 
     import can
 
-    bus = can.interface.Bus(bustype='socketcand', host="10.0.16.15", port=29536, channel="can0")
+    bus = can.interface.Bus(interface='socketcand', host="10.0.16.15", port=29536, channel="can0")
 
     # loop until Ctrl-C
     try:
       while True:
         msg = bus.recv()
         print(msg)
     except KeyboardInterrupt:
```

### Comparing `python-can-4.1.0a2/doc/interfaces/systec.rst` & `python-can-4.2.0rc0/doc/interfaces/systec.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/udp_multicast.rst` & `python-can-4.2.0rc0/doc/interfaces/udp_multicast.rst`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 .. code-block:: python
 
         import time
         import can
         from can.interfaces.udp_multicast import UdpMulticastBus
 
         # The bus can be created using the can.Bus wrapper class or using UdpMulticastBus directly
-        with can.Bus(channel=UdpMulticastBus.DEFAULT_GROUP_IPv6, bustype='udp_multicast') as bus_1, \
+        with can.Bus(channel=UdpMulticastBus.DEFAULT_GROUP_IPv6, interface='udp_multicast') as bus_1, \
                 UdpMulticastBus(channel=UdpMulticastBus.DEFAULT_GROUP_IPv6) as bus_2:
 
             # register a callback on the second bus that prints messages to the standard out
             notifier = can.Notifier(bus_2, [can.Printer()])
 
             # create and send a message with the first bus, which should arrive at the second one
             message = can.Message(arbitration_id=0x123, data=[1, 2, 3])
```

### Comparing `python-can-4.1.0a2/doc/interfaces/usb2can.rst` & `python-can-4.2.0rc0/doc/interfaces/usb2can.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/interfaces/vector.rst` & `python-can-4.2.0rc0/doc/interfaces/vector.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 a new application and assign the channels you may want to use.
 Specify the application name as ``app_name='Your app name'`` when constructing
 the bus or in a config file.
 
 Channel should be given as a list of channels starting at 0.
 
 Here is an example configuration file connecting to CAN 1 and CAN 2 for an
-application named "python-can"::
+application named "python-can":
+
+::
 
     [default]
     interface = vector
     channel = 0, 1
     app_name = python-can
```

### Comparing `python-can-4.1.0a2/doc/interfaces/virtual.rst` & `python-can-4.2.0rc0/doc/interfaces/virtual.rst`

 * *Files 13% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 Example
 -------
 
 .. code-block:: python
 
     import can
 
-    bus1 = can.interface.Bus('test', bustype='virtual')
-    bus2 = can.interface.Bus('test', bustype='virtual')
+    bus1 = can.interface.Bus('test', interface='virtual')
+    bus2 = can.interface.Bus('test', interface='virtual')
 
     msg1 = can.Message(arbitration_id=0xabcde, data=[1,2,3])
     bus1.send(msg1)
     msg2 = bus2.recv()
 
     #assert msg1 == msg2
     assert msg1.arbitration_id == msg2.arbitration_id
     assert msg1.data == msg2.data
     assert msg1.timestamp != msg2.timestamp
 
 .. code-block:: python
 
     import can
 
-    bus1 = can.interface.Bus('test', bustype='virtual', preserve_timestamps=True)
-    bus2 = can.interface.Bus('test', bustype='virtual')
+    bus1 = can.interface.Bus('test', interface='virtual', preserve_timestamps=True)
+    bus2 = can.interface.Bus('test', interface='virtual')
 
     msg1 = can.Message(timestamp=1639740470.051948, arbitration_id=0xabcde, data=[1,2,3])
 
     # Messages sent on bus1 will have their timestamps preserved when received
     # on bus2
     bus1.send(msg1)
     msg2 = bus2.recv()
```

### Comparing `python-can-4.1.0a2/doc/interfaces.rst` & `python-can-4.2.0rc0/doc/interfaces.rst`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 device is different, you should carefully go through your interface's
 documentation.
 
 .. note::
    The *Interface Names* are listed in :doc:`configuration`.
 
 
-The available hardware interfaces are:
+The following hardware interfaces are included in python-can:
 
 .. toctree::
    :maxdepth: 1
 
    interfaces/canalystii
    interfaces/cantact
    interfaces/etas
@@ -35,7 +35,9 @@
    interfaces/slcan
    interfaces/socketcan
    interfaces/socketcand
    interfaces/systec
    interfaces/usb2can
    interfaces/vector
 
+
+Additional interface types can be added via the :ref:`plugin interface`, or by installing a third party package that utilises the :ref:`plugin interface`.
```

### Comparing `python-can-4.1.0a2/doc/internal-api.rst` & `python-can-4.2.0rc0/doc/internal-api.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/listeners.rst` & `python-can-4.2.0rc0/doc/listeners.rst`

 * *Files 20% similar despite different names*

```diff
@@ -207,14 +207,45 @@
     :members:
 
 The following class can be used to read messages from BLF file:
 
 .. autoclass:: can.BLFReader
     :members:
 
+
+MF4 (Measurement Data Format v4)
+--------------------------------
+
+Implements support for MF4 (Measurement Data Format v4) which is a proprietary
+format from ASAM (Association for Standardization of Automation and Measuring Systems), widely used in 
+many automotive software (Vector CANape, ETAS INCA, dSPACE ControlDesk, etc.).
+
+The data is stored in a compressed format which makes it compact.
+
+.. note:: MF4 support has to be installed as an extra with for example ``pip install python-can[mf4]``.
+
+.. note:: Channels will be converted to integers.
+
+.. note:: MF4Writer does not suppport the append mode.
+
+
+.. autoclass:: can.MF4Writer
+    :members:
+
+The MDF format is very flexible regarding the internal structure and it is used to handle data from multiple sources, not just CAN bus logging.
+MDF4Writer will always create a fixed internal file structure where there will be three channel groups (for standard, error and remote frames). 
+Using this fixed file structure allows for a simple implementation of MDF4Writer and MF4Reader classes.
+Therefor MF4Reader can only replay files created with MF4Writer. 
+
+The following class can be used to read messages from MF4 file:
+
+.. autoclass:: can.MF4Reader
+    :members:
+
+
 TRC
 ----
 
 Implements basic support for the TRC file format.
 
 
 .. note::
```

### Comparing `python-can-4.1.0a2/doc/message.rst` & `python-can-4.2.0rc0/doc/message.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         >>> from can import Message
         >>> test = Message(data=[1, 2, 3, 4, 5])
         >>> test.data
         bytearray(b'\x01\x02\x03\x04\x05')
         >>> test.dlc
         5
         >>> print(test)
-        Timestamp:        0.000000    ID: 00000000    010    DLC: 5    01 02 03 04 05
+        Timestamp:        0.000000    ID: 00000000    X Rx                DL:  5    01 02 03 04 05
 
 
     The :attr:`~can.Message.arbitration_id` field in a CAN message may be either
     11 bits (standard addressing, CAN 2.0A) or 29 bits (extended addressing, CAN
     2.0B) in length, and ``python-can`` exposes this difference with the
     :attr:`~can.Message.is_extended_id` attribute.
 
@@ -40,27 +40,27 @@
 
         The arbitration ID can take an int between 0 and the
         maximum value allowed depending on the ``is_extended_id`` flag
         (either 2\ :sup:`11` - 1 for 11-bit IDs, or
         2\ :sup:`29` - 1 for 29-bit identifiers).
 
             >>> print(Message(is_extended_id=False, arbitration_id=100))
-            Timestamp:        0.000000        ID: 0064    S        DLC: 0
+            Timestamp:        0.000000        ID: 0064    S Rx                DL:  0
 
 
     .. attribute:: data
 
         :type: bytearray
 
         The data parameter of a CAN message is exposed as a **bytearray**
         with length between 0 and 8.
 
             >>> example_data = bytearray([1, 2, 3])
             >>> print(Message(data=example_data))
-            Timestamp:        0.000000    ID: 00000000    X        DLC: 3    01 02 03
+            Timestamp:        0.000000    ID: 00000000    X Rx                DL:  3    01 02 03
 
         A :class:`~can.Message` can also be created with bytes, or lists of ints:
 
             >>> m1 = Message(data=[0x64, 0x65, 0x61, 0x64, 0x62, 0x65, 0x65, 0x66])
             >>> print(m1.data)
             bytearray(b'deadbeef')
             >>> m2 = Message(data=b'deadbeef')
@@ -102,17 +102,17 @@
 
         :type: bool
 
         This flag controls the size of the :attr:`~can.Message.arbitration_id` field.
         Previously this was exposed as `id_type`.
 
         >>> print(Message(is_extended_id=False))
-        Timestamp:        0.000000        ID: 0000    S        DLC: 0
+        Timestamp:        0.000000        ID: 0000    S Rx                DL:  0
         >>> print(Message(is_extended_id=True))
-        Timestamp:        0.000000    ID: 00000000    X        DLC: 0
+        Timestamp:        0.000000    ID: 00000000    X Rx                DL:  0
 
 
         .. note::
 
             The initializer argument and attribute ``extended_id`` has been deprecated in favor of
             ``is_extended_id``, but will continue to work for the ``3.x`` release series.
 
@@ -120,26 +120,26 @@
     .. attribute:: is_error_frame
 
         :type: bool
 
         This boolean parameter indicates if the message is an error frame or not.
 
         >>> print(Message(is_error_frame=True))
-        Timestamp:        0.000000    ID: 00000000    X E      DLC: 0
+        Timestamp:        0.000000    ID: 00000000    X Rx E              DL:  0
 
 
     .. attribute:: is_remote_frame
 
         :type: bool
 
         This boolean attribute indicates if the message is a remote frame or a data frame, and
         modifies the bit in the CAN message's flags field indicating this.
 
         >>> print(Message(is_remote_frame=True))
-        Timestamp:        0.000000    ID: 00000000    X   R    DLC: 0
+        Timestamp:        0.000000    ID: 00000000    X Rx   R            DL:  0
 
 
     .. attribute:: is_fd
 
         :type: bool
 
         Indicates that this message is a CAN FD message.
@@ -170,25 +170,25 @@
     .. method:: __str__
 
         A string representation of a CAN message:
 
             >>> from can import Message
             >>> test = Message()
             >>> print(test)
-            Timestamp:        0.000000    ID: 00000000    X        DLC: 0
+            Timestamp:        0.000000    ID: 00000000    X Rx                DL:  0
             >>> test2 = Message(data=[1, 2, 3, 4, 5])
             >>> print(test2)
-            Timestamp:        0.000000    ID: 00000000    X        DLC: 5    01 02 03 04 05
+            Timestamp:        0.000000    ID: 00000000    X Rx                DL:  5    01 02 03 04 05
 
         The fields in the printed message are (in order):
 
         - timestamp,
         - arbitration ID,
         - flags,
-        - dlc,
+        - data length (DL),
         - and data.
 
 
         The flags field is represented as one, two or three letters:
 
         - X if the :attr:`~can.Message.is_extended_id` attribute is set, otherwise S,
         - E if the :attr:`~can.Message.is_error_frame` attribute is set,
```

### Comparing `python-can-4.1.0a2/doc/scripts.rst` & `python-can-4.2.0rc0/doc/scripts.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/doc/virtual-interfaces.rst` & `python-can-4.2.0rc0/doc/virtual-interfaces.rst`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/python_can.egg-info/PKG-INFO` & `python-can-4.2.0rc0/python_can.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can
-Version: 4.1.0a2
+Version: 4.2.0rc0
 Summary: Controller Area Network interface module for Python
 Home-page: https://github.com/hardbyte/python-can
 Author: python-can contributors
 License: LGPL v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,31 +34,40 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: seeedstudio
 Provides-Extra: serial
 Provides-Extra: neovi
 Provides-Extra: canalystii
 Provides-Extra: cantact
+Provides-Extra: cvector
 Provides-Extra: gs_usb
 Provides-Extra: nixnet
 Provides-Extra: pcan
+Provides-Extra: remote
+Provides-Extra: sontheim
+Provides-Extra: canine
 Provides-Extra: viewer
+Provides-Extra: mf4
 License-File: LICENSE.txt
 
 python-can
 ==========
 
-|release| |python_implementation| |downloads| |downloads_monthly| |formatter|
+|pypi| |conda| |python_implementation| |downloads| |downloads_monthly|
 
-|docs| |github-actions| |build_travis| |coverage| |mergify|
+|docs| |github-actions| |build_travis| |coverage| |mergify| |formatter|
 
-.. |release| image:: https://img.shields.io/pypi/v/python-can.svg
+.. |pypi| image:: https://img.shields.io/pypi/v/python-can.svg
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Latest Version on PyPi
 
+.. |conda| image:: https://img.shields.io/conda/v/conda-forge/python-can
+   :target: https://github.com/conda-forge/python-can-feedstock
+   :alt: Latest Version on conda-forge
+
 .. |python_implementation| image:: https://img.shields.io/pypi/implementation/python-can
    :target: https://pypi.python.org/pypi/python-can/
    :alt: Supported Python implementations
 
 .. |downloads| image:: https://pepy.tech/badge/python-can
    :target: https://pepy.tech/project/python-can
    :alt: Downloads on PePy
@@ -71,16 +80,16 @@
    :target: https://github.com/python/black
    :alt: This project uses the black formatter.
 
 .. |docs| image:: https://readthedocs.org/projects/python-can/badge/?version=stable
    :target: https://python-can.readthedocs.io/en/stable/
    :alt: Documentation
 
-.. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/build.yml/badge.svg?branch=develop
-   :target: https://github.com/hardbyte/python-can/actions/workflows/build.yml
+.. |github-actions| image:: https://github.com/hardbyte/python-can/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/hardbyte/python-can/actions/workflows/ci.yml
    :alt: Github Actions workflow status
 
 .. |build_travis| image:: https://img.shields.io/travis/hardbyte/python-can/develop.svg?label=Travis%20CI
    :target: https://app.travis-ci.com/github/hardbyte/python-can
    :alt: Travis CI Server for develop branch
 
 .. |coverage| image:: https://coveralls.io/repos/github/hardbyte/python-can/badge.svg?branch=develop
@@ -116,15 +125,15 @@
 --------
 
 - common abstractions for CAN communication
 - support for many different backends (see the `docs <https://python-can.readthedocs.io/en/stable/interfaces.html>`__)
 - receiving, sending, and periodically sending messages
 - normal and extended arbitration IDs
 - `CAN FD <https://en.wikipedia.org/wiki/CAN_FD>`__ support
-- many different loggers and readers supporting playback: ASC (CANalyzer format), BLF (Binary Logging Format by Vector), TRC, CSV, SQLite, and Canutils log
+- many different loggers and readers supporting playback: ASC (CANalyzer format), BLF (Binary Logging Format by Vector), MF4 (Measurement Data Format v4 by ASAM), TRC, CSV, SQLite, and Canutils log
 - efficient in-kernel or in-hardware filtering of messages on supported interfaces
 - bus configuration reading from a file or from environment variables
 - command line tools for working with CAN buses (see the `docs <https://python-can.readthedocs.io/en/stable/scripts.html>`__)
 - more
 
 
 Example usage
@@ -133,31 +142,32 @@
 ``pip install python-can``
 
 .. code:: python
 
     # import the library
     import can
 
-    # create a bus instance
+    # create a bus instance using 'with' statement,
+    # this will cause bus.shutdown() to be called on the block exit;
     # many other interfaces are supported as well (see documentation)
-    bus = can.Bus(interface='socketcan',
+    with can.Bus(interface='socketcan',
                   channel='vcan0',
-                  receive_own_messages=True)
+                  receive_own_messages=True) as bus:
 
-    # send a message
-    message = can.Message(arbitration_id=123, is_extended_id=True,
-                          data=[0x11, 0x22, 0x33])
-    bus.send(message, timeout=0.2)
-
-    # iterate over received messages
-    for msg in bus:
-        print(f"{msg.arbitration_id:X}: {msg.data}")
+       # send a message
+       message = can.Message(arbitration_id=123, is_extended_id=True,
+                             data=[0x11, 0x22, 0x33])
+       bus.send(message, timeout=0.2)
+
+       # iterate over received messages
+       for msg in bus:
+           print(f"{msg.arbitration_id:X}: {msg.data}")
 
-    # or use an asynchronous notifier
-    notifier = can.Notifier(bus, [can.Logger("recorded.log"), can.Printer()])
+       # or use an asynchronous notifier
+       notifier = can.Notifier(bus, [can.Logger("recorded.log"), can.Printer()])
 
 You can find more information in the documentation, online at
 `python-can.readthedocs.org <https://python-can.readthedocs.org/en/stable/>`__.
 
 
 Discussion
 ----------
```

### Comparing `python-can-4.1.0a2/python_can.egg-info/SOURCES.txt` & `python-can-4.2.0rc0/python_can.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 can/io/__init__.py
 can/io/asc.py
 can/io/blf.py
 can/io/canutils.py
 can/io/csv.py
 can/io/generic.py
 can/io/logger.py
+can/io/mf4.py
 can/io/player.py
 can/io/printer.py
 can/io/sqlite.py
 can/io/trc.py
 doc/api.rst
 doc/asyncio.rst
 doc/bcm.rst
@@ -105,14 +106,15 @@
 doc/history.rst
 doc/index.rst
 doc/installation.rst
 doc/interfaces.rst
 doc/internal-api.rst
 doc/listeners.rst
 doc/message.rst
+doc/other-tools.rst
 doc/plugin-interface.rst
 doc/scripts.rst
 doc/utils.rst
 doc/virtual-interfaces.rst
 doc/interfaces/canalystii.rst
 doc/interfaces/cantact.rst
 doc/interfaces/etas.rst
@@ -153,17 +155,19 @@
 test/logformats_test.py
 test/message_helper.py
 test/network_test.py
 test/notifier_test.py
 test/serial_test.py
 test/simplecyclic_test.py
 test/test_bit_timing.py
+test/test_bus.py
 test/test_cantact.py
 test/test_cyclic_socketcan.py
 test/test_detect_available_configs.py
+test/test_interface.py
 test/test_interface_canalystii.py
 test/test_interface_ixxat.py
 test/test_interface_ixxat_fd.py
 test/test_interface_virtual.py
 test/test_kvaser.py
 test/test_load_config.py
 test/test_load_file_config.py
```

### Comparing `python-can-4.1.0a2/setup.cfg` & `python-can-4.2.0rc0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [mypy]
 warn_return_any = True
 warn_unused_configs = True
 ignore_missing_imports = True
 no_implicit_optional = True
 disallow_incomplete_defs = True
 warn_redundant_casts = True
-warn_unused_ignores = True
+warn_unused_ignores = False
 exclude = 
 	(?x)(
 	venv
 	|^doc/conf.py$
 	|^test
 	|^setup.py$
 	|^can/interfaces/__init__.py
```

### Comparing `python-can-4.1.0a2/setup.py` & `python-can-4.2.0rc0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 #!/usr/bin/env python
 
 """
 Setup script for the `can` package.
 Learn more at https://github.com/hardbyte/python-can/
 """
 
-# pylint: disable=invalid-name
-
+import logging
+import re
 from os import listdir
 from os.path import isfile, join
-import re
-import logging
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 logging.basicConfig(level=logging.WARNING)
 
-with open("can/__init__.py", "r", encoding="utf-8") as fd:
+with open("can/__init__.py", encoding="utf-8") as fd:
     version = re.search(
         r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
     ).group(1)
 
-with open("README.rst", "r", encoding="utf-8") as f:
+with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 # Dependencies
 extras_require = {
     "seeedstudio": ["pyserial>=3.0"],
     "serial": ["pyserial~=3.0"],
     "neovi": ["filelock", "python-ics>=2.12"],
     "canalystii": ["canalystii>=0.1.0"],
     "cantact": ["cantact>=0.0.7"],
+    "cvector": ["python-can-cvector"],
     "gs_usb": ["gs_usb>=0.2.1"],
-    "nixnet": ["nixnet>=0.3.1"],
+    "nixnet": ["nixnet>=0.3.2"],
     "pcan": ["uptime~=3.0.1"],
+    "remote": ["python-can-remote"],
+    "sontheim": ["python-can-sontheim>=0.1.2"],
+    "canine": ["python-can-canine>=0.2.2"],
     "viewer": [
         'windows-curses;platform_system=="Windows" and platform_python_implementation=="CPython"'
     ],
+    "mf4": ["asammdf>=6.0.0"],
 }
 
 setup(
     # Description
     name="python-can",
     url="https://github.com/hardbyte/python-can",
     description="Controller Area Network interface module for Python",
@@ -88,13 +92,13 @@
     # Installation
     # see https://www.python.org/dev/peps/pep-0345/#version-specifiers
     python_requires=">=3.7",
     install_requires=[
         "setuptools",
         "wrapt~=1.10",
         "typing_extensions>=3.10.0.0",
-        'pywin32;platform_system=="Windows" and platform_python_implementation=="CPython"',
+        'pywin32>=305;platform_system=="Windows" and platform_python_implementation=="CPython"',
         'msgpack~=1.0.0;platform_system!="Windows"',
         "packaging",
     ],
     extras_require=extras_require,
 )
```

### Comparing `python-can-4.1.0a2/test/back2back_test.py` & `python-can-4.2.0rc0/test/back2back_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #!/usr/bin/env python
 
 """
 This module tests two buses attached to each other.
 """
 
+import random
 import unittest
-from time import sleep, time
 from multiprocessing.dummy import Pool as ThreadPool
-import random
+from time import sleep, time
 
 import pytest
 
 import can
+from can import CanInterfaceNotImplementedError
 from can.interfaces.udp_multicast import UdpMulticastBus
 
 from .config import (
     IS_CI,
-    IS_UNIX,
     IS_OSX,
+    IS_PYPY,
     IS_TRAVIS,
-    TEST_INTERFACE_SOCKETCAN,
+    IS_UNIX,
     TEST_CAN_FD,
-    IS_PYPY,
+    TEST_INTERFACE_SOCKETCAN,
 )
 
 
 class Back2BackTestCase(unittest.TestCase):
     """Use two interfaces connected to the same CAN bus and test them against each other.
 
     This very class declaration runs the test on the *virtual* interface but subclasses can be created for
@@ -39,22 +40,22 @@
     CHANNEL_1 = "virtual_channel_0"
     INTERFACE_2 = "virtual"
     CHANNEL_2 = "virtual_channel_0"
 
     def setUp(self):
         self.bus1 = can.Bus(
             channel=self.CHANNEL_1,
-            bustype=self.INTERFACE_1,
+            interface=self.INTERFACE_1,
             bitrate=self.BITRATE,
             fd=TEST_CAN_FD,
             single_handle=True,
         )
         self.bus2 = can.Bus(
             channel=self.CHANNEL_2,
-            bustype=self.INTERFACE_2,
+            interface=self.INTERFACE_2,
             bitrate=self.BITRATE,
             fd=TEST_CAN_FD,
             single_handle=True,
         )
 
     def tearDown(self):
         self.bus1.shutdown()
@@ -162,15 +163,15 @@
     @unittest.skip(
         "TODO: how shall this be treated if sending messages locally? should be done uniformly"
     )
     def test_message_is_rx_receive_own_messages(self):
         """The same as `test_message_direction` but testing with `receive_own_messages=True`."""
         bus3 = can.Bus(
             channel=self.CHANNEL_2,
-            bustype=self.INTERFACE_2,
+            interface=self.INTERFACE_2,
             bitrate=self.BITRATE,
             fd=TEST_CAN_FD,
             single_handle=True,
             receive_own_messages=True,
         )
         try:
             msg = can.Message(
@@ -184,15 +185,15 @@
 
     def test_unique_message_instances(self):
         """Verify that we have a different instances of message for each bus even with
         `receive_own_messages=True`.
         """
         bus3 = can.Bus(
             channel=self.CHANNEL_2,
-            bustype=self.INTERFACE_2,
+            interface=self.INTERFACE_2,
             bitrate=self.BITRATE,
             fd=TEST_CAN_FD,
             single_handle=True,
             receive_own_messages=True,
         )
         try:
             msg = can.Message(
@@ -271,36 +272,34 @@
         # Some buses may receive their own messages. Remove it from the queue
         self.bus2.recv(0)
         self.bus2.recv(0)
 
 
 @unittest.skipUnless(TEST_INTERFACE_SOCKETCAN, "skip testing of socketcan")
 class BasicTestSocketCan(Back2BackTestCase):
-
     INTERFACE_1 = "socketcan"
     CHANNEL_1 = "vcan0"
     INTERFACE_2 = "socketcan"
     CHANNEL_2 = "vcan0"
 
 
 # this doesn't even work on Travis CI for macOS; for example, see
 # https://travis-ci.org/github/hardbyte/python-can/jobs/745389871
 @unittest.skipUnless(
     IS_UNIX and not (IS_CI and IS_OSX),
     "only supported on Unix systems (but not on macOS at Travis CI and GitHub Actions)",
 )
 class BasicTestUdpMulticastBusIPv4(Back2BackTestCase):
-
     INTERFACE_1 = "udp_multicast"
     CHANNEL_1 = UdpMulticastBus.DEFAULT_GROUP_IPv4
     INTERFACE_2 = "udp_multicast"
     CHANNEL_2 = UdpMulticastBus.DEFAULT_GROUP_IPv4
 
     def test_unique_message_instances(self):
-        with self.assertRaises(NotImplementedError):
+        with self.assertRaises(CanInterfaceNotImplementedError):
             super().test_unique_message_instances()
 
 
 # this doesn't even work for loopback multicast addresses on Travis CI; for example, see
 # https://travis-ci.org/github/hardbyte/python-can/builds/745065503
 @unittest.skipUnless(
     IS_UNIX and not (IS_TRAVIS or (IS_CI and IS_OSX)),
@@ -311,29 +310,28 @@
 
     INTERFACE_1 = "udp_multicast"
     CHANNEL_1 = HOST_LOCAL_MCAST_GROUP_IPv6
     INTERFACE_2 = "udp_multicast"
     CHANNEL_2 = HOST_LOCAL_MCAST_GROUP_IPv6
 
     def test_unique_message_instances(self):
-        with self.assertRaises(NotImplementedError):
+        with self.assertRaises(CanInterfaceNotImplementedError):
             super().test_unique_message_instances()
 
 
 TEST_INTERFACE_ETAS = False
 try:
     bus_class = can.interface._get_class_for_interface("etas")
     TEST_INTERFACE_ETAS = True
-except can.exceptions.CanInterfaceNotImplementedError:
+except CanInterfaceNotImplementedError:
     pass
 
 
 @unittest.skipUnless(TEST_INTERFACE_ETAS, "skip testing of etas interface")
 class BasicTestEtas(Back2BackTestCase):
-
     if TEST_INTERFACE_ETAS:
         configs = can.interface.detect_available_configs(interfaces="etas")
 
         INTERFACE_1 = "etas"
         CHANNEL_1 = configs[0]["channel"]
         INTERFACE_2 = "etas"
         CHANNEL_2 = configs[2]["channel"]
@@ -343,16 +341,16 @@
             "creating a second instance of a channel with differing self-reception settings is not supported"
         )
 
 
 @unittest.skipUnless(TEST_INTERFACE_SOCKETCAN, "skip testing of socketcan")
 class SocketCanBroadcastChannel(unittest.TestCase):
     def setUp(self):
-        self.broadcast_bus = can.Bus(channel="", bustype="socketcan")
-        self.regular_bus = can.Bus(channel="vcan0", bustype="socketcan")
+        self.broadcast_bus = can.Bus(channel="", interface="socketcan")
+        self.regular_bus = can.Bus(channel="vcan0", interface="socketcan")
 
     def tearDown(self):
         self.broadcast_bus.shutdown()
         self.regular_bus.shutdown()
 
     def test_broadcast_channel(self):
         self.broadcast_bus.send(can.Message(channel="vcan0"))
@@ -366,22 +364,22 @@
         self.assertEqual(recv_msg.channel, "vcan0")
 
 
 class TestThreadSafeBus(Back2BackTestCase):
     def setUp(self):
         self.bus1 = can.ThreadSafeBus(
             channel=self.CHANNEL_1,
-            bustype=self.INTERFACE_1,
+            interface=self.INTERFACE_1,
             bitrate=self.BITRATE,
             fd=TEST_CAN_FD,
             single_handle=True,
         )
         self.bus2 = can.ThreadSafeBus(
             channel=self.CHANNEL_2,
-            bustype=self.INTERFACE_2,
+            interface=self.INTERFACE_2,
             bitrate=self.BITRATE,
             fd=TEST_CAN_FD,
             single_handle=True,
         )
 
     @pytest.mark.timeout(180.0 if IS_PYPY else 5.0)
     def test_concurrent_writes(self):
```

### Comparing `python-can-4.1.0a2/test/config.py` & `python-can-4.2.0rc0/test/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 IS_TRAVIS = env("TRAVIS")
 IS_GITHUB_ACTIONS = env("GITHUB_ACTIONS")
 
 IS_CI = IS_TRAVIS or IS_GITHUB_ACTIONS or env("CI") or env("CONTINUOUS_INTEGRATION")
 
 if IS_TRAVIS and IS_GITHUB_ACTIONS:
-    raise EnvironmentError(
+    raise OSError(
         f"only one of IS_TRAVIS ({IS_TRAVIS}) and IS_GITHUB_ACTIONS ({IS_GITHUB_ACTIONS}) may be True at the "
         "same time"
     )
 
 
 # ############################## Platforms
 
@@ -39,15 +39,15 @@
 IS_WINDOWS = "windows" in _sys or ("win" in _sys and "darwin" not in _sys)
 IS_LINUX = "linux" in _sys
 IS_OSX = "darwin" in _sys
 IS_UNIX = IS_LINUX or IS_OSX
 del _sys
 
 if (IS_WINDOWS and IS_LINUX) or (IS_LINUX and IS_OSX) or (IS_WINDOWS and IS_OSX):
-    raise EnvironmentError(
+    raise OSError(
         f"only one of IS_WINDOWS ({IS_WINDOWS}), IS_LINUX ({IS_LINUX}) and IS_OSX ({IS_OSX}) "
         f'can be True at the same time (platform.system() == "{platform.system()}")'
     )
 
 
 # ############################## Implementations
```

### Comparing `python-can-4.1.0a2/test/contextmanager_test.py` & `python-can-4.2.0rc0/test/contextmanager_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 
 """
 This module tests the context manager of Bus and Notifier classes
 """
 
 import unittest
+
 import can
 
 
 class ContextManagerTest(unittest.TestCase):
     def setUp(self):
         data = [0, 1, 2, 3, 4, 5, 6, 7]
         self.msg_send = can.Message(
```

### Comparing `python-can-4.1.0a2/test/data/example_data.py` & `python-can-4.2.0rc0/test/data/example_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,56 +29,67 @@
 
 
 # List of messages of different types that can be used in tests
 TEST_MESSAGES_BASE = sort_messages(
     [
         Message(
             # empty
+            timestamp=1e-4,
         ),
         Message(
             # only data
-            data=[0x00, 0x42]
+            timestamp=2e-4,
+            data=[0x00, 0x42],
         ),
         Message(
             # no data
+            timestamp=3e-4,
             arbitration_id=0xAB,
             is_extended_id=False,
         ),
         Message(
             # no data
+            timestamp=4e-4,
             arbitration_id=0x42,
             is_extended_id=True,
         ),
         Message(
             # no data
-            arbitration_id=0xABCDEF
+            timestamp=5e-4,
+            arbitration_id=0xABCDEF,
         ),
         Message(
             # empty data
-            data=[]
+            timestamp=6e-4,
+            data=[],
         ),
         Message(
             # empty data
-            data=[0xFF, 0xFE, 0xFD]
+            timestamp=7e-4,
+            data=[0xFF, 0xFE, 0xFD],
         ),
         Message(
             # with channel as integer
-            channel=0
+            timestamp=8e-4,
+            channel=0,
         ),
         Message(
             # with channel as integer
-            channel=42
+            timestamp=9e-4,
+            channel=42,
         ),
         Message(
             # with channel as string
-            channel="vcan0"
+            timestamp=10e-4,
+            channel="vcan0",
         ),
         Message(
             # with channel as string
-            channel="awesome_channel"
+            timestamp=11e-4,
+            channel="awesome_channel",
         ),
         Message(
             arbitration_id=0xABCDEF,
             is_extended_id=True,
             timestamp=TEST_TIME,
             data=[1, 2, 3, 4, 5, 6, 7, 8],
         ),
@@ -105,18 +116,18 @@
         ),
     ]
 )
 
 
 TEST_MESSAGES_CAN_FD = sort_messages(
     [
-        Message(is_fd=True, data=range(64)),
-        Message(is_fd=True, data=range(8)),
-        Message(is_fd=True, data=range(8), bitrate_switch=True),
-        Message(is_fd=True, data=range(8), error_state_indicator=True),
+        Message(timestamp=12e-4, is_fd=True, data=range(64)),
+        Message(timestamp=13e-4, is_fd=True, data=range(8)),
+        Message(timestamp=14e-4, is_fd=True, data=range(8), bitrate_switch=True),
+        Message(timestamp=15e-4, is_fd=True, data=range(8), error_state_indicator=True),
     ]
 )
 
 
 TEST_MESSAGES_REMOTE_FRAMES = sort_messages(
     [
         Message(
```

### Comparing `python-can-4.1.0a2/test/data/issue_1256.asc` & `python-can-4.2.0rc0/test/data/issue_1256.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/issue_1299.asc` & `python-can-4.2.0rc0/test/data/issue_1299.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/logfile.asc` & `python-can-4.2.0rc0/test/data/logfile.asc`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-date Sam Sep 30 15:06:13.191 2017
-base hex  timestamps absolute
-internal events logged
-// version 9.0.0
-//0.000000 previous log file: logfile_errorframes.asc
-Begin Triggerblock Sam Sep 30 15:06:13.191 2017
-   0.000000 Start of measurement
-   0.015991 CAN 1 Status:chip status error passive - TxErr: 132 RxErr: 0
-   0.015991 CAN 2 Status:chip status error active
-   1.015991 1  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
-   1.015991 2  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
-   2.015992 1  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
-   2.501000 1 ErrorFrame
-   2.501010 1 ErrorFrame ECC: 10100010
-   2.501020 2 ErrorFrame Flags = 0xe CodeExt = 0x20a2 Code = 0x82 ID = 0 DLC = 0 Position = 5 Length = 11300
-   2.510001 2 100 Tx r
-   2.520002 3 200 Tx r Length = 1704000 BitCount = 145 ID = 88888888x
-   2.584921 4 300 Tx r 8 Length = 1704000 BitCount = 145 ID = 88888888x
-   3.098426 1  18EBFF00x       Rx d 8 01 A0 0F A6 60 3B D1 40    Length = 273910 BitCount = 141 ID = 418119424x
-   3.148421 1  18EBFF00x       Rx d 8 02 1F DE 80 25 DF C0 2B    Length = 271910 BitCount = 140 ID = 418119424x
-   3.197693 1  18EBFF00x       Rx d 8 03 E1 00 4B FF FF 3C 0F    Length = 283910 BitCount = 146 ID = 418119424x
-   3.248765 1  18EBFF00x       Rx d 8 04 00 4B FF FF FF FF FF    Length = 283910 BitCount = 146 ID = 418119424x
-   3.297743 1  J1939TP FEE3p        6    0  0   -   Rx   d 23 A0 0F A6 60 3B D1 40 1F DE 80 25 DF C0 2B E1 00 4B FF FF 3C 0F 00 4B FF FF FF FF FF FF FF FF FF FF FF FF
-  17.876707 CAN 1 Status:chip status error passive - TxErr: 131 RxErr: 0
-  17.876708 1  6F9             Rx   d 8 05 0C 00 00 00 00 00 00  Length = 240015 BitCount = 124 ID = 1785
-  17.876976 1  6F8             Rx   d 8 FF 00 0C FE 00 00 00 00  Length = 239910 BitCount = 124 ID = 1784
-  18.015997 1  Statistic: D 2 R 0 XD 0 XR 0 E 0 O 0 B 0.04%
-  20.105214 2  18EBFF00x       Rx   d 8 01 A0 0F A6 60 3B D1 40  Length = 273925 BitCount = 141 ID = 418119424x
-  20.155119 2  18EBFF00x       Rx   d 8 02 1F DE 80 25 DF C0 2B  Length = 272152 BitCount = 140 ID = 418119424x
-  20.204671 2  18EBFF00x       Rx   d 8 03 E1 00 4B FF FF 3C 0F  Length = 283910 BitCount = 146 ID = 418119424x
-  20.248887 2  18EBFF00x       Rx   d 8 04 00 4B FF FF FF FF FF  Length = 283925 BitCount = 146 ID = 418119424x
-  20.305233 2  J1939TP FEE3p        6    0  0   -   Rx   d 23 A0 0F A6 60 3B D1 40 1F DE 80 25 DF C0 2B E1 00 4B FF FF 3C 0F 00 4B FF FF FF FF FF FF FF FF FF FF FF FF
-  30.005071 CANFD   2 Rx        300  Generic_Name_12                  1 0 8  8 01 02 03 04 05 06 07 08   102203  133   303000 e0006659 46500250 4b140250 20011736 2001040d
-  30.300981 CANFD   3 Tx     50005x                                0 0 5 0 140000 73 200050 7a60 46500250 460a0250 20011736 20010205
-  30.506898 CANFD   4 Rx        4EE                                   0 0 f 64 01 02 03 04 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 64 1331984 11 0 46500250 460a0250 20011736 20010205
-  30.806898 CANFD   5 Tx ErrorFrame Not Acknowledge error, dominant error flag fffe c7 31ca Arb. 556 44 0 0 f 64 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 1331984 11 0 46500250 460a0250 20011736 20010205
-  113.016026 1  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
- 113.016026 2  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
-End TriggerBlock
+date Sam Sep 30 15:06:13.191 2017
+base hex  timestamps absolute
+internal events logged
+// version 9.0.0
+//0.000000 previous log file: logfile_errorframes.asc
+Begin Triggerblock Sam Sep 30 15:06:13.191 2017
+   0.000000 Start of measurement
+   0.015991 CAN 1 Status:chip status error passive - TxErr: 132 RxErr: 0
+   0.015991 CAN 2 Status:chip status error active
+   1.015991 1  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
+   1.015991 2  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
+   2.015992 1  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
+   2.501000 1 ErrorFrame
+   2.501010 1 ErrorFrame ECC: 10100010
+   2.501020 2 ErrorFrame Flags = 0xe CodeExt = 0x20a2 Code = 0x82 ID = 0 DLC = 0 Position = 5 Length = 11300
+   2.510001 2 100 Tx r
+   2.520002 3 200 Tx r Length = 1704000 BitCount = 145 ID = 88888888x
+   2.584921 4 300 Tx r 8 Length = 1704000 BitCount = 145 ID = 88888888x
+   3.098426 1  18EBFF00x       Rx d 8 01 A0 0F A6 60 3B D1 40    Length = 273910 BitCount = 141 ID = 418119424x
+   3.148421 1  18EBFF00x       Rx d 8 02 1F DE 80 25 DF C0 2B    Length = 271910 BitCount = 140 ID = 418119424x
+   3.197693 1  18EBFF00x       Rx d 8 03 E1 00 4B FF FF 3C 0F    Length = 283910 BitCount = 146 ID = 418119424x
+   3.248765 1  18EBFF00x       Rx d 8 04 00 4B FF FF FF FF FF    Length = 283910 BitCount = 146 ID = 418119424x
+   3.297743 1  J1939TP FEE3p        6    0  0   -   Rx   d 23 A0 0F A6 60 3B D1 40 1F DE 80 25 DF C0 2B E1 00 4B FF FF 3C 0F 00 4B FF FF FF FF FF FF FF FF FF FF FF FF
+  17.876707 CAN 1 Status:chip status error passive - TxErr: 131 RxErr: 0
+  17.876708 1  6F9             Rx   d 8 05 0C 00 00 00 00 00 00  Length = 240015 BitCount = 124 ID = 1785
+  17.876976 1  6F8             Rx   d 8 FF 00 0C FE 00 00 00 00  Length = 239910 BitCount = 124 ID = 1784
+  18.015997 1  Statistic: D 2 R 0 XD 0 XR 0 E 0 O 0 B 0.04%
+  20.105214 2  18EBFF00x       Rx   d 8 01 A0 0F A6 60 3B D1 40  Length = 273925 BitCount = 141 ID = 418119424x
+  20.155119 2  18EBFF00x       Rx   d 8 02 1F DE 80 25 DF C0 2B  Length = 272152 BitCount = 140 ID = 418119424x
+  20.204671 2  18EBFF00x       Rx   d 8 03 E1 00 4B FF FF 3C 0F  Length = 283910 BitCount = 146 ID = 418119424x
+  20.248887 2  18EBFF00x       Rx   d 8 04 00 4B FF FF FF FF FF  Length = 283925 BitCount = 146 ID = 418119424x
+  20.305233 2  J1939TP FEE3p        6    0  0   -   Rx   d 23 A0 0F A6 60 3B D1 40 1F DE 80 25 DF C0 2B E1 00 4B FF FF 3C 0F 00 4B FF FF FF FF FF FF FF FF FF FF FF FF
+  30.005071 CANFD   2 Rx        300  Generic_Name_12                  1 0 8  8 01 02 03 04 05 06 07 08   102203  133   303000 e0006659 46500250 4b140250 20011736 2001040d
+  30.300981 CANFD   3 Tx     50005x                                0 0 5 0 140000 73 200050 7a60 46500250 460a0250 20011736 20010205
+  30.506898 CANFD   4 Rx        4EE                                   0 0 f 64 01 02 03 04 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 64 1331984 11 0 46500250 460a0250 20011736 20010205
+  30.806898 CANFD   5 Tx ErrorFrame Not Acknowledge error, dominant error flag fffe c7 31ca Arb. 556 44 0 0 f 64 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 1331984 11 0 46500250 460a0250 20011736 20010205
+  113.016026 1  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
+ 113.016026 2  Statistic: D 0 R 0 XD 0 XR 0 E 0 O 0 B 0.00%
+End TriggerBlock
```

### Comparing `python-can-4.1.0a2/test/data/logfile_errorframes.asc` & `python-can-4.2.0rc0/test/data/logfile_errorframes.asc`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-date Sam Sep 30 15:06:13.191 2017
-base hex  timestamps absolute
-internal events logged
-// version 9.0.0
-Begin Triggerblock Sam Sep 30 15:06:13.191 2017
-   0.000000 Start of measurement
-   0.015991 CAN 1 Status:chip status error passive - TxErr: 132 RxErr: 0
-   0.015991 CAN 2 Status:chip status error active
-   2.501000 1 ErrorFrame
-   2.501010 1 ErrorFrame ECC: 10100010
-   2.501020 2 ErrorFrame Flags = 0xe CodeExt = 0x20a2 Code = 0x82 ID = 0 DLC = 0 Position = 5 Length = 11300
-   2.520002 3 200 Tx r Length = 1704000 BitCount = 145 ID = 88888888x
-   2.584921 4 300 Tx r 8 Length = 1704000 BitCount = 145 ID = 88888888x
-   3.098426 1  18EBFF00x       Rx d 8 01 A0 0F A6 60 3B D1 40    Length = 273910 BitCount = 141 ID = 418119424x
-   3.197693 1  18EBFF00x       Rx d 8 03 E1 00 4B FF FF 3C 0F    Length = 283910 BitCount = 146 ID = 418119424x
-  17.876976 1  6F8             Rx   d 8 FF 00 0C FE 00 00 00 00  Length = 239910 BitCount = 124 ID = 1784
-  20.105214 2  18EBFF00x       Rx   d 8 01 A0 0F A6 60 3B D1 40  Length = 273925 BitCount = 141 ID = 418119424x
-  20.155119 2  18EBFF00x       Rx   d 8 02 1F DE 80 25 DF C0 2B  Length = 272152 BitCount = 140 ID = 418119424x
-  20.204671 2  18EBFF00x       Rx   d 8 03 E1 00 4B FF FF 3C 0F  Length = 283910 BitCount = 146 ID = 418119424x
-  20.248887 2  18EBFF00x       Rx   d 8 04 00 4B FF FF FF FF FF  Length = 283925 BitCount = 146 ID = 418119424x
-End TriggerBlock
+date Sam Sep 30 15:06:13.191 2017
+base hex  timestamps absolute
+internal events logged
+// version 9.0.0
+Begin Triggerblock Sam Sep 30 15:06:13.191 2017
+   0.000000 Start of measurement
+   0.015991 CAN 1 Status:chip status error passive - TxErr: 132 RxErr: 0
+   0.015991 CAN 2 Status:chip status error active
+   2.501000 1 ErrorFrame
+   2.501010 1 ErrorFrame ECC: 10100010
+   2.501020 2 ErrorFrame Flags = 0xe CodeExt = 0x20a2 Code = 0x82 ID = 0 DLC = 0 Position = 5 Length = 11300
+   2.520002 3 200 Tx r Length = 1704000 BitCount = 145 ID = 88888888x
+   2.584921 4 300 Tx r 8 Length = 1704000 BitCount = 145 ID = 88888888x
+   3.098426 1  18EBFF00x       Rx d 8 01 A0 0F A6 60 3B D1 40    Length = 273910 BitCount = 141 ID = 418119424x
+   3.197693 1  18EBFF00x       Rx d 8 03 E1 00 4B FF FF 3C 0F    Length = 283910 BitCount = 146 ID = 418119424x
+  17.876976 1  6F8             Rx   d 8 FF 00 0C FE 00 00 00 00  Length = 239910 BitCount = 124 ID = 1784
+  20.105214 2  18EBFF00x       Rx   d 8 01 A0 0F A6 60 3B D1 40  Length = 273925 BitCount = 141 ID = 418119424x
+  20.155119 2  18EBFF00x       Rx   d 8 02 1F DE 80 25 DF C0 2B  Length = 272152 BitCount = 140 ID = 418119424x
+  20.204671 2  18EBFF00x       Rx   d 8 03 E1 00 4B FF FF 3C 0F  Length = 283910 BitCount = 146 ID = 418119424x
+  20.248887 2  18EBFF00x       Rx   d 8 04 00 4B FF FF FF FF FF  Length = 283925 BitCount = 146 ID = 418119424x
+End TriggerBlock
```

### Comparing `python-can-4.1.0a2/test/data/test_CanErrorFrames.asc` & `python-can-4.2.0rc0/test/data/test_CanErrorFrames.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/test_CanFdMessage.asc` & `python-can-4.2.0rc0/test/data/test_CanFdMessage.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/test_CanFdMessage.blf` & `python-can-4.2.0rc0/test/data/test_CanFdMessage.blf`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/test_CanFdMessage64.asc` & `python-can-4.2.0rc0/test/data/test_CanFdMessage64.asc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/test_CanFdMessage64.blf` & `python-can-4.2.0rc0/test/data/test_CanFdMessage64.blf`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/test_CanMessage.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage.trc`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ;$FILEVERSION=2.1
-;$STARTTIME=0
+;$STARTTIME=43008.920986006946
 ;$COLUMNS=N,O,T,B,I,d,R,L,D
 ;
 ;   C:\Users\User\Desktop\python-can\test\data\test_CanMessage.trc
 ;   Start time: 30.09.2017 22:06:13.191.000
 ;   Generated by PEAK-Converter Version 2.2.4.136
 ;   Data imported from C:\Users\User\Desktop\python-can\test\data\test_CanMessage.asc
 ;-------------------------------------------------------------------------------
```

### Comparing `python-can-4.1.0a2/test/data/test_CanMessage_V1_0_BUS1.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage_V1_0_BUS1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/test_CanMessage_V1_1.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage_V1_1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/test_CanMessage_V2_0_BUS1.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage_V2_0_BUS1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/data/test_CanMessage_V2_1.trc` & `python-can-4.2.0rc0/test/data/test_CanMessage_V2_1.trc`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/listener_test.py` & `python-can-4.2.0rc0/test/listener_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 
 """
 """
 import asyncio
-import unittest
-import random
 import logging
-import tempfile
 import os
+import random
+import tempfile
+import unittest
 import warnings
-from os.path import join, dirname
+from os.path import dirname, join
 
 import can
 
 from .data.example_data import generate_message
 
 logging.basicConfig(level=logging.DEBUG)
 
@@ -84,15 +84,15 @@
         notifier.stop()
         self.assertIn(a_listener, notifier.listeners)
         notifier.remove_listener(a_listener)
         self.assertNotIn(a_listener, notifier.listeners)
 
     def testPlayerTypeResolution(self):
         def test_filetype_to_instance(extension, klass):
-            print("testing: {}".format(extension))
+            print(f"testing: {extension}")
             try:
                 if extension == ".blf":
                     delete = False
                     file_handler = open(
                         join(dirname(__file__), "data", "test_CanMessage.blf")
                     )
                 else:
@@ -119,15 +119,15 @@
         for should_fail_with in ["", ".", ".some_unknown_extention_42"]:
             with self.assertRaises(ValueError):
                 with can.LogReader(should_fail_with):  # make sure we close it anyways
                     pass
 
     def testLoggerTypeResolution(self):
         def test_filetype_to_instance(extension, klass):
-            print("testing: {}".format(extension))
+            print(f"testing: {extension}")
             try:
                 with tempfile.NamedTemporaryFile(
                     suffix=extension, delete=False
                 ) as my_file:
                     filename = my_file.name
                 with can.Logger(filename) as writer:
                     self.assertIsInstance(writer, klass)
```

### Comparing `python-can-4.1.0a2/test/logformats_test.py` & `python-can-4.2.0rc0/test/logformats_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,67 +8,93 @@
 is correct. The types of messages that are tested differs between the
 different writer/reader pairs - e.g., some don't handle error frames and
 comments.
 
 TODO: correctly set preserves_channel and adds_default_channel
 """
 import logging
-import unittest
-from parameterized import parameterized
-import tempfile
 import os
-from abc import abstractmethod, ABCMeta
-from itertools import zip_longest
+import tempfile
+import unittest
+from abc import ABCMeta, abstractmethod
 from datetime import datetime
+from itertools import zip_longest
+
+from parameterized import parameterized
 
 import can
 from can.io import blf
 
 from .data.example_data import (
+    TEST_COMMENTS,
     TEST_MESSAGES_BASE,
-    TEST_MESSAGES_REMOTE_FRAMES,
-    TEST_MESSAGES_ERROR_FRAMES,
     TEST_MESSAGES_CAN_FD,
-    TEST_COMMENTS,
+    TEST_MESSAGES_ERROR_FRAMES,
+    TEST_MESSAGES_REMOTE_FRAMES,
     sort_messages,
 )
 from .message_helper import ComparingMessagesTestCase
 
 logging.basicConfig(level=logging.DEBUG)
 
+try:
+    import asammdf
+except ModuleNotFoundError:
+    asammdf = None
+
 
 class ReaderWriterExtensionTest(unittest.TestCase):
-    message_writers_and_readers = {}
-    for suffix, writer in can.Logger.message_writers.items():
-        message_writers_and_readers[suffix] = (
-            writer,
-            can.LogReader.message_readers.get(suffix),
-        )
+    def _get_suffix_case_variants(self, suffix):
+        return [
+            suffix.upper(),
+            suffix.lower(),
+            f"can.msg.ext{suffix}",
+            "".join([c.upper() if i % 2 else c for i, c in enumerate(suffix)]),
+        ]
 
-    def test_extension_matching(self):
-        for suffix, (writer, reader) in self.message_writers_and_readers.items():
-            suffix_variants = [
-                suffix.upper(),
-                suffix.lower(),
-                f"can.msg.ext{suffix}",
-                "".join([c.upper() if i % 2 else c for i, c in enumerate(suffix)]),
-            ]
-            for suffix_variant in suffix_variants:
-                tmp_file = tempfile.NamedTemporaryFile(
-                    suffix=suffix_variant, delete=False
-                )
-                tmp_file.close()
-                try:
+    def _test_extension(self, suffix):
+        WriterType = can.Logger.message_writers.get(suffix)
+        ReaderType = can.LogReader.message_readers.get(suffix)
+        for suffix_variant in self._get_suffix_case_variants(suffix):
+            tmp_file = tempfile.NamedTemporaryFile(suffix=suffix_variant, delete=False)
+            tmp_file.close()
+            try:
+                if WriterType:
                     with can.Logger(tmp_file.name) as logger:
-                        assert type(logger) == writer
-                    if reader is not None:
-                        with can.LogReader(tmp_file.name) as player:
-                            assert type(player) == reader
-                finally:
-                    os.remove(tmp_file.name)
+                        assert type(logger) == WriterType
+                if ReaderType:
+                    with can.LogReader(tmp_file.name) as player:
+                        assert type(player) == ReaderType
+            finally:
+                os.remove(tmp_file.name)
+
+    def test_extension_matching_asc(self):
+        self._test_extension(".asc")
+
+    def test_extension_matching_blf(self):
+        self._test_extension(".blf")
+
+    def test_extension_matching_csv(self):
+        self._test_extension(".csv")
+
+    def test_extension_matching_db(self):
+        self._test_extension(".db")
+
+    def test_extension_matching_log(self):
+        self._test_extension(".log")
+
+    def test_extension_matching_txt(self):
+        self._test_extension(".txt")
+
+    def test_extension_matching_mf4(self):
+        try:
+            self._test_extension(".mf4")
+        except NotImplementedError:
+            if asammdf is not None:
+                raise
 
 
 class ReaderWriterTest(unittest.TestCase, ComparingMessagesTestCase, metaclass=ABCMeta):
     """Tests a pair of writer and reader by writing all data first and
     then reading all data and checking if they could be reconstructed
     correctly. Optionally writes some comments as well.
 
@@ -137,15 +163,15 @@
             # we filter for not starts with '__' so we do not get all the builtin
             # methods when logging to the console
             attrs = [
                 attr for attr in dir(writer_constructor) if not attr.startswith("__")
             ]
             assert (
                 "log_event" in attrs
-            ), "cannot check comments with this writer: {}".format(writer_constructor)
+            ), f"cannot check comments with this writer: {writer_constructor}"
 
         # get all test comments
         self.original_comments = TEST_COMMENTS if check_comments else ()
 
         self.writer_constructor = writer_constructor
         self.reader_constructor = reader_constructor
         self.binary_file = binary_file
@@ -703,14 +729,30 @@
             test_append=True,
             check_comments=False,
             preserves_channel=False,
             adds_default_channel=None,
         )
 
 
+@unittest.skipIf(asammdf is None, "MF4 is unavailable")
+class TestMF4FileFormat(ReaderWriterTest):
+    """Tests can.MF4Writer and can.MF4Reader"""
+
+    def _setup_instance(self):
+        super()._setup_instance_helper(
+            can.MF4Writer,
+            can.MF4Reader,
+            binary_file=True,
+            check_comments=False,
+            preserves_channel=False,
+            allowed_timestamp_delta=1e-4,
+            adds_default_channel=0,
+        )
+
+
 class TestSqliteDatabaseFormat(ReaderWriterTest):
     """Tests can.SqliteWriter and can.SqliteReader"""
 
     def _setup_instance(self):
         super()._setup_instance_helper(
             can.SqliteWriter,
             can.SqliteReader,
@@ -806,26 +848,27 @@
             return list(reader)
 
 
 class TestTrcFileFormatGen(TestTrcFileFormatBase):
     """Generic tests for can.TRCWriter and can.TRCReader with different file versions"""
 
     def test_can_message(self):
+        start_time = 1506809173.191  # 30.09.2017 22:06:13.191.000 as timestamp
         expected_messages = [
             can.Message(
-                timestamp=2.5010,
+                timestamp=start_time + 2.5010,
                 arbitration_id=0xC8,
                 is_extended_id=False,
                 is_rx=False,
                 channel=1,
                 dlc=8,
                 data=[9, 8, 7, 6, 5, 4, 3, 2],
             ),
             can.Message(
-                timestamp=17.876708,
+                timestamp=start_time + 17.876708,
                 arbitration_id=0x6F9,
                 is_extended_id=False,
                 channel=0,
                 dlc=0x8,
                 data=[5, 0xC, 0, 0, 0, 0, 0, 0],
             ),
         ]
@@ -837,31 +880,38 @@
             ("V1_0", "test_CanMessage_V1_0_BUS1.trc", False),
             ("V1_1", "test_CanMessage_V1_1.trc", True),
             ("V2_1", "test_CanMessage_V2_1.trc", True),
         ]
     )
     def test_can_message_versions(self, name, filename, is_rx_support):
         with self.subTest(name):
+            if name == "V1_0":
+                # Version 1.0 does not support start time
+                start_time = 0
+            else:
+                start_time = (
+                    1639837687.062001  # 18.12.2021 14:28:07.062.001 as timestamp
+                )
 
             def msg_std(timestamp):
                 msg = can.Message(
-                    timestamp=timestamp,
+                    timestamp=timestamp + start_time,
                     arbitration_id=0x000,
                     is_extended_id=False,
                     channel=1,
                     dlc=8,
                     data=[0, 0, 0, 0, 0, 0, 0, 0],
                 )
                 if is_rx_support:
                     msg.is_rx = False
                 return msg
 
             def msg_ext(timestamp):
                 msg = can.Message(
-                    timestamp=timestamp,
+                    timestamp=timestamp + start_time,
                     arbitration_id=0x100,
                     is_extended_id=True,
                     channel=1,
                     dlc=8,
                     data=[0, 0, 0, 0, 0, 0, 0, 0],
                 )
                 if is_rx_support:
```

### Comparing `python-can-4.1.0a2/test/message_helper.py` & `python-can-4.2.0rc0/test/message_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,31 +27,31 @@
         """
         Checks that two messages are equal, according to the given rules.
         """
 
         if message_1.equals(message_2, timestamp_delta=self.allowed_timestamp_delta):
             return
         elif self.preserves_channel:
-            print("Comparing: message 1: {!r}".format(message_1))
-            print("           message 2: {!r}".format(message_2))
+            print(f"Comparing: message 1: {message_1!r}")
+            print(f"           message 2: {message_2!r}")
             self.fail(
                 "messages are unequal with allowed timestamp delta {}".format(
                     self.allowed_timestamp_delta
                 )
             )
         else:
             message_2 = copy(message_2)  # make sure this method is pure
             message_2.channel = message_1.channel
             if message_1.equals(
                 message_2, timestamp_delta=self.allowed_timestamp_delta
             ):
                 return
             else:
-                print("Comparing: message 1: {!r}".format(message_1))
-                print("           message 2: {!r}".format(message_2))
+                print(f"Comparing: message 1: {message_1!r}")
+                print(f"           message 2: {message_2!r}")
                 self.fail(
                     "messages are unequal with allowed timestamp delta {} even when ignoring channels".format(
                         self.allowed_timestamp_delta
                     )
                 )
 
     def assertMessagesEqual(self, messages_1, messages_2):
```

### Comparing `python-can-4.1.0a2/test/network_test.py` & `python-can-4.2.0rc0/test/network_test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 
-import unittest
-import threading
-import random
 import logging
+import random
+import threading
+import unittest
 
 logging.getLogger(__file__).setLevel(logging.WARNING)
 
 # make a random bool:
 rbool = lambda: bool(round(random.random()))
 
 import can
```

### Comparing `python-can-4.1.0a2/test/notifier_test.py` & `python-can-4.2.0rc0/test/notifier_test.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
-import unittest
-import time
 import asyncio
+import time
+import unittest
 
 import can
 
 
 class NotifierTest(unittest.TestCase):
     def test_single_bus(self):
         with can.Bus("test", interface="virtual", receive_own_messages=True) as bus:
```

### Comparing `python-can-4.1.0a2/test/serial_test.py` & `python-can-4.2.0rc0/test/serial_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 
 import unittest
 from unittest.mock import patch
 
 import can
 from can.interfaces.serial.serial_can import SerialBus
 
-from .message_helper import ComparingMessagesTestCase
 from .config import IS_PYPY
-
+from .message_helper import ComparingMessagesTestCase
 
 # Mentioned in #1010
 TIMEOUT = 0.5 if IS_PYPY else 0.1  # 0.1 is the default set in SerialBus
 
 
 class SerialDummy:
     """
@@ -40,15 +39,14 @@
         self.msg = bytearray(msg)
 
     def reset(self):
         self.msg = None
 
 
 class SimpleSerialTestBase(ComparingMessagesTestCase):
-
     MAX_TIMESTAMP = 0xFFFFFFFF / 1000
 
     def __init__(self):
         ComparingMessagesTestCase.__init__(
             self, allowed_timestamp_delta=None, preserves_channel=True
         )
```

### Comparing `python-can-4.1.0a2/test/simplecyclic_test.py` & `python-can-4.2.0rc0/test/simplecyclic_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 """
 This module tests cyclic send tasks.
 """
 
-from time import sleep
+import gc
 import unittest
+from time import sleep
 from unittest.mock import MagicMock
-import gc
 
 import can
 
 from .config import *
 from .message_helper import ComparingMessagesTestCase
 
 
@@ -27,17 +27,16 @@
         "the timing sensitive behaviour cannot be reproduced reliably on a CI server",
     )
     def test_cycle_time(self):
         msg = can.Message(
             is_extended_id=False, arbitration_id=0x123, data=[0, 1, 2, 3, 4, 5, 6, 7]
         )
 
-        with can.interface.Bus(bustype="virtual") as bus1:
-            with can.interface.Bus(bustype="virtual") as bus2:
-
+        with can.interface.Bus(interface="virtual") as bus1:
+            with can.interface.Bus(interface="virtual") as bus2:
                 # disabling the garbage collector makes the time readings more reliable
                 gc.disable()
 
                 task = bus1.send_periodic(msg, 0.01, 1)
                 self.assertIsInstance(task, can.broadcastmanager.CyclicSendTaskABC)
 
                 sleep(2)
@@ -63,15 +62,15 @@
                 # Set timestamp and channel to match recv'd because we don't care
                 # and they are not initialized by the can.Message constructor.
                 msg.timestamp = last_msg.timestamp
                 msg.channel = last_msg.channel
                 self.assertMessageEqual(msg, last_msg)
 
     def test_removing_bus_tasks(self):
-        bus = can.interface.Bus(bustype="virtual")
+        bus = can.interface.Bus(interface="virtual")
         tasks = []
         for task_i in range(10):
             msg = can.Message(
                 is_extended_id=False,
                 arbitration_id=0x123,
                 data=[0, 1, 2, 3, 4, 5, 6, 7],
             )
@@ -86,15 +85,15 @@
             # Note calling task.stop will remove the task from the Bus's internal task management list
             task.stop()
 
         assert len(bus._periodic_tasks) == 0
         bus.shutdown()
 
     def test_managed_tasks(self):
-        bus = can.interface.Bus(bustype="virtual", receive_own_messages=True)
+        bus = can.interface.Bus(interface="virtual", receive_own_messages=True)
         tasks = []
         for task_i in range(3):
             msg = can.Message(
                 is_extended_id=False,
                 arbitration_id=0x123,
                 data=[0, 1, 2, 3, 4, 5, 6, 7],
             )
@@ -116,15 +115,15 @@
 
         for task in tasks:
             assert task.thread.join(5.0) is None, "Task didn't stop before timeout"
 
         bus.shutdown()
 
     def test_stopping_perodic_tasks(self):
-        bus = can.interface.Bus(bustype="virtual")
+        bus = can.interface.Bus(interface="virtual")
         tasks = []
         for task_i in range(10):
             msg = can.Message(
                 is_extended_id=False,
                 arbitration_id=0x123,
                 data=[0, 1, 2, 3, 4, 5, 6, 7],
             )
@@ -149,15 +148,15 @@
         # still be associated with the bus (e.g. for restarting)
         assert len(bus._periodic_tasks) == 5
 
         bus.shutdown()
 
     @unittest.skipIf(IS_CI, "fails randomly when run on CI server")
     def test_thread_based_cyclic_send_task(self):
-        bus = can.ThreadSafeBus(bustype="virtual")
+        bus = can.ThreadSafeBus(interface="virtual")
         msg = can.Message(
             is_extended_id=False, arbitration_id=0x123, data=[0, 1, 2, 3, 4, 5, 6, 7]
         )
 
         # good case, bus is up
         on_error_mock = MagicMock(return_value=False)
         task = can.broadcastmanager.ThreadBasedCyclicSendTask(
```

### Comparing `python-can-4.1.0a2/test/test_cantact.py` & `python-can-4.2.0rc0/test/test_cantact.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,51 +8,51 @@
 
 import can
 from can.interfaces import cantact
 
 
 class CantactTest(unittest.TestCase):
     def test_bus_creation(self):
-        bus = can.Bus(channel=0, bustype="cantact", _testing=True)
+        bus = can.Bus(channel=0, interface="cantact", _testing=True)
         self.assertIsInstance(bus, cantact.CantactBus)
         cantact.MockInterface.set_bitrate.assert_called()
         cantact.MockInterface.set_bit_timing.assert_not_called()
         cantact.MockInterface.set_enabled.assert_called()
         cantact.MockInterface.set_monitor.assert_called()
         cantact.MockInterface.start.assert_called()
 
     def test_bus_creation_bittiming(self):
         cantact.MockInterface.set_bitrate.reset_mock()
 
-        bt = can.BitTiming(tseg1=13, tseg2=2, brp=6, sjw=1)
-        bus = can.Bus(channel=0, bustype="cantact", bit_timing=bt, _testing=True)
+        bt = can.BitTiming(f_clock=24_000_000, brp=3, tseg1=13, tseg2=2, sjw=1)
+        bus = can.Bus(channel=0, interface="cantact", timing=bt, _testing=True)
         self.assertIsInstance(bus, cantact.CantactBus)
         cantact.MockInterface.set_bitrate.assert_not_called()
         cantact.MockInterface.set_bit_timing.assert_called()
         cantact.MockInterface.set_enabled.assert_called()
         cantact.MockInterface.set_monitor.assert_called()
         cantact.MockInterface.start.assert_called()
 
     def test_transmit(self):
-        bus = can.Bus(channel=0, bustype="cantact", _testing=True)
+        bus = can.Bus(channel=0, interface="cantact", _testing=True)
         msg = can.Message(
             arbitration_id=0xC0FFEF, data=[1, 2, 3, 4, 5, 6, 7, 8], is_extended_id=True
         )
         bus.send(msg)
         cantact.MockInterface.send.assert_called()
 
     def test_recv(self):
-        bus = can.Bus(channel=0, bustype="cantact", _testing=True)
+        bus = can.Bus(channel=0, interface="cantact", _testing=True)
         frame = bus.recv(timeout=0.5)
         cantact.MockInterface.recv.assert_called()
         self.assertIsInstance(frame, can.Message)
 
     def test_recv_timeout(self):
-        bus = can.Bus(channel=0, bustype="cantact", _testing=True)
+        bus = can.Bus(channel=0, interface="cantact", _testing=True)
         frame = bus.recv(timeout=0.0)
         cantact.MockInterface.recv.assert_called()
         self.assertIsNone(frame)
 
     def test_shutdown(self):
-        bus = can.Bus(channel=0, bustype="cantact", _testing=True)
+        bus = can.Bus(channel=0, interface="cantact", _testing=True)
         bus.shutdown()
         cantact.MockInterface.stop.assert_called()
```

### Comparing `python-can-4.1.0a2/test/test_cyclic_socketcan.py` & `python-can-4.2.0rc0/test/test_cyclic_socketcan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """
 This module tests multiple message cyclic send tasks.
 """
+import time
 import unittest
 
-import time
 import can
 
 from .config import TEST_INTERFACE_SOCKETCAN
 
 
 @unittest.skipUnless(TEST_INTERFACE_SOCKETCAN, "skip testing of socketcan")
 class CyclicSocketCan(unittest.TestCase):
@@ -252,22 +252,16 @@
             data=[0x11, 0x11, 0x11, 0x11, 0x11, 0x11],
             is_extended_id=False,
         )
 
         task_a = self._send_bus.send_periodic(messages_a, self.PERIOD)
         time.sleep(0.1)
 
-        # Try to start it again, task_id is not incremented in this case
-        with self.assertRaises(can.CanOperationError) as ctx:
-            task_a.start()
-        self.assertEqual(
-            "A periodic task for task ID 1 is already in progress by the SocketCAN Linux layer",
-            str(ctx.exception),
-        )
-
+        # Task restarting is permitted as of #1440
+        task_a.start()
         task_a.stop()
 
     def test_create_same_id(self):
         messages_a = can.Message(
             arbitration_id=0x401,
             data=[0x11, 0x11, 0x11, 0x11, 0x11, 0x11],
             is_extended_id=False,
```

### Comparing `python-can-4.1.0a2/test/test_detect_available_configs.py` & `python-can-4.2.0rc0/test/test_detect_available_configs.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/test_interface_canalystii.py` & `python-can-4.2.0rc0/test/test_interface_canalystii.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 
 """
 """
 
-import time
 import unittest
-from unittest.mock import Mock, patch, call
 from ctypes import c_ubyte
+from unittest.mock import call, patch
 
 import canalystii as driver  # low-level driver module, mock out this layer
+
 import can
 from can.interfaces.canalystii import CANalystIIBus
 
 
 def create_mock_device():
     return patch("canalystii.CanalystDevice")
 
@@ -35,34 +35,30 @@
                 instance = mock_device.return_value
                 bus = CANalystIIBus(channel, bitrate=1000000)
                 instance.init.assert_called_once_with(channel, bitrate=1000000)
 
     def test_initialize_with_timing_registers(self):
         with create_mock_device() as mock_device:
             instance = mock_device.return_value
-            timing = can.BitTiming(btr0=0x03, btr1=0x6F)
-            bus = CANalystIIBus(bitrate=None, bit_timing=timing)
+            timing = can.BitTiming.from_registers(
+                f_clock=8_000_000, btr0=0x03, btr1=0x6F
+            )
+            bus = CANalystIIBus(bitrate=None, timing=timing)
             instance.init.assert_has_calls(
                 [
                     call(0, timing0=0x03, timing1=0x6F),
                     call(1, timing0=0x03, timing1=0x6F),
                 ]
             )
 
     def test_missing_bitrate(self):
         with self.assertRaises(ValueError) as cm:
-            bus = CANalystIIBus(0, bitrate=None, bit_timing=None)
+            bus = CANalystIIBus(0, bitrate=None, timing=None)
         self.assertIn("bitrate", str(cm.exception))
 
-    def test_invalid_bit_timing(self):
-        with create_mock_device() as mock_device:
-            with self.assertRaises(ValueError) as cm:
-                invalid_timings = can.BitTiming()
-                CANalystIIBus(0, bit_timing=invalid_timings)
-
     def test_receive_message(self):
         driver_message = driver.Message(
             can_id=0x333,
             timestamp=1000000,
             time_flag=1,
             send_type=0,
             remote=False,
```

### Comparing `python-can-4.1.0a2/test/test_interface_ixxat_fd.py` & `python-can-4.2.0rc0/test/test_interface_ixxat_fd.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Unittest for ixxat interface using fd option.
 
 Run only this test:
 python setup.py test --addopts "--verbose -s test/test_interface_ixxat_fd.py"
 """
 
 import unittest
+
 import can
 
 
 class SoftwareTestCase(unittest.TestCase):
     """
     Test cases that test the software only and do not rely on an existing/connected hardware.
     """
```

### Comparing `python-can-4.1.0a2/test/test_interface_virtual.py` & `python-can-4.2.0rc0/test/test_interface_virtual.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python
-# coding: utf-8
 
 """
 This module tests :meth:`can.interface.virtual`.
 """
 
 import unittest
 
 from can import Bus, Message
 
 EXAMPLE_MSG1 = Message(timestamp=1639739471.5565314, arbitration_id=0x481, data=b"\x01")
 
 
 class TestMessageFiltering(unittest.TestCase):
     def setUp(self):
-        self.node1 = Bus("test", bustype="virtual", preserve_timestamps=True)
-        self.node2 = Bus("test", bustype="virtual")
+        self.node1 = Bus("test", interface="virtual", preserve_timestamps=True)
+        self.node2 = Bus("test", interface="virtual")
 
     def tearDown(self):
         self.node1.shutdown()
         self.node2.shutdown()
 
     def test_sendmsg(self):
         self.node2.send(EXAMPLE_MSG1)
```

### Comparing `python-can-4.1.0a2/test/test_kvaser.py` & `python-can-4.2.0rc0/test/test_kvaser.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 import time
 import unittest
 from unittest.mock import Mock
 
 import pytest
 
 import can
-from can.interfaces.kvaser import canlib
-from can.interfaces.kvaser import constants
+from can.interfaces.kvaser import canlib, constants
 
 
 class KvaserTest(unittest.TestCase):
     def setUp(self):
         canlib.canGetNumberOfChannels = KvaserTest.canGetNumberOfChannels
         canlib.canOpenChannel = Mock(return_value=0)
         canlib.canIoCtl = Mock(return_value=0)
@@ -33,15 +32,15 @@
         canlib.canWrite = self.canWrite
         canlib.canReadWait = self.canReadWait
         canlib.canGetBusStatistics = Mock()
         canlib.canRequestBusStatistics = Mock()
 
         self.msg = {}
         self.msg_in_cue = None
-        self.bus = can.Bus(channel=0, bustype="kvaser")
+        self.bus = can.Bus(channel=0, interface="kvaser")
 
     def tearDown(self):
         if self.bus:
             self.bus.shutdown()
             self.bus = None
 
     def test_bus_creation(self):
@@ -145,38 +144,38 @@
             {"interface": "kvaser", "channel": 1},
         ]
         self.assertListEqual(configs, expected)
 
     def test_canfd_default_data_bitrate(self):
         canlib.canSetBusParams.reset_mock()
         canlib.canSetBusParamsFd.reset_mock()
-        can.Bus(channel=0, bustype="kvaser", fd=True)
+        can.Bus(channel=0, interface="kvaser", fd=True)
         canlib.canSetBusParams.assert_called_once_with(
             0, constants.canFD_BITRATE_500K_80P, 0, 0, 0, 0, 0
         )
         canlib.canSetBusParamsFd.assert_called_once_with(
             0, constants.canFD_BITRATE_500K_80P, 0, 0, 0
         )
 
     def test_canfd_nondefault_data_bitrate(self):
         canlib.canSetBusParams.reset_mock()
         canlib.canSetBusParamsFd.reset_mock()
         data_bitrate = 2000000
-        can.Bus(channel=0, bustype="kvaser", fd=True, data_bitrate=data_bitrate)
+        can.Bus(channel=0, interface="kvaser", fd=True, data_bitrate=data_bitrate)
         bitrate_constant = canlib.BITRATE_FD[data_bitrate]
         canlib.canSetBusParams.assert_called_once_with(
             0, constants.canFD_BITRATE_500K_80P, 0, 0, 0, 0, 0
         )
         canlib.canSetBusParamsFd.assert_called_once_with(0, bitrate_constant, 0, 0, 0)
 
     def test_canfd_custom_data_bitrate(self):
         canlib.canSetBusParams.reset_mock()
         canlib.canSetBusParamsFd.reset_mock()
         data_bitrate = 123456
-        can.Bus(channel=0, bustype="kvaser", fd=True, data_bitrate=data_bitrate)
+        can.Bus(channel=0, interface="kvaser", fd=True, data_bitrate=data_bitrate)
         canlib.canSetBusParams.assert_called_once_with(
             0, constants.canFD_BITRATE_500K_80P, 0, 0, 0, 0, 0
         )
         canlib.canSetBusParamsFd.assert_called_once_with(0, data_bitrate, 0, 0, 0)
 
     def test_bus_get_stats(self):
         stats = self.bus.get_stats()
```

### Comparing `python-can-4.1.0a2/test/test_load_config.py` & `python-can-4.2.0rc0/test/test_load_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #!/usr/bin/env python
 
-import os
 import shutil
 import tempfile
 import unittest
+import unittest.mock
 from tempfile import NamedTemporaryFile
 
 import can
 
 
 class LoadConfigTest(unittest.TestCase):
-    configuration = {
+    configuration_in = {
         "default": {"interface": "serial", "channel": "0"},
         "one": {"interface": "kvaser", "channel": "1", "bitrate": 100000},
         "two": {"channel": "2"},
     }
+    configuration_out = {
+        "default": {"interface": "serial", "channel": 0},
+        "one": {"interface": "kvaser", "channel": 1, "bitrate": 100000},
+        "two": {"channel": 2},
+    }
 
     def setUp(self):
         # Create a temporary directory
         self.test_dir = tempfile.mkdtemp()
 
     def tearDown(self):
         # Remove the directory after the test
@@ -26,61 +31,61 @@
 
     def _gen_configration_file(self, sections):
         with NamedTemporaryFile(
             mode="w", dir=self.test_dir, delete=False
         ) as tmp_config_file:
             content = []
             for section in sections:
-                content.append("[{}]".format(section))
-                for k, v in self.configuration[section].items():
-                    content.append("{} = {}".format(k, v))
+                content.append(f"[{section}]")
+                for k, v in self.configuration_in[section].items():
+                    content.append(f"{k} = {v}")
             tmp_config_file.write("\n".join(content))
             return tmp_config_file.name
 
     def _dict_to_env(self, d):
         return {f"CAN_{k.upper()}": str(v) for k, v in d.items()}
 
     def test_config_default(self):
         tmp_config = self._gen_configration_file(["default"])
         config = can.util.load_config(path=tmp_config)
-        self.assertEqual(config, self.configuration["default"])
+        self.assertEqual(config, self.configuration_out["default"])
 
     def test_config_whole_default(self):
-        tmp_config = self._gen_configration_file(self.configuration)
+        tmp_config = self._gen_configration_file(self.configuration_in)
         config = can.util.load_config(path=tmp_config)
-        self.assertEqual(config, self.configuration["default"])
+        self.assertEqual(config, self.configuration_out["default"])
 
     def test_config_whole_context(self):
-        tmp_config = self._gen_configration_file(self.configuration)
+        tmp_config = self._gen_configration_file(self.configuration_in)
         config = can.util.load_config(path=tmp_config, context="one")
-        self.assertEqual(config, self.configuration["one"])
+        self.assertEqual(config, self.configuration_out["one"])
 
     def test_config_merge_context(self):
-        tmp_config = self._gen_configration_file(self.configuration)
+        tmp_config = self._gen_configration_file(self.configuration_in)
         config = can.util.load_config(path=tmp_config, context="two")
-        expected = self.configuration["default"]
-        expected.update(self.configuration["two"])
+        expected = self.configuration_out["default"].copy()
+        expected.update(self.configuration_out["two"])
         self.assertEqual(config, expected)
 
     def test_config_merge_environment_to_context(self):
-        tmp_config = self._gen_configration_file(self.configuration)
+        tmp_config = self._gen_configration_file(self.configuration_in)
         env_data = {"interface": "serial", "bitrate": 125000}
         env_dict = self._dict_to_env(env_data)
         with unittest.mock.patch.dict("os.environ", env_dict):
             config = can.util.load_config(path=tmp_config, context="one")
-        expected = self.configuration["one"]
+        expected = self.configuration_out["one"].copy()
         expected.update(env_data)
         self.assertEqual(config, expected)
 
     def test_config_whole_environment(self):
-        tmp_config = self._gen_configration_file(self.configuration)
+        tmp_config = self._gen_configration_file(self.configuration_in)
         env_data = {"interface": "socketcan", "channel": "3", "bitrate": 250000}
         env_dict = self._dict_to_env(env_data)
         with unittest.mock.patch.dict("os.environ", env_dict):
             config = can.util.load_config(path=tmp_config, context="one")
-        expected = self.configuration["one"]
-        expected.update(env_data)
+        expected = self.configuration_out["one"].copy()
+        expected.update({"interface": "socketcan", "channel": 3, "bitrate": 250000})
         self.assertEqual(config, expected)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `python-can-4.1.0a2/test/test_load_file_config.py` & `python-can-4.2.0rc0/test/test_load_file_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
     def _gen_configration_file(self, sections):
         with NamedTemporaryFile(
             mode="w", dir=self.test_dir, delete=False
         ) as tmp_config_file:
             content = []
             for section in sections:
-                content.append("[{}]".format(section))
+                content.append(f"[{section}]")
                 for k, v in self.configuration[section].items():
-                    content.append("{} = {}".format(k, v))
+                    content.append(f"{k} = {v}")
             tmp_config_file.write("\n".join(content))
             return tmp_config_file.name
 
     def test_config_file_with_default(self):
         tmp_config = self._gen_configration_file(["default"])
         config = can.util.load_file_config(path=tmp_config)
         self.assertEqual(config, self.configuration["default"])
```

### Comparing `python-can-4.1.0a2/test/test_logger.py` & `python-can-4.2.0rc0/test/test_logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 
 """
 This module tests the functions inside of logger.py
 """
 
-import unittest
-from unittest import mock
-from unittest.mock import Mock
 import gzip
 import os
 import sys
+import unittest
+from unittest import mock
+from unittest.mock import Mock
 
 import pytest
 
 import can
 import can.logger
 
 from .config import *
```

### Comparing `python-can-4.1.0a2/test/test_message_class.py` & `python-can-4.2.0rc0/test/test_message_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 
-import unittest
+import pickle
 import sys
-from math import isinf, isnan
+import unittest
 from copy import copy, deepcopy
-import pickle
 from datetime import timedelta
+from math import isinf, isnan
 
-from hypothesis import HealthCheck, given, settings
 import hypothesis.errors
 import hypothesis.strategies as st
+import pytest
+from hypothesis import HealthCheck, given, settings
 
 from can import Message
 
+from .config import IS_GITHUB_ACTIONS, IS_PYPY, IS_WINDOWS
 from .message_helper import ComparingMessagesTestCase
-from .config import IS_GITHUB_ACTIONS, IS_WINDOWS, IS_PYPY
-
-import pytest
 
 
 class TestMessageClass(unittest.TestCase):
     """
     This test tries many inputs to the message class constructor and then sanity checks
     all methods and ensures that nothing crashes. It also checks whether Message._check()
     allows all valid can frames.
@@ -83,16 +82,16 @@
                 Message(check=True, **kwargs)
 
         self.assertGreater(len(str(message)), 0)
         self.assertGreater(len(message.__repr__()), 0)
         if is_valid:
             self.assertEqual(len(message), kwargs["dlc"])
         self.assertTrue(bool(message))
-        self.assertGreater(len("{}".format(message)), 0)
-        _ = "{}".format(message)
+        self.assertGreater(len(f"{message}"), 0)
+        _ = f"{message}"
         with self.assertRaises(Exception):
             _ = "{somespec}".format(
                 message
             )  # pylint: disable=missing-format-argument-key
         if sys.version_info.major > 2:
             self.assertEqual(bytearray(bytes(message)), kwargs["data"])
```

### Comparing `python-can-4.1.0a2/test/test_message_filtering.py` & `python-can-4.2.0rc0/test/test_message_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 
 import unittest
 
 from can import Bus, Message
 
 from .data.example_data import TEST_ALL_MESSAGES
 
-
 EXAMPLE_MSG = Message(arbitration_id=0x123, is_extended_id=True)
 HIGHEST_MSG = Message(arbitration_id=0x1FFFFFFF, is_extended_id=True)
 
 MATCH_EXAMPLE = [{"can_id": 0x123, "can_mask": 0x1FFFFFFF, "extended": True}]
 
 MATCH_ONLY_HIGHEST = [{"can_id": 0xFFFFFFFF, "can_mask": 0x1FFFFFFF, "extended": True}]
 
 
 class TestMessageFiltering(unittest.TestCase):
     def setUp(self):
-        self.bus = Bus(bustype="virtual", channel="testy")
+        self.bus = Bus(interface="virtual", channel="testy")
 
     def tearDown(self):
         self.bus.shutdown()
 
     def test_match_all(self):
         # explicitly
         self.bus.set_filters()
```

### Comparing `python-can-4.1.0a2/test/test_message_sync.py` & `python-can-4.2.0rc0/test/test_message_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 
 """
 This module tests :class:`can.MessageSync`.
 """
 
-from copy import copy
-import time
 import gc
-
+import time
 import unittest
+from copy import copy
+
 import pytest
 
-from can import MessageSync, Message
+from can import Message, MessageSync
 
-from .config import IS_CI, IS_TRAVIS, IS_OSX, IS_GITHUB_ACTIONS, IS_LINUX
-from .message_helper import ComparingMessagesTestCase
+from .config import IS_CI, IS_GITHUB_ACTIONS, IS_LINUX, IS_OSX, IS_TRAVIS
 from .data.example_data import TEST_MESSAGES_BASE
-
+from .message_helper import ComparingMessagesTestCase
 
 TEST_FEWER_MESSAGES = TEST_MESSAGES_BASE[::2]
 
 
 def inc(value):
     """Makes the test boundaries give some more space when run on the CI server."""
     if IS_CI:
@@ -83,15 +82,15 @@
         before = time.perf_counter()
         collected = list(sync)
         after = time.perf_counter()
         took = after - before
 
         # the handling of the messages itself also takes some time:
         # ~0.001 s/message on a ThinkPad T560 laptop (Ubuntu 18.04, i5-6200U)
-        assert 0 < took < inc(len(messages) * (0.005 + 0.003)), "took: {}s".format(took)
+        assert 0 < took < inc(len(messages) * (0.005 + 0.003)), f"took: {took}s"
 
         self.assertMessagesEqual(messages, collected)
 
 
 @skip_on_unreliable_platforms
 @pytest.mark.parametrize(
     "timestamp_1,timestamp_2", [(0.0, 0.0), (0.0, 0.01), (0.01, 1.5)]
```

### Comparing `python-can-4.1.0a2/test/test_neousys.py` & `python-can-4.2.0rc0/test/test_neousys.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 #!/usr/bin/env python
 
-import ctypes
-import os
-import pickle
 import unittest
-from unittest.mock import Mock
-
 from ctypes import (
+    POINTER,
     byref,
+    c_ubyte,
     cast,
-    POINTER,
     sizeof,
-    c_ubyte,
 )
-
-import pytest
+from unittest.mock import Mock
 
 import can
 from can.interfaces.neousys import neousys
 
 
 class TestNeousysBus(unittest.TestCase):
     def setUp(self) -> None:
@@ -29,29 +23,29 @@
         can.interfaces.neousys.neousys.NEOUSYS_CANLIB.CAN_RegisterStatus = Mock(
             return_value=1
         )
         can.interfaces.neousys.neousys.NEOUSYS_CANLIB.CAN_Setup = Mock(return_value=1)
         can.interfaces.neousys.neousys.NEOUSYS_CANLIB.CAN_Start = Mock(return_value=1)
         can.interfaces.neousys.neousys.NEOUSYS_CANLIB.CAN_Send = Mock(return_value=1)
         can.interfaces.neousys.neousys.NEOUSYS_CANLIB.CAN_Stop = Mock(return_value=1)
-        self.bus = can.Bus(channel=0, bustype="neousys")
+        self.bus = can.Bus(channel=0, interface="neousys")
 
     def tearDown(self) -> None:
         if self.bus:
             self.bus.shutdown()
             self.bus = None
 
     def test_bus_creation(self) -> None:
         self.assertIsInstance(self.bus, neousys.NeousysBus)
-        self.assertTrue(neousys.NEOUSYS_CANLIB.CAN_Setup.called)
-        self.assertTrue(neousys.NEOUSYS_CANLIB.CAN_Start.called)
-        self.assertTrue(neousys.NEOUSYS_CANLIB.CAN_RegisterReceived.called)
-        self.assertTrue(neousys.NEOUSYS_CANLIB.CAN_RegisterStatus.called)
-        self.assertTrue(neousys.NEOUSYS_CANLIB.CAN_Send.not_called)
-        self.assertTrue(neousys.NEOUSYS_CANLIB.CAN_Stop.not_called)
+        neousys.NEOUSYS_CANLIB.CAN_Setup.assert_called()
+        neousys.NEOUSYS_CANLIB.CAN_Start.assert_called()
+        neousys.NEOUSYS_CANLIB.CAN_RegisterReceived.assert_called()
+        neousys.NEOUSYS_CANLIB.CAN_RegisterStatus.assert_called()
+        neousys.NEOUSYS_CANLIB.CAN_Send.assert_not_called()
+        neousys.NEOUSYS_CANLIB.CAN_Stop.assert_not_called()
 
         CAN_Start_args = (
             can.interfaces.neousys.neousys.NEOUSYS_CANLIB.CAN_Setup.call_args[0]
         )
 
         # sizeof struct should be 16
         self.assertEqual(CAN_Start_args[0], 0)
@@ -62,15 +56,15 @@
         self.assertEqual(NeousysCanSetup_struct.contents.bitRate, 500000)
         self.assertEqual(
             NeousysCanSetup_struct.contents.recvConfig,
             neousys.NEOUSYS_CAN_MSG_USE_ID_FILTER,
         )
 
     def test_bus_creation_bitrate(self) -> None:
-        self.bus = can.Bus(channel=0, bustype="neousys", bitrate=200000)
+        self.bus = can.Bus(channel=0, interface="neousys", bitrate=200000)
         self.assertIsInstance(self.bus, neousys.NeousysBus)
         CAN_Start_args = (
             can.interfaces.neousys.neousys.NEOUSYS_CANLIB.CAN_Setup.call_args[0]
         )
 
         # sizeof struct should be 16
         self.assertEqual(CAN_Start_args[0], 0)
@@ -97,16 +91,16 @@
         self.assertSequenceEqual(recv_msg.data, msg_data)
 
     def test_send(self) -> None:
         msg = can.Message(
             arbitration_id=0x01, data=[1, 2, 3, 4, 5, 6, 7, 8], is_extended_id=False
         )
         self.bus.send(msg)
-        self.assertTrue(neousys.NEOUSYS_CANLIB.CAN_Send.called)
+        neousys.NEOUSYS_CANLIB.CAN_Send.assert_called()
 
     def test_shutdown(self) -> None:
         self.bus.shutdown()
-        self.assertTrue(neousys.NEOUSYS_CANLIB.CAN_Stop.called)
+        neousys.NEOUSYS_CANLIB.CAN_Stop.assert_called()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `python-can-4.1.0a2/test/test_neovi.py` & `python-can-4.2.0rc0/test/test_neovi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 """
 """
 import pickle
 import unittest
+
 from can.interfaces.ics_neovi import ICSApiError
 
 
 class ICSApiErrorTest(unittest.TestCase):
     def test_error_pickling(self):
         iae = ICSApiError(
             0xF00,
```

### Comparing `python-can-4.1.0a2/test/test_player.py` & `python-can-4.2.0rc0/test/test_player.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 
 """
 This module tests the functions inside of player.py
 """
 
+import io
+import os
+import sys
 import unittest
 from unittest import mock
 from unittest.mock import Mock
-import os
-import sys
-import io
+
 import can
 import can.player
 
 
 class TestPlayerScriptModule(unittest.TestCase):
-
     logfile = os.path.join(os.path.dirname(__file__), "data", "test_CanMessage.asc")
 
     def setUp(self) -> None:
         # Patch VirtualBus object
         patcher_virtual_bus = mock.patch("can.interfaces.virtual.VirtualBus", spec=True)
         self.MockVirtualBus = patcher_virtual_bus.start()
         self.addCleanup(patcher_virtual_bus.stop)
```

### Comparing `python-can-4.1.0a2/test/test_robotell.py` & `python-can-4.2.0rc0/test/test_robotell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python
 
 import unittest
+
 import can
 
 
 class robotellTestCase(unittest.TestCase):
     def setUp(self):
         # will log timeout messages since we are not feeding ack messages to the serial port at this stage
-        self.bus = can.Bus("loop://", bustype="robotell")
+        self.bus = can.Bus("loop://", interface="robotell")
         self.serial = self.bus.serialPortOrig
         self.serial.read(self.serial.in_waiting)
 
     def tearDown(self):
         self.bus.shutdown()
 
     def test_recv_extended(self):
```

### Comparing `python-can-4.1.0a2/test/test_rotating_loggers.py` & `python-can-4.2.0rc0/test/test_rotating_loggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 import os
 from pathlib import Path
 from unittest.mock import Mock
 
 import can
+
 from .data.example_data import generate_message
 
 
 class TestBaseRotatingLogger:
     @staticmethod
     def _get_instance(path, *args, **kwargs) -> can.io.BaseRotatingLogger:
         class SubClass(can.io.BaseRotatingLogger):
```

### Comparing `python-can-4.1.0a2/test/test_scripts.py` & `python-can-4.2.0rc0/test/test_scripts.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 """
 This module tests that the scripts are all callable.
 """
 
+import errno
 import subprocess
-import unittest
 import sys
-import errno
+import unittest
 from abc import ABCMeta, abstractmethod
 
 from .config import *
 
 
 class CanScriptTest(unittest.TestCase, metaclass=ABCMeta):
     @classmethod
```

### Comparing `python-can-4.1.0a2/test/test_socketcan.py` & `python-can-4.2.0rc0/test/test_socketcan.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,35 @@
 
 """
 Test functions in `can.interfaces.socketcan.socketcan`.
 """
 import ctypes
 import struct
 import unittest
+import warnings
 from unittest.mock import patch
 
-from can.interfaces.socketcan.socketcan import (
-    bcm_header_factory,
-    build_bcm_header,
-    build_bcm_tx_delete_header,
-    build_bcm_transmit_header,
-    build_bcm_update_header,
-    BcmMsgHead,
-)
+import can
 from can.interfaces.socketcan.constants import (
     CAN_BCM_TX_DELETE,
     CAN_BCM_TX_SETUP,
     SETTIMER,
     STARTTIMER,
     TX_COUNTEVT,
 )
+from can.interfaces.socketcan.socketcan import (
+    BcmMsgHead,
+    bcm_header_factory,
+    build_bcm_header,
+    build_bcm_transmit_header,
+    build_bcm_tx_delete_header,
+    build_bcm_update_header,
+)
+
+from .config import IS_LINUX, IS_PYPY
 
 
 class SocketCANTest(unittest.TestCase):
     def setUp(self):
         self._ctypes_sizeof = ctypes.sizeof
         self._ctypes_alignment = ctypes.alignment
 
@@ -349,10 +353,28 @@
         self.assertEqual(0, result.ival1_tv_sec)
         self.assertEqual(0, result.ival1_tv_usec)
         self.assertEqual(0, result.ival2_tv_sec)
         self.assertEqual(0, result.ival2_tv_usec)
         self.assertEqual(can_id, result.can_id)
         self.assertEqual(1, result.nframes)
 
+    @unittest.skipUnless(IS_LINUX and IS_PYPY, "Only test when run on Linux with PyPy")
+    def test_pypy_socketcan_support(self):
+        """Wait for PyPy raw CAN socket support
+
+        This test shall document raw CAN socket support under PyPy. Once this test fails, it is likely that PyPy
+        either implemented raw CAN socket support or at least changed the error that is thrown.
+        https://foss.heptapod.net/pypy/pypy/-/issues/3809
+        https://github.com/hardbyte/python-can/issues/1479
+        """
+        try:
+            can.Bus(interface="socketcan", channel="vcan0", bitrate=500000)
+        except OSError as e:
+            if "unknown address family" not in str(e):
+                warnings.warn(
+                    "Please check if PyPy has implemented raw CAN socket support! "
+                    "See: https://foss.heptapod.net/pypy/pypy/-/issues/3809"
+                )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `python-can-4.1.0a2/test/test_socketcan_loopback.py` & `python-can-4.2.0rc0/test/test_socketcan_loopback.py`

 * *Files identical despite different names*

### Comparing `python-can-4.1.0a2/test/test_systec.py` & `python-can-4.2.0rc0/test/test_systec.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         ucan.UcanGetHardwareInfoEx2 = Mock()
         ucan.UcanSetAcceptanceEx = Mock()
         ucan.UcanDeinitCanEx = Mock()
         ucan.UcanDeinitHardware = Mock()
         ucan.UcanWriteCanMsgEx = Mock()
         ucan.UcanResetCanEx = Mock()
         ucan._UCAN_INITIALIZED = True  # Fake this
-        self.bus = can.Bus(bustype="systec", channel=0, bitrate=125000)
+        self.bus = can.Bus(interface="systec", channel=0, bitrate=125000)
 
     def test_bus_creation(self):
         self.assertIsInstance(self.bus, ucanbus.UcanBus)
         self.assertTrue(ucan.UcanInitHwConnectControlEx.called)
         self.assertTrue(
             ucan.UcanInitHardwareEx.called or ucan.UcanInitHardwareEx2.called
         )
@@ -132,15 +132,15 @@
         msg = can.Message(arbitration_id=0x321, data=[50, 51], is_extended_id=False)
         can_msg = self.bus.recv()
         self.assertEqual(can_msg, msg)
 
     @staticmethod
     def test_bus_defaults():
         ucan.UcanInitCanEx2.reset_mock()
-        bus = can.Bus(bustype="systec", channel=0)
+        bus = can.Bus(interface="systec", channel=0)
         ucan.UcanInitCanEx2.assert_called_once_with(
             bus._ucan._handle,
             0,
             InitCanParam(
                 Mode.MODE_NORMAL,
                 Baudrate.BAUD_500kBit,
                 OutputControl.OCR_DEFAULT,
@@ -151,15 +151,15 @@
                 DEFAULT_BUFFER_ENTRIES,
             ),
         )
 
     @staticmethod
     def test_bus_channel():
         ucan.UcanInitCanEx2.reset_mock()
-        bus = can.Bus(bustype="systec", channel=1)
+        bus = can.Bus(interface="systec", channel=1)
         ucan.UcanInitCanEx2.assert_called_once_with(
             bus._ucan._handle,
             1,
             InitCanParam(
                 Mode.MODE_NORMAL,
                 Baudrate.BAUD_500kBit,
                 OutputControl.OCR_DEFAULT,
@@ -170,15 +170,15 @@
                 DEFAULT_BUFFER_ENTRIES,
             ),
         )
 
     @staticmethod
     def test_bus_bitrate():
         ucan.UcanInitCanEx2.reset_mock()
-        bus = can.Bus(bustype="systec", channel=0, bitrate=125000)
+        bus = can.Bus(interface="systec", channel=0, bitrate=125000)
         ucan.UcanInitCanEx2.assert_called_once_with(
             bus._ucan._handle,
             0,
             InitCanParam(
                 Mode.MODE_NORMAL,
                 Baudrate.BAUD_125kBit,
                 OutputControl.OCR_DEFAULT,
@@ -188,20 +188,20 @@
                 DEFAULT_BUFFER_ENTRIES,
                 DEFAULT_BUFFER_ENTRIES,
             ),
         )
 
     def test_bus_custom_bitrate(self):
         with self.assertRaises(ValueError):
-            can.Bus(bustype="systec", channel=0, bitrate=123456)
+            can.Bus(interface="systec", channel=0, bitrate=123456)
 
     @staticmethod
     def test_receive_own_messages():
         ucan.UcanInitCanEx2.reset_mock()
-        bus = can.Bus(bustype="systec", channel=0, receive_own_messages=True)
+        bus = can.Bus(interface="systec", channel=0, receive_own_messages=True)
         ucan.UcanInitCanEx2.assert_called_once_with(
             bus._ucan._handle,
             0,
             InitCanParam(
                 Mode.MODE_TX_ECHO,
                 Baudrate.BAUD_500kBit,
                 OutputControl.OCR_DEFAULT,
@@ -212,15 +212,15 @@
                 DEFAULT_BUFFER_ENTRIES,
             ),
         )
 
     @staticmethod
     def test_bus_passive_state():
         ucan.UcanInitCanEx2.reset_mock()
-        bus = can.Bus(bustype="systec", channel=0, state=can.BusState.PASSIVE)
+        bus = can.Bus(interface="systec", channel=0, state=can.BusState.PASSIVE)
         ucan.UcanInitCanEx2.assert_called_once_with(
             bus._ucan._handle,
             0,
             InitCanParam(
                 Mode.MODE_LISTEN_ONLY,
                 Baudrate.BAUD_500kBit,
                 OutputControl.OCR_DEFAULT,
@@ -231,15 +231,15 @@
                 DEFAULT_BUFFER_ENTRIES,
             ),
         )
 
     @staticmethod
     def test_rx_buffer_entries():
         ucan.UcanInitCanEx2.reset_mock()
-        bus = can.Bus(bustype="systec", channel=0, rx_buffer_entries=1024)
+        bus = can.Bus(interface="systec", channel=0, rx_buffer_entries=1024)
         ucan.UcanInitCanEx2.assert_called_once_with(
             bus._ucan._handle,
             0,
             InitCanParam(
                 Mode.MODE_NORMAL,
                 Baudrate.BAUD_500kBit,
                 OutputControl.OCR_DEFAULT,
@@ -250,15 +250,15 @@
                 DEFAULT_BUFFER_ENTRIES,
             ),
         )
 
     @staticmethod
     def test_tx_buffer_entries():
         ucan.UcanInitCanEx2.reset_mock()
-        bus = can.Bus(bustype="systec", channel=0, tx_buffer_entries=1024)
+        bus = can.Bus(interface="systec", channel=0, tx_buffer_entries=1024)
         ucan.UcanInitCanEx2.assert_called_once_with(
             bus._ucan._handle,
             0,
             InitCanParam(
                 Mode.MODE_NORMAL,
                 Baudrate.BAUD_500kBit,
                 OutputControl.OCR_DEFAULT,
```

### Comparing `python-can-4.1.0a2/test/test_vector.py` & `python-can-4.2.0rc0/test/test_vector.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 """
 
 import ctypes
 import functools
 import pickle
 import sys
 import time
+from test.config import IS_WINDOWS
 from unittest.mock import Mock
 
 import pytest
 
 import can
 from can.interfaces.vector import (
-    canlib,
-    xldefine,
-    xlclass,
+    VectorBusParams,
+    VectorCanFdParams,
+    VectorCanParams,
+    VectorChannelConfig,
     VectorError,
     VectorInitializationError,
     VectorOperationError,
-    VectorChannelConfig,
+    canlib,
+    xlclass,
+    xldefine,
 )
-from can.interfaces.vector import VectorBusParams, VectorCanParams, VectorCanFdParams
-from test.config import IS_WINDOWS
 
 XLDRIVER_FOUND = canlib.xldriver is not None
 
 
 @pytest.fixture()
 def mock_xldriver() -> None:
     # basic mock for XLDriver
@@ -73,15 +75,15 @@
     # cleanup
     canlib.xldriver = real_xldriver
     canlib.WaitForSingleObject = real_waitforsingleobject
     canlib.HAS_EVENTS = real_has_events
 
 
 def test_bus_creation_mocked(mock_xldriver) -> None:
-    bus = can.Bus(channel=0, bustype="vector", _testing=True)
+    bus = can.Bus(channel=0, interface="vector", _testing=True)
     assert isinstance(bus, canlib.VectorBus)
     can.interfaces.vector.canlib.xldriver.xlOpenDriver.assert_called()
     can.interfaces.vector.canlib.xldriver.xlGetApplConfig.assert_called()
 
     can.interfaces.vector.canlib.xldriver.xlOpenPort.assert_called()
     xlOpenPort_args = can.interfaces.vector.canlib.xldriver.xlOpenPort.call_args[0]
     assert xlOpenPort_args[5] == xldefine.XL_InterfaceVersion.XL_INTERFACE_VERSION.value
@@ -89,15 +91,15 @@
 
     can.interfaces.vector.canlib.xldriver.xlCanFdSetConfiguration.assert_not_called()
     can.interfaces.vector.canlib.xldriver.xlCanSetChannelBitrate.assert_not_called()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_bus_creation() -> None:
-    bus = can.Bus(channel=0, serial=_find_virtual_can_serial(), bustype="vector")
+    bus = can.Bus(channel=0, serial=_find_virtual_can_serial(), interface="vector")
     assert isinstance(bus, canlib.VectorBus)
     bus.shutdown()
 
     xl_channel_config = _find_xl_channel_config(
         serial=_find_virtual_can_serial(), channel=0
     )
     assert bus.channel_masks[0] == xl_channel_config.channelMask
@@ -108,15 +110,15 @@
 
     bus = canlib.VectorBus(channel=0, serial=_find_virtual_can_serial())
     assert isinstance(bus, canlib.VectorBus)
     bus.shutdown()
 
 
 def test_bus_creation_bitrate_mocked(mock_xldriver) -> None:
-    bus = can.Bus(channel=0, bustype="vector", bitrate=200_000, _testing=True)
+    bus = can.Bus(channel=0, interface="vector", bitrate=200_000, _testing=True)
     assert isinstance(bus, canlib.VectorBus)
     can.interfaces.vector.canlib.xldriver.xlOpenDriver.assert_called()
     can.interfaces.vector.canlib.xldriver.xlGetApplConfig.assert_called()
 
     can.interfaces.vector.canlib.xldriver.xlOpenPort.assert_called()
     xlOpenPort_args = can.interfaces.vector.canlib.xldriver.xlOpenPort.call_args[0]
     assert xlOpenPort_args[5] == xldefine.XL_InterfaceVersion.XL_INTERFACE_VERSION.value
@@ -129,28 +131,31 @@
     )
     assert xlCanSetChannelBitrate_args[2] == 200_000
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_bus_creation_bitrate() -> None:
     bus = can.Bus(
-        channel=0, serial=_find_virtual_can_serial(), bustype="vector", bitrate=200_000
+        channel=0,
+        serial=_find_virtual_can_serial(),
+        interface="vector",
+        bitrate=200_000,
     )
     assert isinstance(bus, canlib.VectorBus)
 
     xl_channel_config = _find_xl_channel_config(
         serial=_find_virtual_can_serial(), channel=0
     )
     assert xl_channel_config.busParams.data.can.bitRate == 200_000
 
     bus.shutdown()
 
 
 def test_bus_creation_fd_mocked(mock_xldriver) -> None:
-    bus = can.Bus(channel=0, bustype="vector", fd=True, _testing=True)
+    bus = can.Bus(channel=0, interface="vector", fd=True, _testing=True)
     assert isinstance(bus, canlib.VectorBus)
     can.interfaces.vector.canlib.xldriver.xlOpenDriver.assert_called()
     can.interfaces.vector.canlib.xldriver.xlGetApplConfig.assert_called()
 
     can.interfaces.vector.canlib.xldriver.xlOpenPort.assert_called()
     xlOpenPort_args = can.interfaces.vector.canlib.xldriver.xlOpenPort.call_args[0]
     assert (
@@ -161,15 +166,15 @@
     can.interfaces.vector.canlib.xldriver.xlCanFdSetConfiguration.assert_called()
     can.interfaces.vector.canlib.xldriver.xlCanSetChannelBitrate.assert_not_called()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_bus_creation_fd() -> None:
     bus = can.Bus(
-        channel=0, serial=_find_virtual_can_serial(), bustype="vector", fd=True
+        channel=0, serial=_find_virtual_can_serial(), interface="vector", fd=True
     )
     assert isinstance(bus, canlib.VectorBus)
 
     xl_channel_config = _find_xl_channel_config(
         serial=_find_virtual_can_serial(), channel=0
     )
     assert (
@@ -182,24 +187,24 @@
     )
     bus.shutdown()
 
 
 def test_bus_creation_fd_bitrate_timings_mocked(mock_xldriver) -> None:
     bus = can.Bus(
         channel=0,
-        bustype="vector",
+        interface="vector",
         fd=True,
         bitrate=500_000,
         data_bitrate=2_000_000,
-        sjw_abr=10,
-        tseg1_abr=11,
-        tseg2_abr=12,
-        sjw_dbr=13,
-        tseg1_dbr=14,
-        tseg2_dbr=15,
+        sjw_abr=16,
+        tseg1_abr=127,
+        tseg2_abr=32,
+        sjw_dbr=6,
+        tseg1_dbr=27,
+        tseg2_dbr=12,
         _testing=True,
     )
     assert isinstance(bus, canlib.VectorBus)
     can.interfaces.vector.canlib.xldriver.xlOpenDriver.assert_called()
     can.interfaces.vector.canlib.xldriver.xlGetApplConfig.assert_called()
 
     can.interfaces.vector.canlib.xldriver.xlOpenPort.assert_called()
@@ -215,37 +220,213 @@
 
     xlCanFdSetConfiguration_args = (
         can.interfaces.vector.canlib.xldriver.xlCanFdSetConfiguration.call_args[0]
     )
     canFdConf = xlCanFdSetConfiguration_args[2]
     assert canFdConf.arbitrationBitRate == 500000
     assert canFdConf.dataBitRate == 2000000
-    assert canFdConf.sjwAbr == 10
-    assert canFdConf.tseg1Abr == 11
-    assert canFdConf.tseg2Abr == 12
-    assert canFdConf.sjwDbr == 13
-    assert canFdConf.tseg1Dbr == 14
-    assert canFdConf.tseg2Dbr == 15
+    assert canFdConf.sjwAbr == 16
+    assert canFdConf.tseg1Abr == 127
+    assert canFdConf.tseg2Abr == 32
+    assert canFdConf.sjwDbr == 6
+    assert canFdConf.tseg1Dbr == 27
+    assert canFdConf.tseg2Dbr == 12
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_bus_creation_fd_bitrate_timings() -> None:
     bus = can.Bus(
         channel=0,
         serial=_find_virtual_can_serial(),
-        bustype="vector",
+        interface="vector",
         fd=True,
         bitrate=500_000,
         data_bitrate=2_000_000,
-        sjw_abr=10,
-        tseg1_abr=11,
-        tseg2_abr=12,
-        sjw_dbr=13,
-        tseg1_dbr=14,
-        tseg2_dbr=15,
+        sjw_abr=16,
+        tseg1_abr=127,
+        tseg2_abr=32,
+        sjw_dbr=6,
+        tseg1_dbr=27,
+        tseg2_dbr=12,
+    )
+
+    xl_channel_config = _find_xl_channel_config(
+        serial=_find_virtual_can_serial(), channel=0
+    )
+    assert (
+        xl_channel_config.interfaceVersion
+        == xldefine.XL_InterfaceVersion.XL_INTERFACE_VERSION_V4
+    )
+    assert (
+        xl_channel_config.busParams.data.canFD.canOpMode
+        & xldefine.XL_CANFD_BusParams_CanOpMode.XL_BUS_PARAMS_CANOPMODE_CANFD
+    )
+    assert xl_channel_config.busParams.data.canFD.arbitrationBitRate == 500_000
+    assert xl_channel_config.busParams.data.canFD.sjwAbr == 16
+    assert xl_channel_config.busParams.data.canFD.tseg1Abr == 127
+    assert xl_channel_config.busParams.data.canFD.tseg2Abr == 32
+    assert xl_channel_config.busParams.data.canFD.sjwDbr == 6
+    assert xl_channel_config.busParams.data.canFD.tseg1Dbr == 27
+    assert xl_channel_config.busParams.data.canFD.tseg2Dbr == 12
+    assert xl_channel_config.busParams.data.canFD.dataBitRate == 2_000_000
+
+    bus.shutdown()
+
+
+def test_bus_creation_timing_8mhz_mocked(mock_xldriver) -> None:
+    timing = can.BitTiming.from_bitrate_and_segments(
+        f_clock=8_000_000,
+        bitrate=125_000,
+        tseg1=13,
+        tseg2=2,
+        sjw=1,
+    )
+    bus = can.Bus(channel=0, interface="vector", timing=timing, _testing=True)
+    assert isinstance(bus, canlib.VectorBus)
+    can.interfaces.vector.canlib.xldriver.xlOpenDriver.assert_called()
+    can.interfaces.vector.canlib.xldriver.xlGetApplConfig.assert_called()
+
+    can.interfaces.vector.canlib.xldriver.xlOpenPort.assert_called()
+    xlOpenPort_args = can.interfaces.vector.canlib.xldriver.xlOpenPort.call_args[0]
+    assert xlOpenPort_args[5] == xldefine.XL_InterfaceVersion.XL_INTERFACE_VERSION.value
+    assert xlOpenPort_args[6] == xldefine.XL_BusTypes.XL_BUS_TYPE_CAN.value
+
+    can.interfaces.vector.canlib.xldriver.xlCanFdSetConfiguration.assert_not_called()
+    can.interfaces.vector.canlib.xldriver.xlCanSetChannelParamsC200.assert_called()
+    btr0, btr1 = (
+        can.interfaces.vector.canlib.xldriver.xlCanSetChannelParamsC200.call_args[0]
+    )[2:]
+    assert btr0 == timing.btr0
+    assert btr1 == timing.btr1
+
+
+def test_bus_creation_timing_16mhz_mocked(mock_xldriver) -> None:
+    timing = can.BitTiming.from_bitrate_and_segments(
+        f_clock=16_000_000,
+        bitrate=125_000,
+        tseg1=13,
+        tseg2=2,
+        sjw=1,
+    )
+    bus = can.Bus(channel=0, interface="vector", timing=timing, _testing=True)
+    assert isinstance(bus, canlib.VectorBus)
+    can.interfaces.vector.canlib.xldriver.xlOpenDriver.assert_called()
+    can.interfaces.vector.canlib.xldriver.xlGetApplConfig.assert_called()
+
+    can.interfaces.vector.canlib.xldriver.xlOpenPort.assert_called()
+    xlOpenPort_args = can.interfaces.vector.canlib.xldriver.xlOpenPort.call_args[0]
+    assert xlOpenPort_args[5] == xldefine.XL_InterfaceVersion.XL_INTERFACE_VERSION.value
+    assert xlOpenPort_args[6] == xldefine.XL_BusTypes.XL_BUS_TYPE_CAN.value
+
+    can.interfaces.vector.canlib.xldriver.xlCanFdSetConfiguration.assert_not_called()
+    can.interfaces.vector.canlib.xldriver.xlCanSetChannelParams.assert_called()
+    chip_params = (
+        can.interfaces.vector.canlib.xldriver.xlCanSetChannelParams.call_args[0]
+    )[2]
+    assert chip_params.bitRate == 125_000
+    assert chip_params.sjw == 1
+    assert chip_params.tseg1 == 13
+    assert chip_params.tseg2 == 2
+    assert chip_params.sam == 1
+
+
+@pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
+def test_bus_creation_timing() -> None:
+    for f_clock in [8_000_000, 16_000_000]:
+        timing = can.BitTiming.from_bitrate_and_segments(
+            f_clock=f_clock,
+            bitrate=125_000,
+            tseg1=13,
+            tseg2=2,
+            sjw=1,
+        )
+        bus = can.Bus(
+            channel=0,
+            serial=_find_virtual_can_serial(),
+            interface="vector",
+            timing=timing,
+        )
+        assert isinstance(bus, canlib.VectorBus)
+
+        xl_channel_config = _find_xl_channel_config(
+            serial=_find_virtual_can_serial(), channel=0
+        )
+        assert xl_channel_config.busParams.data.can.bitRate == 125_000
+        assert xl_channel_config.busParams.data.can.sjw == 1
+        assert xl_channel_config.busParams.data.can.tseg1 == 13
+        assert xl_channel_config.busParams.data.can.tseg2 == 2
+
+        bus.shutdown()
+
+
+def test_bus_creation_timingfd_mocked(mock_xldriver) -> None:
+    timing = can.BitTimingFd.from_bitrate_and_segments(
+        f_clock=80_000_000,
+        nom_bitrate=500_000,
+        nom_tseg1=68,
+        nom_tseg2=11,
+        nom_sjw=10,
+        data_bitrate=2_000_000,
+        data_tseg1=10,
+        data_tseg2=9,
+        data_sjw=8,
+    )
+    bus = can.Bus(
+        channel=0,
+        interface="vector",
+        timing=timing,
+        _testing=True,
+    )
+    assert isinstance(bus, canlib.VectorBus)
+    can.interfaces.vector.canlib.xldriver.xlOpenDriver.assert_called()
+    can.interfaces.vector.canlib.xldriver.xlGetApplConfig.assert_called()
+
+    can.interfaces.vector.canlib.xldriver.xlOpenPort.assert_called()
+    xlOpenPort_args = can.interfaces.vector.canlib.xldriver.xlOpenPort.call_args[0]
+    assert (
+        xlOpenPort_args[5] == xldefine.XL_InterfaceVersion.XL_INTERFACE_VERSION_V4.value
+    )
+
+    assert xlOpenPort_args[6] == xldefine.XL_BusTypes.XL_BUS_TYPE_CAN.value
+
+    can.interfaces.vector.canlib.xldriver.xlCanFdSetConfiguration.assert_called()
+    can.interfaces.vector.canlib.xldriver.xlCanSetChannelBitrate.assert_not_called()
+
+    xlCanFdSetConfiguration_args = (
+        can.interfaces.vector.canlib.xldriver.xlCanFdSetConfiguration.call_args[0]
+    )
+    canFdConf = xlCanFdSetConfiguration_args[2]
+    assert canFdConf.arbitrationBitRate == 500_000
+    assert canFdConf.dataBitRate == 2_000_000
+    assert canFdConf.sjwAbr == 10
+    assert canFdConf.tseg1Abr == 68
+    assert canFdConf.tseg2Abr == 11
+    assert canFdConf.sjwDbr == 8
+    assert canFdConf.tseg1Dbr == 10
+    assert canFdConf.tseg2Dbr == 9
+
+
+@pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
+def test_bus_creation_timingfd() -> None:
+    timing = can.BitTimingFd.from_bitrate_and_segments(
+        f_clock=80_000_000,
+        nom_bitrate=500_000,
+        nom_tseg1=68,
+        nom_tseg2=11,
+        nom_sjw=10,
+        data_bitrate=2_000_000,
+        data_tseg1=10,
+        data_tseg2=9,
+        data_sjw=8,
+    )
+    bus = can.Bus(
+        channel=0,
+        serial=_find_virtual_can_serial(),
+        interface="vector",
+        timing=timing,
     )
 
     xl_channel_config = _find_xl_channel_config(
         serial=_find_virtual_can_serial(), channel=0
     )
     assert (
         xl_channel_config.interfaceVersion
@@ -253,64 +434,64 @@
     )
     assert (
         xl_channel_config.busParams.data.canFD.canOpMode
         & xldefine.XL_CANFD_BusParams_CanOpMode.XL_BUS_PARAMS_CANOPMODE_CANFD
     )
     assert xl_channel_config.busParams.data.canFD.arbitrationBitRate == 500_000
     assert xl_channel_config.busParams.data.canFD.sjwAbr == 10
-    assert xl_channel_config.busParams.data.canFD.tseg1Abr == 11
-    assert xl_channel_config.busParams.data.canFD.tseg2Abr == 12
-    assert xl_channel_config.busParams.data.canFD.sjwDbr == 13
-    assert xl_channel_config.busParams.data.canFD.tseg1Dbr == 14
-    assert xl_channel_config.busParams.data.canFD.tseg2Dbr == 15
+    assert xl_channel_config.busParams.data.canFD.tseg1Abr == 68
+    assert xl_channel_config.busParams.data.canFD.tseg2Abr == 11
+    assert xl_channel_config.busParams.data.canFD.sjwDbr == 8
+    assert xl_channel_config.busParams.data.canFD.tseg1Dbr == 10
+    assert xl_channel_config.busParams.data.canFD.tseg2Dbr == 9
     assert xl_channel_config.busParams.data.canFD.dataBitRate == 2_000_000
 
     bus.shutdown()
 
 
 def test_send_mocked(mock_xldriver) -> None:
-    bus = can.Bus(channel=0, bustype="vector", _testing=True)
+    bus = can.Bus(channel=0, interface="vector", _testing=True)
     msg = can.Message(
         arbitration_id=0xC0FFEF, data=[1, 2, 3, 4, 5, 6, 7, 8], is_extended_id=True
     )
     bus.send(msg)
     can.interfaces.vector.canlib.xldriver.xlCanTransmit.assert_called()
     can.interfaces.vector.canlib.xldriver.xlCanTransmitEx.assert_not_called()
 
 
 def test_send_fd_mocked(mock_xldriver) -> None:
-    bus = can.Bus(channel=0, bustype="vector", fd=True, _testing=True)
+    bus = can.Bus(channel=0, interface="vector", fd=True, _testing=True)
     msg = can.Message(
         arbitration_id=0xC0FFEF, data=[1, 2, 3, 4, 5, 6, 7, 8], is_extended_id=True
     )
     bus.send(msg)
     can.interfaces.vector.canlib.xldriver.xlCanTransmit.assert_not_called()
     can.interfaces.vector.canlib.xldriver.xlCanTransmitEx.assert_called()
 
 
 def test_receive_mocked(mock_xldriver) -> None:
     can.interfaces.vector.canlib.xldriver.xlReceive = Mock(side_effect=xlReceive)
-    bus = can.Bus(channel=0, bustype="vector", _testing=True)
+    bus = can.Bus(channel=0, interface="vector", _testing=True)
     bus.recv(timeout=0.05)
     can.interfaces.vector.canlib.xldriver.xlReceive.assert_called()
     can.interfaces.vector.canlib.xldriver.xlCanReceive.assert_not_called()
 
 
 def test_receive_fd_mocked(mock_xldriver) -> None:
     can.interfaces.vector.canlib.xldriver.xlCanReceive = Mock(side_effect=xlCanReceive)
-    bus = can.Bus(channel=0, bustype="vector", fd=True, _testing=True)
+    bus = can.Bus(channel=0, interface="vector", fd=True, _testing=True)
     bus.recv(timeout=0.05)
     can.interfaces.vector.canlib.xldriver.xlReceive.assert_not_called()
     can.interfaces.vector.canlib.xldriver.xlCanReceive.assert_called()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_send_and_receive() -> None:
-    bus1 = can.Bus(channel=0, serial=_find_virtual_can_serial(), bustype="vector")
-    bus2 = can.Bus(channel=0, serial=_find_virtual_can_serial(), bustype="vector")
+    bus1 = can.Bus(channel=0, serial=_find_virtual_can_serial(), interface="vector")
+    bus2 = can.Bus(channel=0, serial=_find_virtual_can_serial(), interface="vector")
 
     msg_std = can.Message(
         channel=0, arbitration_id=0xFF, data=list(range(8)), is_extended_id=False
     )
     msg_ext = can.Message(
         channel=0, arbitration_id=0xFFFFFF, data=list(range(8)), is_extended_id=True
     )
@@ -326,18 +507,18 @@
     bus1.shutdown()
     bus2.shutdown()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_send_and_receive_fd() -> None:
     bus1 = can.Bus(
-        channel=0, serial=_find_virtual_can_serial(), fd=True, bustype="vector"
+        channel=0, serial=_find_virtual_can_serial(), fd=True, interface="vector"
     )
     bus2 = can.Bus(
-        channel=0, serial=_find_virtual_can_serial(), fd=True, bustype="vector"
+        channel=0, serial=_find_virtual_can_serial(), fd=True, interface="vector"
     )
 
     msg_std = can.Message(
         channel=0,
         arbitration_id=0xFF,
         data=list(range(64)),
         is_extended_id=False,
@@ -363,106 +544,106 @@
     bus2.shutdown()
 
 
 def test_receive_non_msg_event_mocked(mock_xldriver) -> None:
     can.interfaces.vector.canlib.xldriver.xlReceive = Mock(
         side_effect=xlReceive_chipstate
     )
-    bus = can.Bus(channel=0, bustype="vector", _testing=True)
+    bus = can.Bus(channel=0, interface="vector", _testing=True)
     bus.handle_can_event = Mock()
     bus.recv(timeout=0.05)
     can.interfaces.vector.canlib.xldriver.xlReceive.assert_called()
     can.interfaces.vector.canlib.xldriver.xlCanReceive.assert_not_called()
     bus.handle_can_event.assert_called()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_receive_non_msg_event() -> None:
     bus = canlib.VectorBus(
-        channel=0, serial=_find_virtual_can_serial(), bustype="vector"
+        channel=0, serial=_find_virtual_can_serial(), interface="vector"
     )
     bus.handle_can_event = Mock()
     bus.xldriver.xlCanRequestChipState(bus.port_handle, bus.channel_masks[0])
     bus.recv(timeout=0.5)
     bus.handle_can_event.assert_called()
     bus.shutdown()
 
 
 def test_receive_fd_non_msg_event_mocked(mock_xldriver) -> None:
     can.interfaces.vector.canlib.xldriver.xlCanReceive = Mock(
         side_effect=xlCanReceive_chipstate
     )
-    bus = can.Bus(channel=0, bustype="vector", fd=True, _testing=True)
+    bus = can.Bus(channel=0, interface="vector", fd=True, _testing=True)
     bus.handle_canfd_event = Mock()
     bus.recv(timeout=0.05)
     can.interfaces.vector.canlib.xldriver.xlReceive.assert_not_called()
     can.interfaces.vector.canlib.xldriver.xlCanReceive.assert_called()
     bus.handle_canfd_event.assert_called()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_receive_fd_non_msg_event() -> None:
     bus = canlib.VectorBus(
-        channel=0, serial=_find_virtual_can_serial(), fd=True, bustype="vector"
+        channel=0, serial=_find_virtual_can_serial(), fd=True, interface="vector"
     )
     bus.handle_canfd_event = Mock()
     bus.xldriver.xlCanRequestChipState(bus.port_handle, bus.channel_masks[0])
     bus.recv(timeout=0.5)
     bus.handle_canfd_event.assert_called()
     bus.shutdown()
 
 
 def test_flush_tx_buffer_mocked(mock_xldriver) -> None:
-    bus = can.Bus(channel=0, bustype="vector", _testing=True)
+    bus = can.Bus(channel=0, interface="vector", _testing=True)
     bus.flush_tx_buffer()
     can.interfaces.vector.canlib.xldriver.xlCanFlushTransmitQueue.assert_called()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_flush_tx_buffer() -> None:
-    bus = can.Bus(channel=0, serial=_find_virtual_can_serial(), bustype="vector")
+    bus = can.Bus(channel=0, serial=_find_virtual_can_serial(), interface="vector")
     bus.flush_tx_buffer()
     bus.shutdown()
 
 
 def test_shutdown_mocked(mock_xldriver) -> None:
-    bus = can.Bus(channel=0, bustype="vector", _testing=True)
+    bus = can.Bus(channel=0, interface="vector", _testing=True)
     bus.shutdown()
     can.interfaces.vector.canlib.xldriver.xlDeactivateChannel.assert_called()
     can.interfaces.vector.canlib.xldriver.xlClosePort.assert_called()
     can.interfaces.vector.canlib.xldriver.xlCloseDriver.assert_called()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_shutdown() -> None:
-    bus = can.Bus(channel=0, serial=_find_virtual_can_serial(), bustype="vector")
+    bus = can.Bus(channel=0, serial=_find_virtual_can_serial(), interface="vector")
 
     xl_channel_config = _find_xl_channel_config(
         serial=_find_virtual_can_serial(), channel=0
     )
     assert xl_channel_config.isOnBus != 0
     bus.shutdown()
 
     xl_channel_config = _find_xl_channel_config(
         serial=_find_virtual_can_serial(), channel=0
     )
     assert xl_channel_config.isOnBus == 0
 
 
 def test_reset_mocked(mock_xldriver) -> None:
-    bus = canlib.VectorBus(channel=0, bustype="vector", _testing=True)
+    bus = canlib.VectorBus(channel=0, interface="vector", _testing=True)
     bus.reset()
     can.interfaces.vector.canlib.xldriver.xlDeactivateChannel.assert_called()
     can.interfaces.vector.canlib.xldriver.xlActivateChannel.assert_called()
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
-def test_reset_mocked() -> None:
+def test_reset() -> None:
     bus = canlib.VectorBus(
-        channel=0, serial=_find_virtual_can_serial(), bustype="vector"
+        channel=0, serial=_find_virtual_can_serial(), interface="vector"
     )
     bus.reset()
     bus.shutdown()
 
 
 def test_popup_hw_cfg_mocked(mock_xldriver) -> None:
     canlib.xldriver.xlPopupHwConfig = Mock()
@@ -516,23 +697,23 @@
     assert hw_type == xldefine.XL_HardwareType(xl_channel_config.hwType)
     assert hw_index == xl_channel_config.hwIndex
     assert hw_channel == xl_channel_config.hwChannel
 
 
 def test_set_timer_mocked(mock_xldriver) -> None:
     canlib.xldriver.xlSetTimerRate = Mock()
-    bus = canlib.VectorBus(channel=0, bustype="vector", fd=True, _testing=True)
+    bus = canlib.VectorBus(channel=0, interface="vector", fd=True, _testing=True)
     bus.set_timer_rate(timer_rate_ms=1)
     assert canlib.xldriver.xlSetTimerRate.called
 
 
 @pytest.mark.skipif(not XLDRIVER_FOUND, reason="Vector XL API is unavailable")
 def test_set_timer() -> None:
     bus = canlib.VectorBus(
-        channel=0, serial=_find_virtual_can_serial(), bustype="vector"
+        channel=0, serial=_find_virtual_can_serial(), interface="vector"
     )
     bus.handle_can_event = Mock()
     bus.set_timer_rate(timer_rate_ms=1)
     t0 = time.perf_counter()
     while time.perf_counter() - t0 < 0.5:
         bus.recv(timeout=-1)
 
@@ -542,15 +723,15 @@
 
 
 @pytest.mark.skipif(IS_WINDOWS, reason="Not relevant for Windows.")
 def test_called_without_testing_argument() -> None:
     """This tests if an exception is thrown when we are not running on Windows."""
     with pytest.raises(can.CanInterfaceNotImplementedError):
         # do not set the _testing argument, since it would suppress the exception
-        can.Bus(channel=0, bustype="vector")
+        can.Bus(channel=0, interface="vector")
 
 
 def test_vector_error_pickle() -> None:
     for error_type in [
         VectorError,
         VectorInitializationError,
         VectorOperationError,
@@ -689,15 +870,15 @@
     canlib.xldriver.xlOpenDriver()
     canlib.xldriver.xlGetDriverConfig(xl_driver_config)
     canlib.xldriver.xlCloseDriver()
 
     for i in range(xl_driver_config.channelCount):
         xl_channel_config: xlclass.XLchannelConfig = xl_driver_config.channel[i]
 
-        if xl_channel_config.transceiverName.decode() == "Virtual CAN":
+        if "Virtual CAN" in xl_channel_config.transceiverName.decode():
             return xl_channel_config.serialNumber
 
     raise LookupError("Vector virtual CAN not found")
 
 
 XL_DRIVER_CONFIG_EXAMPLE = (
     b"\x0E\x00\x1E\x14\x0C\x00\x00\x00\x03\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
```

### Comparing `python-can-4.1.0a2/test/test_viewer.py` & `python-can-4.2.0rc0/test/test_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,22 +26,21 @@
 import math
 import os
 import random
 import struct
 import time
 import unittest
 from collections import defaultdict
-from typing import Dict, Tuple, Union
+from test.config import IS_CI
 from unittest.mock import patch
 
 import pytest
 
 import can
 from can.viewer import CanViewer, parse_args
-from test.config import IS_CI
 
 # Allow the curses module to be missing (e.g. on PyPy on Windows)
 try:
     import curses
 
     CURSES_AVAILABLE = True
 except ImportError:
@@ -298,15 +297,15 @@
                 else:
                     # No conversion from SI-units is needed
                     struct_t = value  # type: struct.Struct
                     data = args
 
                 return struct_t.pack(*data)
         else:
-            raise ValueError("Unknown command: 0x{:02X}".format(cmd))
+            raise ValueError(f"Unknown command: 0x{cmd:02X}")
 
     def test_pack_unpack(self):
         CANOPEN_TPDO1 = 0x180
         CANOPEN_TPDO2 = 0x280
         CANOPEN_TPDO3 = 0x380
         CANOPEN_TPDO4 = 0x480
```

