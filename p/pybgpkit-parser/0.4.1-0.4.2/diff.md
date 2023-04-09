# Comparing `tmp/pybgpkit_parser-0.4.1.tar.gz` & `tmp/pybgpkit_parser-0.4.2.tar.gz`

## Comparing `pybgpkit_parser-0.4.1.tar` & `pybgpkit_parser-0.4.2.tar`

### file list

```diff
@@ -1,106 +1,109 @@
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/Cargo.toml
--rw-r--r--   0      501       20       23 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/.gitignore
--rw-r--r--   0      501       20    49749 2022-08-10 17:21:22.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/Cargo.lock
--rw-r--r--   0      501       20     1069 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/LICENSE
--rw-r--r--   0      501       20      624 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/benches/README.md
--rw-r--r--   0      501       20     5024 2023-02-25 16:01:29.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/benches/bench_main.rs
--rw-r--r--   0      501       20     5326 2023-03-09 20:32:42.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/benches/data_source.rs
--rw-r--r--   0      501       20     3428 2023-02-25 16:01:14.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/benches/internals.rs
--rw-r--r--   0      501       20      335 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/count_elems.rs
--rw-r--r--   0      501       20      365 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/display_elems.rs
--rw-r--r--   0      501       20     1054 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/extended_communities.rs
--rw-r--r--   0      501       20     1750 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/filters.rs
--rw-r--r--   0      501       20     1379 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/find_as_set_messages.rs
--rw-r--r--   0      501       20      441 2023-03-26 05:27:50.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/only-to-customer.rs
--rw-r--r--   0      501       20      992 2023-03-09 20:37:57.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/parse-files-from-broker-parallel.rs
--rw-r--r--   0      501       20     1292 2023-03-09 20:38:12.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/parse-files-from-broker.rs
--rw-r--r--   0      501       20      701 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/parse-single-file.rs
--rw-r--r--   0      501       20      594 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/peer_index_table.rs
--rw-r--r--   0      501       20     1354 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/real-time-ris-live-websocket.rs
--rw-r--r--   0      501       20     2792 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/real-time-routeviews-kafka-openbmp.rs
--rw-r--r--   0      501       20     1434 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/records_iter.rs
--rw-r--r--   0      501       20     4537 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/bin/README.md
--rw-r--r--   0      501       20     5291 2023-03-26 07:22:12.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/bin/main.rs
--rw-r--r--   0      501       20     2540 2023-03-12 16:52:38.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/error.rs
--rw-r--r--   0      501       20    13417 2023-03-09 20:50:57.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/lib.rs
--rw-r--r--   0      501       20     1658 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/README.md
--rw-r--r--   0      501       20     1945 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_01_origin.rs
--rw-r--r--   0      501       20     5670 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_02_17_as_path.rs
--rw-r--r--   0      501       20     3190 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_03_next_hop.rs
--rw-r--r--   0      501       20      610 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_04_med.rs
--rw-r--r--   0      501       20      610 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_05_local_pref.rs
--rw-r--r--   0      501       20     2272 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_07_18_aggregator.rs
--rw-r--r--   0      501       20     2431 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_08_communities.rs
--rw-r--r--   0      501       20     1129 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_09_originator.rs
--rw-r--r--   0      501       20     1385 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_10_13_cluster.rs
--rw-r--r--   0      501       20     6301 2023-03-30 03:44:12.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_14_15_nlri.rs
--rw-r--r--   0      501       20    12759 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_16_25_extended_communities.rs
--rw-r--r--   0      501       20     1701 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_32_large_communities.rs
--rw-r--r--   0      501       20     2054 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_35_otc.rs
--rw-r--r--   0      501       20     8500 2023-03-26 06:36:35.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/mod.rs
--rw-r--r--   0      501       20     8906 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/messages.rs
--rw-r--r--   0      501       20      116 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/mod.rs
--rw-r--r--   0      501       20     1198 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/error.rs
--rw-r--r--   0      501       20     5325 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/headers.rs
--rw-r--r--   0      501       20     1275 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/initiation_message.rs
--rw-r--r--   0      501       20     1473 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/mod.rs
--rw-r--r--   0      501       20     2470 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/peer_down_notification.rs
--rw-r--r--   0      501       20     1750 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/peer_up_notification.rs
--rw-r--r--   0      501       20     1835 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/route_mirroring.rs
--rw-r--r--   0      501       20      552 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/route_monitoring.rs
--rw-r--r--   0      501       20     1109 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/stats_report.rs
--rw-r--r--   0      501       20     1278 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/termination_message.rs
--rw-r--r--   0      501       20     5614 2023-03-30 03:44:55.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/mod.rs
--rw-r--r--   0      501       20     5894 2023-03-30 03:44:42.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/openbmp.rs
--rw-r--r--   0      501       20    16961 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/filter.rs
--rw-r--r--   0      501       20     6881 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/iters.rs
--rw-r--r--   0      501       20     4455 2023-03-26 07:28:02.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mod.rs
--rw-r--r--   0      501       20     7621 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/messages/bgp4mp.rs
--rw-r--r--   0      501       20       96 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/messages/mod.rs
--rw-r--r--   0      501       20     4099 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_message.rs
--rw-r--r--   0      501       20     7416 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_v2_message.rs
--rw-r--r--   0      501       20      360 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/mod.rs
--rw-r--r--   0      501       20    14998 2023-03-26 05:27:50.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_elem.rs
--rw-r--r--   0      501       20     5785 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_record.rs
--rw-r--r--   0      501       20     1934 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/error.rs
--rw-r--r--   0      501       20     2412 2023-03-30 03:44:46.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/mod.rs
--rw-r--r--   0      501       20       98 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/pong.rs
--rw-r--r--   0      501       20     4103 2023-03-30 03:45:53.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/raw_bytes.rs
--rw-r--r--   0      501       20      128 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_error.rs
--rw-r--r--   0      501       20     3928 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_message.rs
--rw-r--r--   0      501       20      104 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_rrc_list.rs
--rw-r--r--   0      501       20      191 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_subscribe_ok.rs
--rw-r--r--   0      501       20    10845 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/mod.rs
--rw-r--r--   0      501       20     9873 2023-03-26 07:29:47.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/utils.rs
--rw-r--r--   0      501       20      790 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/tests/bgpkit-parser-tests.rs
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/Cargo.toml
--rw-r--r--   0      501       20       35 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/.gitignore
--rw-r--r--   0      501       20     1069 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/LICENSE
--rw-r--r--   0      501       20     3105 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/README.md
--rw-r--r--   0      501       20    14970 2023-03-26 06:35:49.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/attributes.rs
--rw-r--r--   0      501       20     6822 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/capabilities.rs
--rw-r--r--   0      501       20     9965 2023-03-26 06:13:19.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/community.rs
--rw-r--r--   0      501       20     6380 2023-03-26 05:27:50.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/elem.rs
--rw-r--r--   0      501       20    20404 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/error.rs
--rw-r--r--   0      501       20     3296 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/mod.rs
--rw-r--r--   0      501       20     3335 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/role.rs
--rw-r--r--   0      501       20      635 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/err.rs
--rw-r--r--   0      501       20     3164 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/lib.rs
--rw-r--r--   0      501       20     1780 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/mrt/bgp4mp.rs
--rw-r--r--   0      501       20     5593 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/mrt/mod.rs
--rw-r--r--   0      501       20     7021 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/mrt/tabledump.rs
--rw-r--r--   0      501       20     3742 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/network.rs
--rw-r--r--   0      501       20      109 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/prelude.rs
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.1/Cargo.toml
--rw-r--r--   0      501       20    12288 2023-03-30 05:29:36.000000 pybgpkit_parser-0.4.1/.Dockerfile.swp
--rw-r--r--   0      501       20        5 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/.gitignore
--rw-r--r--   0      501       20      952 2023-03-30 22:59:17.000000 pybgpkit_parser-0.4.1/Dockerfile
--rw-r--r--   0      501       20     1063 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/LICENSE
--rw-r--r--   0      501       20     2182 2023-03-30 05:18:22.000000 pybgpkit_parser-0.4.1/README.md
--rw-r--r--   0      501       20       71 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.1/build.rs
--rw-r--r--   0      501       20   591321 2023-03-30 22:32:13.000000 pybgpkit_parser-0.4.1/new_cache/cache-c728148b-update-example
--rw-r--r--   0      501       20       76 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.1/pyproject.toml
--rw-r--r--   0      501       20     3910 2023-03-30 03:56:50.000000 pybgpkit_parser-0.4.1/src/lib.rs
--rw-r--r--   0      501       20      315 2023-03-30 22:59:17.000000 pybgpkit_parser-0.4.1/test.py
--rw-r--r--   0      501       20    36797 2022-11-03 17:46:36.000000 pybgpkit_parser-0.4.1/Cargo.lock
--rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/Cargo.toml
+-rw-r--r--   0      501       20       23 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/.gitignore
+-rw-r--r--   0      501       20    49749 2022-08-10 17:21:22.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/Cargo.lock
+-rw-r--r--   0      501       20     1069 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/LICENSE
+-rw-r--r--   0      501       20      624 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/README.md
+-rw-r--r--   0      501       20     5024 2023-02-25 16:01:29.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/bench_main.rs
+-rw-r--r--   0      501       20     5326 2023-03-09 20:32:42.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/data_source.rs
+-rw-r--r--   0      501       20     3428 2023-02-25 16:01:14.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/internals.rs
+-rw-r--r--   0      501       20      858 2023-04-09 05:55:46.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/cache_reading.rs
+-rw-r--r--   0      501       20      335 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/count_elems.rs
+-rw-r--r--   0      501       20      365 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/display_elems.rs
+-rw-r--r--   0      501       20     1062 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/extended_communities.rs
+-rw-r--r--   0      501       20     1750 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/filters.rs
+-rw-r--r--   0      501       20     1381 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/find_as_set_messages.rs
+-rw-r--r--   0      501       20      441 2023-03-26 05:27:50.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/only-to-customer.rs
+-rw-r--r--   0      501       20      992 2023-03-09 20:37:57.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-files-from-broker-parallel.rs
+-rw-r--r--   0      501       20     1292 2023-04-03 03:02:57.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-files-from-broker.rs
+-rw-r--r--   0      501       20      701 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-single-file.rs
+-rw-r--r--   0      501       20      594 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/peer_index_table.rs
+-rw-r--r--   0      501       20     1354 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/real-time-ris-live-websocket.rs
+-rw-r--r--   0      501       20     2612 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/real-time-routeviews-kafka-openbmp.rs
+-rw-r--r--   0      501       20     1436 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/records_iter.rs
+-rw-r--r--   0      501       20     4537 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/bin/README.md
+-rw-r--r--   0      501       20     5291 2023-03-26 07:22:12.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/bin/main.rs
+-rw-r--r--   0      501       20     2540 2023-03-12 16:52:38.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/error.rs
+-rw-r--r--   0      501       20    13426 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/lib.rs
+-rw-r--r--   0      501       20     7528 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/aspath.rs
+-rw-r--r--   0      501       20      809 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/atomic_aggregate.rs
+-rw-r--r--   0      501       20     4353 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/mod.rs
+-rw-r--r--   0      501       20     1057 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/nlri.rs
+-rw-r--r--   0      501       20      718 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/attributes/origin.rs
+-rw-r--r--   0      501       20     6822 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/capabilities.rs
+-rw-r--r--   0      501       20     9926 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/community.rs
+-rw-r--r--   0      501       20     6267 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/elem.rs
+-rw-r--r--   0      501       20    20404 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/error.rs
+-rw-r--r--   0      501       20     3208 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/mod.rs
+-rw-r--r--   0      501       20     3338 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/role.rs
+-rw-r--r--   0      501       20      635 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/err.rs
+-rw-r--r--   0      501       20     3179 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mod.rs
+-rw-r--r--   0      501       20     1742 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/bgp4mp.rs
+-rw-r--r--   0      501       20     5569 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/mod.rs
+-rw-r--r--   0      501       20     6963 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/tabledump.rs
+-rw-r--r--   0      501       20      512 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/afi.rs
+-rw-r--r--   0      501       20     1479 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/asn.rs
+-rw-r--r--   0      501       20      152 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/mod.rs
+-rw-r--r--   0      501       20      899 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/nexthop.rs
+-rw-r--r--   0      501       20     1035 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/network/prefix.rs
+-rw-r--r--   0      501       20     1658 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/README.md
+-rw-r--r--   0      501       20     1887 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_01_origin.rs
+-rw-r--r--   0      501       20     5573 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_02_17_as_path.rs
+-rw-r--r--   0      501       20     3095 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_03_next_hop.rs
+-rw-r--r--   0      501       20      508 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_04_med.rs
+-rw-r--r--   0      501       20      508 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_05_local_pref.rs
+-rw-r--r--   0      501       20     2197 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_07_18_aggregator.rs
+-rw-r--r--   0      501       20     1986 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_08_communities.rs
+-rw-r--r--   0      501       20     1117 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_09_originator.rs
+-rw-r--r--   0      501       20     1252 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_10_13_cluster.rs
+-rw-r--r--   0      501       20     6012 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_14_15_nlri.rs
+-rw-r--r--   0      501       20    12414 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_16_25_extended_communities.rs
+-rw-r--r--   0      501       20     1663 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_32_large_communities.rs
+-rw-r--r--   0      501       20     2034 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_35_otc.rs
+-rw-r--r--   0      501       20     8076 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/mod.rs
+-rw-r--r--   0      501       20     8727 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/messages.rs
+-rw-r--r--   0      501       20      116 2023-03-26 06:01:54.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/mod.rs
+-rw-r--r--   0      501       20     1198 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/error.rs
+-rw-r--r--   0      501       20     5207 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/headers.rs
+-rw-r--r--   0      501       20     1189 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/initiation_message.rs
+-rw-r--r--   0      501       20     1473 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/mod.rs
+-rw-r--r--   0      501       20     2419 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/peer_down_notification.rs
+-rw-r--r--   0      501       20     1627 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/peer_up_notification.rs
+-rw-r--r--   0      501       20     1684 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/route_mirroring.rs
+-rw-r--r--   0      501       20      569 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/route_monitoring.rs
+-rw-r--r--   0      501       20     1086 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/stats_report.rs
+-rw-r--r--   0      501       20     1184 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/termination_message.rs
+-rw-r--r--   0      501       20     5380 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/mod.rs
+-rw-r--r--   0      501       20     5766 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/openbmp.rs
+-rw-r--r--   0      501       20    16954 2023-04-09 04:44:23.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/filter.rs
+-rw-r--r--   0      501       20     6855 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/iters.rs
+-rw-r--r--   0      501       20     5212 2023-04-09 05:55:46.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mod.rs
+-rw-r--r--   0      501       20     7368 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/bgp4mp.rs
+-rw-r--r--   0      501       20       96 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/mod.rs
+-rw-r--r--   0      501       20     3808 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_message.rs
+-rw-r--r--   0      501       20     6910 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_v2_message.rs
+-rw-r--r--   0      501       20      360 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/mod.rs
+-rw-r--r--   0      501       20    14992 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_elem.rs
+-rw-r--r--   0      501       20     6843 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_record.rs
+-rw-r--r--   0      501       20     1934 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/error.rs
+-rw-r--r--   0      501       20     2412 2023-03-30 03:44:46.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/mod.rs
+-rw-r--r--   0      501       20       98 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/pong.rs
+-rw-r--r--   0      501       20     4109 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/raw_bytes.rs
+-rw-r--r--   0      501       20      128 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_error.rs
+-rw-r--r--   0      501       20     3916 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_message.rs
+-rw-r--r--   0      501       20      104 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_rrc_list.rs
+-rw-r--r--   0      501       20      191 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_subscribe_ok.rs
+-rw-r--r--   0      501       20    10786 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/mod.rs
+-rw-r--r--   0      501       20    10214 2023-04-09 05:37:47.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/utils.rs
+-rw-r--r--   0      501       20      792 2023-04-03 23:29:41.000000 pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/tests/bgpkit-parser-tests.rs
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.2/Cargo.toml
+-rw-r--r--   0      501       20        5 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/.gitignore
+-rw-r--r--   0      501       20      952 2023-03-30 22:59:17.000000 pybgpkit_parser-0.4.2/Dockerfile
+-rw-r--r--   0      501       20     1063 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/LICENSE
+-rw-r--r--   0      501       20     2182 2023-03-30 05:18:22.000000 pybgpkit_parser-0.4.2/README.md
+-rw-r--r--   0      501       20       71 2023-02-23 23:21:15.000000 pybgpkit_parser-0.4.2/build.rs
+-rw-r--r--   0      501       20       76 2023-02-22 04:21:43.000000 pybgpkit_parser-0.4.2/pyproject.toml
+-rw-r--r--   0      501       20     3940 2023-04-03 23:29:39.000000 pybgpkit_parser-0.4.2/src/lib.rs
+-rw-r--r--   0      501       20      297 2023-04-09 06:00:05.000000 pybgpkit_parser-0.4.2/test-cache.py
+-rw-r--r--   0      501       20      315 2023-03-30 22:59:17.000000 pybgpkit_parser-0.4.2/test.py
+-rw-r--r--   0      501       20    36797 2022-11-03 17:46:36.000000 pybgpkit_parser-0.4.2/Cargo.lock
+-rw-r--r--   0        0        0     2572 1970-01-01 00:00:00.000000 pybgpkit_parser-0.4.2/PKG-INFO
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/Cargo.toml` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,62 +7,53 @@
 repository = "https://github.com/bgpkit/bgpkit-parser"
 documentation = "https://docs.rs/bgpkit-parser"
 description = """
 A library to parse MRT/BGP/BMP binary data.
 """
 keywords = ["bgp", "bgpkit", "mrt"]
 
+[[bin]]
+name = "bgpkit-parser"
+path = "src/bin/main.rs"
+required-features = ["build-binary"]
+
 [dependencies]
 ipnet = "2.7"
 enum-primitive-derive = "0.2"
 num-traits = "0.2"
-chrono = "0.4"
 regex = "1"
-byteorder = "1"
-
-bgp-models = {path= "../bgp-models", version="0.9.1"}
-
-# logging
 log="0.4"
 itertools = "0.10.1"
-
-# ris-live parsing
 serde={version="1.0.130", features=["derive"]}
-serde_json = "1.0.69"
-
-# bmp/openbmp parsing
-hex="0.4.3"
-
+serde_json = "1.0.69" # RIS Live parsing
+hex="0.4.3" # bmp/openbmp parsing
 oneio = {version= "0.8.1", features=["lib_only"]}
+bytes = "1.4.0"
 
 env_logger = {version="0.10", optional=true}
 clap = {version= "4.0", features=["derive"], optional=true}
 
+[features]
+default = ["build-binary"]
+build-binary = ["clap", "env_logger"]
+
+[[bench]]
+name = "internals"
+harness = false
+
+[[bench]]
+name = "bench_main"
+harness = false
+
 [dev-dependencies]
 bgpkit-broker = "0.5.1"
 kafka = "0.9.0"
 tungstenite= "0.18.0"
 url = "2.1.0"
 criterion = {version= "0.4.0", features=["html_reports"]}
 rayon = "1.5.1"
 ureq = "2.6.2"
 bzip2 = "0.4"
 flate2 = "1.0.25"
 md5 = "0.7.0"
 which = "4.4.0"
 
-[features]
-default = ["build-binary"]
-build-binary = ["clap", "env_logger"]
-
-[[bench]]
-name = "internals"
-harness = false
-
-[[bench]]
-name = "bench_main"
-harness = false
-
-[[bin]]
-name = "bgpkit-parser"
-path = "src/bin/main.rs"
-required-features = ["build-binary"]
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/Cargo.lock` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/LICENSE` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/benches/README.md` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/README.md`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/benches/bench_main.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/bench_main.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/benches/data_source.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/data_source.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/benches/internals.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/benches/internals.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/extended_communities.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/extended_communities.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+use bgpkit_parser::models::MetaCommunity;
 use bgpkit_parser::BgpkitParser;
-use bgpkit_parser::MetaCommunity;
 
 /// This example shows how to printout BGP messages with extended or large communities;
 fn main() {
     env_logger::Builder::from_env(env_logger::Env::default().default_filter_or("info")).init();
 
     log::info!("downloading updates file");
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/filters.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/filters.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/find_as_set_messages.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/find_as_set_messages.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-use bgp_models::prelude::AsPathSegment;
 use bgpkit_broker::BgpkitBroker;
+use bgpkit_parser::models::AsPathSegment;
 use bgpkit_parser::BgpkitParser;
 use rayon::prelude::*;
 use std::collections::HashSet;
 
 fn main() {
     let items = BgpkitBroker::new()
         .data_type("rib")
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/parse-files-from-broker-parallel.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-files-from-broker-parallel.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/parse-files-from-broker.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-files-from-broker.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/parse-single-file.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/parse-single-file.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/peer_index_table.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/peer_index_table.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/real-time-ris-live-websocket.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/real-time-ris-live-websocket.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/real-time-routeviews-kafka-openbmp.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/real-time-routeviews-kafka-openbmp.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 extern crate core;
 
 use bgpkit_parser::parser::bmp::messages::MessageBody;
 use bgpkit_parser::Elementor;
 pub use bgpkit_parser::{parse_bmp_msg, parse_openbmp_header};
+use bytes::Bytes;
 use kafka::consumer::{Consumer, FetchOffset, GroupOffsetStorage};
 use kafka::error::Error as KafkaError;
 use log::{error, info};
-use std::io::Cursor;
 use std::thread::sleep;
 use std::time::Duration;
 
 fn consume_and_print(group: String, topic: String, brokers: Vec<String>) -> Result<(), KafkaError> {
     let mut con = Consumer::from_hosts(brokers)
         .with_topic(topic)
         .with_group(group)
@@ -26,33 +26,29 @@
             println!("No messages available right now, wait for 5 seconds.");
             sleep(Duration::from_secs(5));
             continue;
         }
 
         for ms in mss.iter() {
             for m in ms.messages() {
-                let bytes = m.value.to_vec();
-                let mut reader = Cursor::new(bytes.as_slice());
-                let header = parse_openbmp_header(&mut reader).unwrap();
-                let bmp_msg = parse_bmp_msg(&mut reader);
+                let mut bytes = Bytes::from(m.value.to_vec());
+                let header = parse_openbmp_header(&mut bytes).unwrap();
+                let bmp_msg = parse_bmp_msg(&mut bytes);
                 match bmp_msg {
                     Ok(msg) => {
                         let per_peer_header = msg.per_peer_header.unwrap();
-                        match msg.message_body {
-                            MessageBody::RouteMonitoring(m) => {
-                                for elem in Elementor::bgp_to_elems(
-                                    m.bgp_message,
-                                    header.timestamp,
-                                    &per_peer_header.peer_ip,
-                                    &per_peer_header.peer_asn.into(),
-                                ) {
-                                    info!("{}", elem);
-                                }
+                        if let MessageBody::RouteMonitoring(m) = msg.message_body {
+                            for elem in Elementor::bgp_to_elems(
+                                m.bgp_message,
+                                header.timestamp,
+                                &per_peer_header.peer_ip,
+                                &per_peer_header.peer_asn.into(),
+                            ) {
+                                info!("{}", elem);
                             }
-                            _ => {}
                         }
                     }
                     Err(_e) => {
                         let hex = hex::encode(bytes);
                         error!("{}", hex);
                         break;
                     }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/examples/records_iter.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/examples/records_iter.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use bgp_models::prelude::*;
+use bgpkit_parser::models::*;
 use bgpkit_parser::BgpkitParser;
 
 /// an very simple example that reads a remote BGP data file and print out the message count.
 fn main() {
     let url = "http://archive.routeviews.org/route-views.amsix/bgpdata/2023.02/UPDATES/updates.20230222.0430.bz2";
     let parser = BgpkitParser::new(url).unwrap();
     for record in parser.into_record_iter() {
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/bin/README.md` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/bin/README.md`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/bin/main.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/bin/main.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/error.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/error.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/lib.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -312,17 +312,18 @@
 #![allow(clippy::needless_range_loop)]
 
 #[macro_use]
 extern crate enum_primitive_derive;
 extern crate core;
 
 pub mod error;
+pub mod models;
 pub mod parser;
 
-pub use bgp_models::prelude::*;
+pub use models::BgpElem;
 pub use parser::bmp::parse_bmp_msg;
 pub use parser::bmp::parse_openbmp_header;
 pub use parser::bmp::parse_openbmp_msg;
 pub use parser::filter::*;
 pub use parser::iters::{ElemIterator, RecordIterator};
 pub use parser::mrt::parse_mrt_record;
 pub use parser::rislive::parse_ris_live_message;
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/README.md` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/README.md`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_01_origin.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_01_origin.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::{AttributeValue, Origin};
+use bytes::Bytes;
 use num_traits::FromPrimitive;
-use std::io::Cursor;
 
-pub fn parse_origin(input: &mut Cursor<&[u8]>) -> Result<AttributeValue, ParserError> {
-    let origin = input.read_8b()?;
-    match Origin::from_u8(origin) {
+pub fn parse_origin(mut input: Bytes) -> Result<AttributeValue, ParserError> {
+    match Origin::from_u8(input.read_u8()?) {
         Some(v) => Ok(AttributeValue::Origin(v)),
         None => Err(ParserError::UnknownAttr(
             "Failed to parse attribute type: origin".to_string(),
         )),
     }
 }
 
@@ -37,23 +36,23 @@
     ///
     /// Usage of this attribute is defined in 5.1.1.
     /// ```
     #[test]
     fn test_parse_origin() {
         assert_eq!(
             AttributeValue::Origin(Origin::IGP),
-            parse_origin(&mut Cursor::new(&[0u8])).unwrap()
+            parse_origin(Bytes::from_static(&[0u8])).unwrap()
         );
         assert_eq!(
             AttributeValue::Origin(Origin::EGP),
-            parse_origin(&mut Cursor::new(&[1u8])).unwrap()
+            parse_origin(Bytes::from_static(&[1u8])).unwrap()
         );
         assert_eq!(
             AttributeValue::Origin(Origin::INCOMPLETE),
-            parse_origin(&mut Cursor::new(&[2u8])).unwrap()
+            parse_origin(Bytes::from_static(&[2u8])).unwrap()
         );
         assert!(matches!(
-            parse_origin(&mut Cursor::new(&[3u8])).unwrap_err(),
+            parse_origin(Bytes::from_static(&[3u8])).unwrap_err(),
             ParserError::UnknownAttr(_)
         ));
     }
 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_02_17_as_path.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_02_17_as_path.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,37 @@
+use crate::models::attributes::AttributeValue;
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::*;
-use std::io::Cursor;
+use bytes::{Buf, Bytes};
 
 const AS_PATH_AS_SET: u8 = 1;
 const AS_PATH_AS_SEQUENCE: u8 = 2;
 // https://datatracker.ietf.org/doc/html/rfc5065
 const AS_PATH_CONFED_SEQUENCE: u8 = 3;
 const AS_PATH_CONFED_SET: u8 = 4;
 
-pub fn parse_as_path(
-    input: &mut Cursor<&[u8]>,
-    asn_len: &AsnLength,
-    total_bytes: usize,
-) -> Result<AttributeValue, ParserError> {
+pub fn parse_as_path(mut input: Bytes, asn_len: &AsnLength) -> Result<AttributeValue, ParserError> {
     let mut output = AsPath {
         segments: Vec::with_capacity(5),
     };
-    let pos_end = input.position() + total_bytes as u64;
-    while input.position() < pos_end {
-        let segment = parse_as_path_segment(input, asn_len)?;
+    while input.remaining() > 0 {
+        let segment = parse_as_path_segment(&mut input, asn_len)?;
         output.add_segment(segment);
     }
     Ok(AttributeValue::AsPath(output))
 }
 
 fn parse_as_path_segment(
-    input: &mut Cursor<&[u8]>,
+    input: &mut Bytes,
     asn_len: &AsnLength,
 ) -> Result<AsPathSegment, ParserError> {
-    let segment_type = input.read_8b()?;
-    let count = input.read_8b()?;
-    let path = input.read_asns(asn_len, count as usize)?;
+    let segment_type = input.read_u8()?;
+    let count = input.read_u8()? as usize;
+    let path = input.read_asns(asn_len, count)?;
     match segment_type {
         AS_PATH_AS_SET => Ok(AsPathSegment::AsSet(path)),
         AS_PATH_AS_SEQUENCE => Ok(AsPathSegment::AsSequence(path)),
         AS_PATH_CONFED_SEQUENCE => Ok(AsPathSegment::ConfedSequence(path)),
         AS_PATH_CONFED_SET => Ok(AsPathSegment::ConfedSet(path)),
         _ => Err(ParserError::ParseError(format!(
             "Invalid AS path segment type: {}",
@@ -43,15 +39,15 @@
         ))),
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
-    use bgp_models::prelude::AttributeValue::AsPath;
+    use crate::models::AttributeValue::AsPath;
 
     ///
     /// ```text
     /// AS_PATH is a well-known mandatory attribute that is composed
     /// of a sequence of AS path segments.  Each AS path segment is
     /// represented by a triple <path segment type, path segment
     /// length, path segment value>.
@@ -74,101 +70,101 @@
     /// The path segment value field contains one or more AS
     /// numbers, each encoded as a 2-octet length field.
     ///
     /// Usage of this attribute is defined in 5.1.2.
     /// ```
     #[test]
     fn test_parse_as_path() {
-        let data: [u8; 8] = [
+        let data = Bytes::from(vec![
             2, // sequence
             3, // 3 ASes in path
             0, 1, // AS1
             0, 2, // AS2
             0, 3, // AS3
-        ];
-        let res = parse_as_path(&mut Cursor::new(&data), &AsnLength::Bits16, 8).unwrap();
+        ]);
+        let res = parse_as_path(data, &AsnLength::Bits16).unwrap();
 
         assert!(matches!(res, AsPath(_)));
         if let AsPath(path) = res {
             assert_eq!(vec![1, 2, 3], path.to_u32_vec().unwrap())
         } else {
             panic!("cannot parse the path")
         }
     }
 
     #[test]
     fn test_parse_as_path_segment() {
         //////////////////////
         // 16 bits sequence //
         //////////////////////
-        let data: [u8; 8] = [
+        let mut data = Bytes::from(vec![
             2, // sequence
             3, // 3 ASes in path
             0, 1, // AS1
             0, 2, // AS2
             0, 3, // AS3
-        ];
-        let res = parse_as_path_segment(&mut Cursor::new(&data), &AsnLength::Bits16).unwrap();
+        ]);
+        let res = parse_as_path_segment(&mut data, &AsnLength::Bits16).unwrap();
 
         assert!(matches!(res, AsPathSegment::AsSequence(_)));
         if let AsPathSegment::AsSequence(p) = res {
             let asns: Vec<u32> = p.into_iter().map(|a| a.asn).collect();
             assert_eq!(asns, vec![1, 2, 3]);
         } else {
             panic!("not a as sequence")
         }
 
         //////////////////////
         // 16 bits sequence //
         //////////////////////
-        let data: [u8; 14] = [
+        let mut data = Bytes::from(vec![
             2, // sequence
             3, // 3 ASes in path
             0, 0, 0, 1, // AS1
             0, 0, 0, 2, // AS2
             0, 0, 0, 3, // AS3
-        ];
-        let res = parse_as_path_segment(&mut Cursor::new(&data), &AsnLength::Bits32).unwrap();
+        ]);
+        let res = parse_as_path_segment(&mut data, &AsnLength::Bits32).unwrap();
         assert!(matches!(res, AsPathSegment::AsSequence(_)));
         if let AsPathSegment::AsSequence(p) = res {
             let asns: Vec<u32> = p.into_iter().map(|a| a.asn).collect();
             assert_eq!(asns, vec![1, 2, 3]);
         } else {
             panic!("not a as sequence")
         }
 
         /////////////////
         // other types //
         /////////////////
-        let data: [u8; 4] = [
+        let mut data = Bytes::from(vec![
             1, // AS Set
             1, // 1 AS in path
             0, 1,
-        ];
-        let res = parse_as_path_segment(&mut Cursor::new(&data), &AsnLength::Bits16).unwrap();
+        ]);
+        let res = parse_as_path_segment(&mut data, &AsnLength::Bits16).unwrap();
         assert!(matches!(res, AsPathSegment::AsSet(_)));
 
-        let data: [u8; 4] = [
+        let mut data = Bytes::from(vec![
             3, // Confed Sequence
             1, // 1 AS in path
             0, 1,
-        ];
-        let res = parse_as_path_segment(&mut Cursor::new(&data), &AsnLength::Bits16).unwrap();
+        ]);
+        let res = parse_as_path_segment(&mut data, &AsnLength::Bits16).unwrap();
         assert!(matches!(res, AsPathSegment::ConfedSequence(_)));
 
-        let data: [u8; 4] = [
+        let mut data = Bytes::from(vec![
             4, // Confed Set
             1, // 1 AS in path
             0, 1,
-        ];
-        let res = parse_as_path_segment(&mut Cursor::new(&data), &AsnLength::Bits16).unwrap();
+        ]);
+        let res = parse_as_path_segment(&mut data, &AsnLength::Bits16).unwrap();
         assert!(matches!(res, AsPathSegment::ConfedSet(_)));
 
-        let data: [u8; 4] = [
+        let mut data = Bytes::from(vec![
             5, // ERROR
             1, // 1 AS in path
             0, 1,
-        ];
-        let res = parse_as_path_segment(&mut Cursor::new(&data), &AsnLength::Bits16).unwrap_err();
+        ]);
+        let res = parse_as_path_segment(&mut data, &AsnLength::Bits16).unwrap_err();
         assert!(matches!(res, ParserError::ParseError(_)));
     }
 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_03_next_hop.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_03_next_hop.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,24 @@
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::*;
-use std::io::Cursor;
+use bytes::Bytes;
 
-pub fn parse_next_hop(
-    input: &mut Cursor<&[u8]>,
-    afi: &Option<Afi>,
-) -> Result<AttributeValue, ParserError> {
+pub fn parse_next_hop(mut input: Bytes, afi: &Option<Afi>) -> Result<AttributeValue, ParserError> {
     if let Some(afi) = afi {
         Ok(input.read_address(afi).map(AttributeValue::NextHop)?)
     } else {
         Ok(input
             .read_address(&Afi::Ipv4)
             .map(AttributeValue::NextHop)?)
     }
 }
 
-pub fn parse_mp_next_hop(
-    next_hop_length: u8,
-    input: &mut Cursor<&[u8]>,
-) -> Result<Option<NextHopAddress>, ParserError> {
-    let output = match next_hop_length {
+pub fn parse_mp_next_hop(mut input: Bytes) -> Result<Option<NextHopAddress>, ParserError> {
+    let output = match input.len() {
         0 => None,
         4 => Some(input.read_ipv4_address().map(NextHopAddress::Ipv4)?),
         16 => Some(input.read_ipv6_address().map(NextHopAddress::Ipv6)?),
         32 => Some(NextHopAddress::Ipv6LinkLocal(
             input.read_ipv6_address()?,
             input.read_ipv6_address()?,
         )),
@@ -37,70 +31,63 @@
     };
     Ok(output)
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
+    use bytes::BytesMut;
     use std::net::{Ipv4Addr, Ipv6Addr};
     use std::str::FromStr;
 
     #[test]
     fn test_parse_next_hop() {
         let ipv4 = Ipv4Addr::from_str("10.0.0.1").unwrap();
         let ipv6 = Ipv6Addr::from_str("FC00::1").unwrap();
+        let ipv4_bytes = Bytes::from(ipv4.octets().to_vec());
+        let ipv6_bytes = Bytes::from(ipv6.octets().to_vec());
 
-        let res = parse_next_hop(&mut Cursor::new(&ipv4.octets()), &None).unwrap();
+        let res = parse_next_hop(ipv4_bytes, &None).unwrap();
         if let AttributeValue::NextHop(n) = res {
             assert_eq!(n.to_string(), "10.0.0.1".to_string())
         } else {
             panic!();
         }
 
-        let res = parse_next_hop(&mut Cursor::new(&ipv6.octets()), &Some(Afi::Ipv6)).unwrap();
+        let res = parse_next_hop(ipv6_bytes, &Some(Afi::Ipv6)).unwrap();
         if let AttributeValue::NextHop(n) = res {
             assert_eq!(n.to_string().to_ascii_uppercase(), "FC00::1".to_string())
         } else {
             panic!();
         }
     }
 
     #[test]
     fn test_parse_np_next_hop() {
-        let ipv4 = Ipv4Addr::from_str("10.0.0.1").unwrap();
-        let ipv6 = Ipv6Addr::from_str("fc00::1").unwrap();
-        let ipv6_2 = Ipv6Addr::from_str("fc00::2").unwrap();
-
-        assert_eq!(
-            None,
-            parse_mp_next_hop(0, &mut Cursor::new(&ipv4.octets())).unwrap()
-        );
+        let ipv4 = Bytes::from(Ipv4Addr::from_str("10.0.0.1").unwrap().octets().to_vec());
+        let ipv6 = Bytes::from(Ipv6Addr::from_str("fc00::1").unwrap().octets().to_vec());
+        let ipv6_2 = Bytes::from(Ipv6Addr::from_str("fc00::2").unwrap().octets().to_vec());
 
-        if let Some(NextHopAddress::Ipv4(n)) =
-            parse_mp_next_hop(4, &mut Cursor::new(&ipv4.octets())).unwrap()
-        {
+        if let Some(NextHopAddress::Ipv4(n)) = parse_mp_next_hop(ipv4).unwrap() {
             assert_eq!(n.to_string(), "10.0.0.1".to_string())
         } else {
             panic!();
         }
 
-        if let Some(NextHopAddress::Ipv6(n)) =
-            parse_mp_next_hop(16, &mut Cursor::new(&ipv6.octets())).unwrap()
-        {
+        if let Some(NextHopAddress::Ipv6(n)) = parse_mp_next_hop(ipv6.clone()).unwrap() {
             assert_eq!(n.to_string(), "fc00::1".to_string())
         } else {
             panic!();
         }
 
-        let mut bytes = vec![];
-        bytes.extend(ipv6.octets());
-        bytes.extend(ipv6_2.octets());
+        let mut combined = BytesMut::from(ipv6.to_vec().as_slice());
+        combined.extend_from_slice(&ipv6_2.to_vec());
 
         if let Some(NextHopAddress::Ipv6LinkLocal(n, m)) =
-            parse_mp_next_hop(32, &mut Cursor::new(&bytes)).unwrap()
+            parse_mp_next_hop(combined.into()).unwrap()
         {
             assert_eq!(n.to_string(), "fc00::1".to_string());
             assert_eq!(m.to_string(), "fc00::2".to_string());
         } else {
             panic!();
         }
     }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_07_18_aggregator.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_07_18_aggregator.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::*;
-use std::io::Cursor;
+use bytes::Bytes;
 
 pub fn parse_aggregator(
-    input: &mut Cursor<&[u8]>,
+    mut input: Bytes,
     asn_len: &AsnLength,
     afi: &Option<Afi>,
 ) -> Result<AttributeValue, ParserError> {
     let asn = input.read_asn(asn_len)?;
     let afi = match afi {
         None => &Afi::Ipv4,
         Some(a) => a,
@@ -16,67 +16,64 @@
     let addr = input.read_address(afi)?;
     Ok(AttributeValue::Aggregator(asn, addr))
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
-    use bgp_models::prelude::Asn;
     use std::net::{Ipv4Addr, Ipv6Addr};
     use std::str::FromStr;
 
     #[test]
     fn test_parse_aggregator() {
         let ipv4 = Ipv4Addr::from_str("10.0.0.1").unwrap();
-        let mut bytes = vec![];
-        bytes.extend([1u8, 2]);
-        bytes.extend(ipv4.octets());
+        let mut data = vec![];
+        data.extend([1u8, 2]);
+        data.extend(ipv4.octets());
+        let bytes = Bytes::from(data);
 
         if let Ok(AttributeValue::Aggregator(asn, n)) =
-            parse_aggregator(&mut Cursor::new(&bytes), &AsnLength::Bits16, &None)
+            parse_aggregator(bytes.clone(), &AsnLength::Bits16, &None)
         {
             assert_eq!(n, ipv4);
             assert_eq!(
                 asn,
                 Asn {
                     asn: 258,
                     len: AsnLength::Bits16
                 }
             )
         } else {
             panic!()
         }
 
-        if let Ok(AttributeValue::Aggregator(asn, n)) = parse_aggregator(
-            &mut Cursor::new(&bytes),
-            &AsnLength::Bits16,
-            &Some(Afi::Ipv4),
-        ) {
+        if let Ok(AttributeValue::Aggregator(asn, n)) =
+            parse_aggregator(bytes.clone(), &AsnLength::Bits16, &Some(Afi::Ipv4))
+        {
             assert_eq!(n, ipv4);
             assert_eq!(
                 asn,
                 Asn {
                     asn: 258,
                     len: AsnLength::Bits16
                 }
             )
         } else {
             panic!()
         }
 
         let ipv6 = Ipv6Addr::from_str("fc00::1").unwrap();
-        let mut bytes = vec![];
-        bytes.extend([0u8, 0, 1, 2]);
-        bytes.extend(ipv6.octets());
-
-        if let Ok(AttributeValue::Aggregator(asn, n)) = parse_aggregator(
-            &mut Cursor::new(&bytes),
-            &AsnLength::Bits32,
-            &Some(Afi::Ipv6),
-        ) {
+        let mut data = vec![];
+        data.extend([0u8, 0, 1, 2]);
+        data.extend(ipv6.octets());
+        let bytes = Bytes::from(data);
+
+        if let Ok(AttributeValue::Aggregator(asn, n)) =
+            parse_aggregator(bytes, &AsnLength::Bits32, &Some(Afi::Ipv6))
+        {
             assert_eq!(n, ipv6);
             assert_eq!(
                 asn,
                 Asn {
                     asn: 258,
                     len: AsnLength::Bits32
                 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_08_communities.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_08_communities.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,54 @@
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::*;
-use log::debug;
-use std::io::Cursor;
-
-pub fn parse_regular_communities(
-    input: &mut Cursor<&[u8]>,
-    total_bytes: usize,
-) -> Result<AttributeValue, ParserError> {
+use bytes::{Buf, Bytes};
+
+pub fn parse_regular_communities(mut input: Bytes) -> Result<AttributeValue, ParserError> {
     const COMMUNITY_NO_EXPORT: u32 = 0xFFFFFF01;
     const COMMUNITY_NO_ADVERTISE: u32 = 0xFFFFFF02;
     const COMMUNITY_NO_EXPORT_SUBCONFED: u32 = 0xFFFFFF03;
 
-    debug!(
-        "reading communities. cursor_pos: {}/{}; total to read: {}",
-        input.position(),
-        input.get_ref().len(),
-        total_bytes
-    );
-
     let mut communities = vec![];
-    let mut read = 0;
 
-    while read < total_bytes {
-        let community_val = input.read_32b()?;
+    while input.remaining() > 0 {
+        let community_val = input.read_u32()?;
         communities.push(match community_val {
             COMMUNITY_NO_EXPORT => Community::NoExport,
             COMMUNITY_NO_ADVERTISE => Community::NoAdvertise,
             COMMUNITY_NO_EXPORT_SUBCONFED => Community::NoExportSubConfed,
             value => {
                 let asn = Asn {
                     asn: ((value >> 16) & 0xffff),
                     len: AsnLength::Bits16,
                 };
                 let value = (value & 0xffff) as u16;
                 Community::Custom(asn, value)
             }
         });
-        read += 4;
     }
 
-    debug!(
-        "finished reading communities. cursor_pos: {}/{}; {:?}",
-        input.position(),
-        input.get_ref().len(),
-        &communities
-    );
     Ok(AttributeValue::Communities(communities))
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     /// Test parsing of communities values, as defined in RFC1997.
     #[test]
     fn test_parse_communities() {
-        if let Ok(AttributeValue::Communities(communities)) = parse_regular_communities(
-            &mut Cursor::new(&[
+        if let Ok(AttributeValue::Communities(communities)) =
+            parse_regular_communities(Bytes::from(vec![
                 0xFF, 0xFF, 0xFF, 0x01, // NoExport
                 0xFF, 0xFF, 0xFF, 0x02, // NoAdvertise
                 0xFF, 0xFF, 0xFF, 0x03, // NoExportSubConfed
                 0x00, 0x7B, 0x01, 0xC8, // Custom(123, 456)
-            ]),
-            16,
-        ) {
+            ]))
+        {
             assert_eq!(communities.len(), 4);
             assert_eq!(communities[0], Community::NoExport);
             assert_eq!(communities[1], Community::NoAdvertise);
             assert_eq!(communities[2], Community::NoExportSubConfed);
             assert_eq!(communities[3], Community::Custom(Asn::from(123), 456));
         } else {
             panic!("parsing error");
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_09_originator.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_09_originator.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::*;
-use std::io::Cursor;
+use bytes::Bytes;
 
 pub fn parse_originator_id(
-    input: &mut Cursor<&[u8]>,
+    mut input: Bytes,
     afi: &Option<Afi>,
 ) -> Result<AttributeValue, ParserError> {
     let afi = match afi {
         None => &Afi::Ipv4,
         Some(a) => a,
     };
     let addr = input.read_address(afi)?;
@@ -21,24 +21,24 @@
     use std::net::{Ipv4Addr, Ipv6Addr};
     use std::str::FromStr;
 
     #[test]
     fn test_parse_originator_id() {
         let ipv4 = Ipv4Addr::from_str("10.0.0.1").unwrap();
         if let Ok(AttributeValue::OriginatorId(n)) =
-            parse_originator_id(&mut Cursor::new(&ipv4.octets()), &None)
+            parse_originator_id(Bytes::from(ipv4.octets().to_vec()), &None)
         {
             assert_eq!(n, ipv4);
         } else {
             panic!()
         }
 
         let ipv6 = Ipv6Addr::from_str("fc::1").unwrap();
         if let Ok(AttributeValue::OriginatorId(n)) =
-            parse_originator_id(&mut Cursor::new(&ipv6.octets()), &Some(Afi::Ipv6))
+            parse_originator_id(Bytes::from(ipv6.octets().to_vec()), &Some(Afi::Ipv6))
         {
             assert_eq!(n, ipv6);
         } else {
             panic!()
         }
     }
 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_10_13_cluster.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_10_13_cluster.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,16 @@
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::*;
-use std::io::Cursor;
+use bytes::{Buf, Bytes};
 
-pub fn parse_clusters(
-    input: &mut Cursor<&[u8]>,
-    afi: &Option<Afi>,
-    total_bytes: usize,
-) -> Result<AttributeValue, ParserError> {
+pub fn parse_clusters(mut input: Bytes, afi: &Option<Afi>) -> Result<AttributeValue, ParserError> {
     // FIXME: in https://tools.ietf.org/html/rfc4456, the CLUSTER_LIST is a set of CLUSTER_ID each represented by a 4-byte number
     let mut clusters = Vec::new();
-    let initial_pos = input.position();
-    while input.position() - initial_pos < total_bytes as u64 {
+    while input.remaining() > 0 {
         let afi = match afi {
             None => &Afi::Ipv4,
             Some(a) => a,
         };
         let addr = input.read_address(afi)?;
         clusters.push(addr);
     }
@@ -27,20 +22,19 @@
     use super::*;
     use std::net::Ipv4Addr;
     use std::str::FromStr;
 
     #[test]
     fn test_parse_clusters() {
         if let Ok(AttributeValue::Clusters(n)) = parse_clusters(
-            &mut Cursor::new(&[
+            Bytes::from(vec![
                 0xC0, 0x00, 0x02, 0x01, // 192.0.2.1
                 0xC0, 0x00, 0x02, 0x02, // 192.0.2.2
             ]),
             &None,
-            8,
         ) {
             assert_eq!(n.len(), 2);
             assert_eq!(n[0], Ipv4Addr::from_str("192.0.2.1").unwrap());
             assert_eq!(n[1], Ipv4Addr::from_str("192.0.2.2").unwrap());
         } else {
             panic!()
         }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_14_15_nlri.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_14_15_nlri.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+use crate::models::*;
 use crate::parser::bgp::attributes::attr_03_next_hop::parse_mp_next_hop;
 use crate::parser::{parse_nlri_list, ReadUtils};
 use crate::ParserError;
-use bgp_models::prelude::*;
+use bytes::Bytes;
 use log::warn;
-use std::io::Cursor;
 
 ///
 /// <https://datatracker.ietf.org/doc/html/rfc4760#section-3>
 /// The attribute is encoded as shown below:
 /// +---------------------------------------------------------+
 /// | Address Family Identifier (2 octets)                    |
 /// +---------------------------------------------------------+
@@ -18,24 +18,22 @@
 /// | Network Address of Next Hop (variable)                  |
 /// +---------------------------------------------------------+
 /// | Reserved (1 octet)                                      |
 /// +---------------------------------------------------------+
 /// | Network Layer Reachability Information (variable)       |
 /// +---------------------------------------------------------+
 pub fn parse_nlri(
-    input: &mut Cursor<&[u8]>,
+    mut input: Bytes,
     afi: &Option<Afi>,
     safi: &Option<Safi>,
     prefixes: &Option<&[NetworkPrefix]>,
-    reachable: bool,
-    additional_paths: bool,
-    total_bytes: usize,
+    reachable: bool,        // whether the NLRI is announcements or withdrawals
+    additional_paths: bool, // whether the NLRI is part of an additional paths message
 ) -> Result<AttributeValue, ParserError> {
-    let first_byte_zero = input.get_ref()[input.position() as usize] == 0;
-    let pos_end = input.position() + total_bytes as u64;
+    let first_byte_zero = input[0] == 0;
 
     // read address family
     let afi = match afi {
         Some(afi) => {
             if first_byte_zero {
                 input.read_afi()?
             } else {
@@ -53,48 +51,46 @@
             }
         }
         None => input.read_safi()?,
     };
 
     let mut next_hop = None;
     if reachable {
-        let next_hop_length = input.read_8b()?;
-        next_hop = match parse_mp_next_hop(next_hop_length, input) {
+        let next_hop_length = input.read_u8()? as usize;
+        input.has_n_remaining(next_hop_length)?;
+        let next_hop_bytes = input.split_to(next_hop_length);
+        next_hop = match parse_mp_next_hop(next_hop_bytes) {
             Ok(x) => x,
             Err(e) => return Err(e),
         };
     }
 
-    let mut bytes_left = pos_end - input.position();
-
     let prefixes = match prefixes {
         Some(pfxs) => {
             // skip parsing prefixes: https://datatracker.ietf.org/doc/html/rfc6396#section-4.3.4
             if first_byte_zero {
                 if reachable {
                     // skip reserved byte for reachable NRLI
-                    if input.read_8b()? != 0 {
+                    if input.read_u8()? != 0 {
                         warn!("NRLI reserved byte not 0");
                     }
-                    bytes_left -= 1;
                 }
-                parse_nlri_list(input, additional_paths, &afi, bytes_left)?
+                parse_nlri_list(input, additional_paths, &afi)?
             } else {
                 pfxs.to_vec()
             }
         }
         None => {
             if reachable {
                 // skip reserved byte for reachable NRLI
-                if input.read_8b()? != 0 {
+                if input.read_u8()? != 0 {
                     warn!("NRLI reserved byte not 0");
                 }
-                bytes_left -= 1;
             }
-            parse_nlri_list(input, additional_paths, &afi, bytes_left)?
+            parse_nlri_list(input, additional_paths, &afi)?
         }
     };
 
     // Reserved field, should ignore
     match reachable {
         true => Ok(AttributeValue::MpReachNlri(Nlri {
             afi,
@@ -116,33 +112,25 @@
     use super::*;
     use ipnet::IpNet;
     use std::net::Ipv4Addr;
     use std::str::FromStr;
 
     #[test]
     fn test_parsing_nlri_simple() {
-        let test_bytes = vec![
+        let test_bytes = Bytes::from(vec![
             0x00, 0x01, // address family: IPv4
             0x01, // safi: unicast
             0x04, // next hop length: 4
             0xC0, 0x00, 0x02, 0x01, // next hop: 192.0.2.1
             0x00, // reserved
             // NLRI
             0x18, // 24 bits prefix length
             0xC0, 0x00, 0x02, // 192.0.2
-        ];
-        let res = parse_nlri(
-            &mut Cursor::new(&test_bytes),
-            &None,
-            &None,
-            &None,
-            true,
-            false,
-            test_bytes.len(),
-        );
+        ]);
+        let res = parse_nlri(test_bytes, &None, &None, &None, true, false);
 
         if let Ok(AttributeValue::MpReachNlri(nlri)) = res {
             assert_eq!(nlri.afi, Afi::Ipv4);
             assert_eq!(nlri.safi, Safi::Unicast);
             assert_eq!(
                 nlri.next_hop,
                 Some(NextHopAddress::Ipv4(
@@ -156,34 +144,26 @@
         } else {
             panic!("Unexpected result: {:?}", res);
         }
     }
 
     #[test]
     fn test_parsing_nlri_add_path() {
-        let test_bytes = vec![
+        let test_bytes = Bytes::from(vec![
             0x00, 0x01, // address family: IPv4
             0x01, // safi: unicast
             0x04, // next hop length: 4
             0xC0, 0x00, 0x02, 0x01, // next hop: 192.0.2.1
             0x00, // reserved
             // NLRI
             0x00, 0x00, 0x00, 0x7B, // path_id: 123
             0x18, // 24 bits prefix length
             0xC0, 0x00, 0x02, // 192.0.2
-        ];
-        let res = parse_nlri(
-            &mut Cursor::new(&test_bytes),
-            &None,
-            &None,
-            &None,
-            true,
-            true,
-            test_bytes.len(),
-        );
+        ]);
+        let res = parse_nlri(test_bytes, &None, &None, &None, true, true);
 
         if let Ok(AttributeValue::MpReachNlri(nlri)) = res {
             assert_eq!(nlri.afi, Afi::Ipv4);
             assert_eq!(nlri.safi, Safi::Unicast);
             assert_eq!(
                 nlri.next_hop,
                 Some(NextHopAddress::Ipv4(
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_16_25_extended_communities.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_16_25_extended_communities.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,181 +1,174 @@
 //! BGP Extended Communities Attribute
 //!
 //! RFC4360: <https://datatracker.ietf.org/doc/html/rfc4360#section-4.5>
 //! IANA Codes: <https://www.iana.org/assignments/bgp-extended-communities/bgp-extended-communities.xhtml>
 
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::*;
 use num_traits::FromPrimitive;
-use std::io::Cursor;
 
+use bytes::{Buf, Bytes};
 use std::net::Ipv4Addr;
 
-pub fn parse_extended_community(
-    input: &mut Cursor<&[u8]>,
-    total_bytes: usize,
-) -> Result<AttributeValue, ParserError> {
+pub fn parse_extended_community(mut input: Bytes) -> Result<AttributeValue, ParserError> {
     let mut communities = Vec::new();
-    let pos_end = input.position() + total_bytes as u64;
-    while input.position() < pos_end {
-        let ec_type_u8 = input.read_8b()?;
+
+    while input.remaining() > 0 {
+        let ec_type_u8 = input.read_u8()?;
         let ec_type: ExtendedCommunityType = match ExtendedCommunityType::from_u8(ec_type_u8) {
             Some(t) => t,
             None => {
                 let mut buffer: [u8; 8] = [0; 8];
                 let mut i = 0;
                 buffer[i] = ec_type_u8;
                 for _b in 0..7 {
                     i += 1;
-                    buffer[i] = input.read_8b()?;
+                    buffer[i] = input.read_u8()?;
                 }
                 let ec = ExtendedCommunity::Raw(buffer);
                 communities.push(ec);
                 continue;
             }
         };
         let ec: ExtendedCommunity = match ec_type {
             ExtendedCommunityType::TransitiveTwoOctetAsSpecific => {
-                let sub_type = input.read_8b()?;
-                let global = input.read_16b()?;
+                let sub_type = input.read_u8()?;
+                let global = input.read_u16()?;
                 let mut local: [u8; 4] = [0; 4];
                 for i in 0..4 {
-                    local[i] = input.read_8b()?;
+                    local[i] = input.read_u8()?;
                 }
                 ExtendedCommunity::TransitiveTwoOctetAsSpecific(TwoOctetAsSpecific {
                     ec_type: ec_type_u8,
                     ec_subtype: sub_type,
                     global_administrator: Asn {
                         asn: global as u32,
                         len: AsnLength::Bits16,
                     },
                     local_administrator: local,
                 })
             }
             ExtendedCommunityType::NonTransitiveTwoOctetAsSpecific => {
-                let sub_type = input.read_8b()?;
-                let global = input.read_16b()?;
+                let sub_type = input.read_u8()?;
+                let global = input.read_u16()?;
                 let mut local: [u8; 4] = [0; 4];
                 for i in 0..4 {
-                    local[i] = input.read_8b()?;
+                    local[i] = input.read_u8()?;
                 }
                 ExtendedCommunity::NonTransitiveTwoOctetAsSpecific(TwoOctetAsSpecific {
                     ec_type: ec_type_u8,
                     ec_subtype: sub_type,
                     global_administrator: Asn {
                         asn: global as u32,
                         len: AsnLength::Bits16,
                     },
                     local_administrator: local,
                 })
             }
 
             ExtendedCommunityType::TransitiveIpv4AddressSpecific => {
-                let sub_type = input.read_8b()?;
-                let global = Ipv4Addr::from(input.read_32b()?);
+                let sub_type = input.read_u8()?;
+                let global = Ipv4Addr::from(input.read_u32()?);
                 let mut local: [u8; 2] = [0; 2];
-                local[0] = input.read_8b()?;
-                local[1] = input.read_8b()?;
+                local[0] = input.read_u8()?;
+                local[1] = input.read_u8()?;
                 ExtendedCommunity::TransitiveIpv4AddressSpecific(Ipv4AddressSpecific {
                     ec_type: ec_type_u8,
                     ec_subtype: sub_type,
                     global_administrator: global,
                     local_administrator: local,
                 })
             }
             ExtendedCommunityType::NonTransitiveIpv4AddressSpecific => {
-                let sub_type = input.read_8b()?;
-                let global = Ipv4Addr::from(input.read_32b()?);
+                let sub_type = input.read_u8()?;
+                let global = Ipv4Addr::from(input.read_u32()?);
                 let mut local: [u8; 2] = [0; 2];
-                local[0] = input.read_8b()?;
-                local[1] = input.read_8b()?;
+                local[0] = input.read_u8()?;
+                local[1] = input.read_u8()?;
                 ExtendedCommunity::NonTransitiveIpv4AddressSpecific(Ipv4AddressSpecific {
                     ec_type: ec_type_u8,
                     ec_subtype: sub_type,
                     global_administrator: global,
                     local_administrator: local,
                 })
             }
             ExtendedCommunityType::TransitiveFourOctetAsSpecific => {
-                let sub_type = input.read_8b()?;
-                let global = input.read_32b()?;
+                let sub_type = input.read_u8()?;
+                let global = input.read_u32()?;
                 let mut local: [u8; 2] = [0; 2];
-                local[0] = input.read_8b()?;
-                local[1] = input.read_8b()?;
+                local[0] = input.read_u8()?;
+                local[1] = input.read_u8()?;
                 ExtendedCommunity::TransitiveFourOctetAsSpecific(FourOctetAsSpecific {
                     ec_type: ec_type_u8,
                     ec_subtype: sub_type,
                     global_administrator: Asn {
                         asn: global,
                         len: AsnLength::Bits32,
                     },
                     local_administrator: local,
                 })
             }
             ExtendedCommunityType::NonTransitiveFourOctetAsSpecific => {
-                let sub_type = input.read_8b()?;
-                let global = input.read_32b()?;
+                let sub_type = input.read_u8()?;
+                let global = input.read_u32()?;
                 let mut local: [u8; 2] = [0; 2];
-                local[0] = input.read_8b()?;
-                local[1] = input.read_8b()?;
+                local[0] = input.read_u8()?;
+                local[1] = input.read_u8()?;
                 ExtendedCommunity::NonTransitiveFourOctetAsSpecific(FourOctetAsSpecific {
                     ec_type: ec_type_u8,
                     ec_subtype: sub_type,
                     global_administrator: Asn {
                         asn: global,
                         len: AsnLength::Bits32,
                     },
                     local_administrator: local,
                 })
             }
             ExtendedCommunityType::TransitiveOpaque => {
-                let sub_type = input.read_8b()?;
+                let sub_type = input.read_u8()?;
                 let mut value: [u8; 6] = [0; 6];
                 for i in 0..6 {
-                    value[i] = input.read_8b()?;
+                    value[i] = input.read_u8()?;
                 }
                 ExtendedCommunity::TransitiveOpaque(Opaque {
                     ec_type: ec_type_u8,
                     ec_subtype: sub_type,
                     value,
                 })
             }
             ExtendedCommunityType::NonTransitiveOpaque => {
-                let sub_type = input.read_8b()?;
+                let sub_type = input.read_u8()?;
                 let mut value: [u8; 6] = [0; 6];
                 for i in 0..6 {
-                    value[i] = input.read_8b()?;
+                    value[i] = input.read_u8()?;
                 }
                 ExtendedCommunity::NonTransitiveOpaque(Opaque {
                     ec_type: ec_type_u8,
                     ec_subtype: sub_type,
                     value,
                 })
             }
         };
 
         communities.push(ec);
     }
     Ok(AttributeValue::ExtendedCommunities(communities))
 }
 
-pub fn parse_ipv6_extended_community(
-    input: &mut Cursor<&[u8]>,
-    total_bytes: usize,
-) -> Result<AttributeValue, ParserError> {
+pub fn parse_ipv6_extended_community(mut input: Bytes) -> Result<AttributeValue, ParserError> {
     let mut communities = Vec::new();
-    let pos_end = input.position() + total_bytes as u64;
-    while input.position() < pos_end {
-        let ec_type_u8 = input.read_8b()?;
-        let sub_type = input.read_8b()?;
+    while input.remaining() > 0 {
+        let ec_type_u8 = input.read_u8()?;
+        let sub_type = input.read_u8()?;
         let global = input.read_ipv6_address()?;
         let mut local: [u8; 2] = [0; 2];
-        local[0] = input.read_8b()?;
-        local[1] = input.read_8b()?;
+        local[0] = input.read_u8()?;
+        local[1] = input.read_u8()?;
         let ec = ExtendedCommunity::Ipv6AddressSpecific(Ipv6AddressSpecific {
             ec_type: ec_type_u8,
             ec_subtype: sub_type,
             global_administrator: global,
             local_administrator: local,
         });
         communities.push(ec);
@@ -199,15 +192,15 @@
             0x00, // Transitive Two Octet AS Specific
             0x02, // Route Target
             0x00, 0x01, // AS 1
             0x00, 0x00, 0x00, 0x01, // Local Admin 1
         ];
 
         if let AttributeValue::ExtendedCommunities(communities) =
-            parse_extended_community(&mut Cursor::new(data.as_slice()), data.len()).unwrap()
+            parse_extended_community(Bytes::from(data)).unwrap()
         {
             assert_eq!(communities.len(), 1);
             if let ExtendedCommunity::TransitiveTwoOctetAsSpecific(community) = &communities[0] {
                 assert_eq!(community.ec_type, 0x00);
                 assert_eq!(community.ec_subtype, 0x02);
                 assert_eq!(community.global_administrator.asn, 1);
                 assert_eq!(community.local_administrator, [0x00, 0x00, 0x00, 0x01]);
@@ -225,15 +218,15 @@
             0x01, // Transitive IPv4 Address Specific
             0x02, // Route Target
             0xC0, 0x00, 0x02, 0x01, // ipv4: 192.0.2.1
             0x00, 0x01, // Local Admin 1
         ];
 
         if let AttributeValue::ExtendedCommunities(communities) =
-            parse_extended_community(&mut Cursor::new(data.as_slice()), data.len()).unwrap()
+            parse_extended_community(Bytes::from(data)).unwrap()
         {
             assert_eq!(communities.len(), 1);
             if let ExtendedCommunity::TransitiveIpv4AddressSpecific(community) = &communities[0] {
                 assert_eq!(community.ec_type, 0x01);
                 assert_eq!(community.ec_subtype, 0x02);
                 assert_eq!(community.global_administrator, Ipv4Addr::new(192, 0, 2, 1));
                 assert_eq!(community.local_administrator, [0x00, 0x01]);
@@ -251,15 +244,15 @@
             0x02, // Transitive Four Octet AS Specific
             0x02, // Route Target
             0x00, 0x00, 0x00, 0x01, // AS 1
             0x00, 0x01, // Local Admin 1
         ];
 
         if let AttributeValue::ExtendedCommunities(communities) =
-            parse_extended_community(&mut Cursor::new(data.as_slice()), data.len()).unwrap()
+            parse_extended_community(Bytes::from(data)).unwrap()
         {
             assert_eq!(communities.len(), 1);
             if let ExtendedCommunity::TransitiveFourOctetAsSpecific(community) = &communities[0] {
                 assert_eq!(community.ec_type, 0x02);
                 assert_eq!(community.ec_subtype, 0x02);
                 assert_eq!(community.global_administrator.asn, 1);
                 assert_eq!(community.local_administrator, [0x00, 0x01]);
@@ -276,15 +269,15 @@
         let data: Vec<u8> = vec![
             0x03, // Transitive Opaque
             0x02, // Route Target
             0x00, 0x01, 0x02, 0x03, 0x04, 0x05, // Opaque
         ];
 
         if let AttributeValue::ExtendedCommunities(communities) =
-            parse_extended_community(&mut Cursor::new(data.as_slice()), data.len()).unwrap()
+            parse_extended_community(Bytes::from(data)).unwrap()
         {
             assert_eq!(communities.len(), 1);
             if let ExtendedCommunity::TransitiveOpaque(community) = &communities[0] {
                 assert_eq!(community.ec_type, 0x03);
                 assert_eq!(community.ec_subtype, 0x02);
                 assert_eq!(community.value, [0x00, 0x01, 0x02, 0x03, 0x04, 0x05]);
             } else {
@@ -302,15 +295,15 @@
             0x02, // Route Target
             0x20, 0x01, 0x0D, 0xB8, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
             0x00, 0x01, // ipv6: 2001:db8::1
             0x00, 0x01, // Local Admin 1
         ];
 
         if let AttributeValue::ExtendedCommunities(communities) =
-            parse_ipv6_extended_community(&mut Cursor::new(data.as_slice()), data.len()).unwrap()
+            parse_ipv6_extended_community(Bytes::from(data)).unwrap()
         {
             assert_eq!(communities.len(), 1);
             if let ExtendedCommunity::Ipv6AddressSpecific(community) = &communities[0] {
                 assert_eq!(community.ec_type, 0x40);
                 assert_eq!(community.ec_subtype, 0x02);
                 assert_eq!(
                     community.global_administrator,
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_35_otc.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/attr_35_otc.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+use crate::models::*;
 use crate::parser::ReadUtils;
 use crate::ParserError;
-use bgp_models::prelude::*;
-use std::io::Cursor;
+use bytes::Bytes;
 
 /// parse RFC9234 OnlyToCustomer attribute.
 ///
 /// RFC: https://www.rfc-editor.org/rfc/rfc9234.html#name-bgp-only-to-customer-otc-at
 ///
 /// ```text
 /// The OTC Attribute is an optional transitive Path Attribute of the UPDATE message with Attribute Type Code 35 and a length of 4 octets.
@@ -15,26 +15,26 @@
 /// 2. If a route with the OTC Attribute is received from a Peer (i.e., remote AS with a Peer Role) and the Attribute has a value that is not equal to the remote (i.e., Peer's) AS number, then it is a route leak and MUST be considered ineligible.
 /// 3. If a route is received from a Provider, a Peer, or an RS and the OTC Attribute is not present, then it MUST be added with a value equal to the AS number of the remote AS.
 ///
 /// The following egress procedure applies to the processing of the OTC Attribute on route advertisement:
 /// 1. If a route is to be advertised to a Customer, a Peer, or an RS-Client (when the sender is an RS), and the OTC Attribute is not present, then when advertising the route, an OTC Attribute MUST be added with a value equal to the AS number of the local AS.
 /// 2. If a route already contains the OTC Attribute, it MUST NOT be propagated to Providers, Peers, or RSes.
 /// ```
-pub fn parse_only_to_customer(input: &mut Cursor<&[u8]>) -> Result<AttributeValue, ParserError> {
-    let remote_asn = input.read_32b()?;
+pub fn parse_only_to_customer(mut input: Bytes) -> Result<AttributeValue, ParserError> {
+    let remote_asn = input.read_u32()?;
     Ok(AttributeValue::OnlyToCustomer(remote_asn))
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn test_parse_otc() {
         if let Ok(AttributeValue::OnlyToCustomer(123)) =
-            parse_only_to_customer(&mut Cursor::new(&[0, 0, 0, 123]))
+            parse_only_to_customer(Bytes::from(vec![0, 0, 0, 123]))
         {
         } else {
             panic!("parsing error")
         }
     }
 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/mod.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/attributes/mod.rs`

 * *Files 24% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 mod attr_09_originator;
 mod attr_10_13_cluster;
 mod attr_14_15_nlri;
 mod attr_16_25_extended_communities;
 mod attr_32_large_communities;
 mod attr_35_otc;
 
-use byteorder::{ReadBytesExt, BE};
+use bytes::{Buf, Bytes};
 use log::{debug, warn};
-use std::io::{Cursor, Seek, SeekFrom};
 
-use bgp_models::prelude::*;
+use crate::models::*;
 use num_traits::FromPrimitive;
 
 use crate::error::ParserError;
 use crate::parser::bgp::attributes::attr_01_origin::parse_origin;
 use crate::parser::bgp::attributes::attr_02_17_as_path::parse_as_path;
 use crate::parser::bgp::attributes::attr_03_next_hop::parse_next_hop;
 use crate::parser::bgp::attributes::attr_04_med::parse_med;
@@ -50,148 +49,138 @@
 
     /// Parse BGP attributes given a slice of u8 and some options.
     ///
     /// The `data: &[u8]` contains the entirety of the attributes bytes, therefore the size of
     /// the slice is the total byte length of the attributes section of the message.
     pub fn parse_attributes(
         &self,
-        data: &[u8],
+        mut data: Bytes,
         asn_len: &AsnLength,
         afi: Option<Afi>,
         safi: Option<Safi>,
         prefixes: Option<&[NetworkPrefix]>,
     ) -> Result<Vec<Attribute>, ParserError> {
         let mut attributes: Vec<Attribute> = Vec::with_capacity(20);
-        let total_slices_bytes = data.len() as u64;
-        let mut input = Cursor::new(data);
 
-        while input.position() + 3 <= total_slices_bytes {
+        while data.remaining() >= 3 {
             // each attribute is at least 3 bytes: flag(1) + type(1) + length(1)
             // thus the while loop condition is set to be at least 3 bytes to read.
 
             // has content to read
-            let flag = input.read_8b()?;
-            let attr_type = input.read_8b()?;
+            let flag = data.get_u8();
+            let attr_type = data.get_u8();
             let length = match flag & AttributeFlagsBit::ExtendedLengthBit as u8 {
-                0 => input.read_8b()? as usize,
-                _ => input.read_u16::<BE>()? as usize,
+                0 => data.get_u8() as usize,
+                _ => data.get_u16() as usize,
             };
 
             let mut partial = false;
-
             if flag & AttributeFlagsBit::PartialBit as u8 != 0 {
                 /*
                 https://datatracker.ietf.org/doc/html/rfc4271#section-4.3
 
                 > The third high-order bit (bit 2) of the Attribute Flags octet
                 > is the Partial bit.  It defines whether the information
                 > contained in the optional transitive attribute is partial (if
                 > set to 1) or complete (if set to 0).  For well-known attributes
                 > and for optional non-transitive attributes, the Partial bit
                 > MUST be set to 0.
-
                 */
                 partial = true;
             }
 
             debug!(
                 "reading attribute: type -- {:?}, length -- {}",
                 &attr_type, length
             );
             let attr_type = match AttrType::from_u8(attr_type) {
                 Some(t) => t,
                 None => {
                     // input.read_and_drop_n_bytes(length)?;
-                    input.seek(SeekFrom::Current(length as i64))?;
+                    data.has_n_remaining(length)?;
+                    data.advance(length);
                     return match get_deprecated_attr_type(attr_type) {
                         Some(t) => Err(ParserError::DeprecatedAttr(format!(
                             "deprecated attribute type: {} - {}",
                             attr_type, t
                         ))),
                         None => Err(ParserError::UnknownAttr(format!(
                             "unknown attribute type: {}",
                             attr_type
                         ))),
                     };
                 }
             };
 
-            let bytes_left = total_slices_bytes - input.position();
-            let attr_end_pos = input.position() + length as u64;
+            let bytes_left = data.remaining();
 
-            if bytes_left < length as u64 {
+            if data.remaining() < length {
                 warn!(
                     "not enough bytes: input bytes left - {}, want to read - {}; skipping",
                     bytes_left, length
                 );
+                // break and return already parsed attributes
                 break;
             }
 
+            // we know data has enough bytes to read, so we can split the bytes into a new Bytes object
+            let mut attr_data = data.split_to(length);
+
             let attr = match attr_type {
-                AttrType::ORIGIN => parse_origin(&mut input),
-                AttrType::AS_PATH => parse_as_path(&mut input, asn_len, length),
-                AttrType::NEXT_HOP => parse_next_hop(&mut input, &afi),
-                AttrType::MULTI_EXIT_DISCRIMINATOR => parse_med(&mut input),
-                AttrType::LOCAL_PREFERENCE => parse_local_pref(&mut input),
+                AttrType::ORIGIN => parse_origin(attr_data),
+                AttrType::AS_PATH => parse_as_path(attr_data, asn_len),
+                AttrType::NEXT_HOP => parse_next_hop(attr_data, &afi),
+                AttrType::MULTI_EXIT_DISCRIMINATOR => parse_med(attr_data),
+                AttrType::LOCAL_PREFERENCE => parse_local_pref(attr_data),
                 AttrType::ATOMIC_AGGREGATE => {
                     Ok(AttributeValue::AtomicAggregate(AtomicAggregate::AG))
                 }
-                AttrType::AGGREGATOR => parse_aggregator(&mut input, asn_len, &afi),
-                AttrType::ORIGINATOR_ID => parse_originator_id(&mut input, &afi),
-                AttrType::CLUSTER_LIST => parse_clusters(&mut input, &afi, length),
+                AttrType::AGGREGATOR => parse_aggregator(attr_data, asn_len, &afi),
+                AttrType::ORIGINATOR_ID => parse_originator_id(attr_data, &afi),
+                AttrType::CLUSTER_LIST => parse_clusters(attr_data, &afi),
                 AttrType::MP_REACHABLE_NLRI => parse_nlri(
-                    &mut input,
+                    attr_data,
                     &afi,
                     &safi,
                     &prefixes,
                     true,
                     self.additional_paths,
-                    length,
                 ),
                 AttrType::MP_UNREACHABLE_NLRI => parse_nlri(
-                    &mut input,
+                    attr_data,
                     &afi,
                     &safi,
                     &prefixes,
                     false,
                     self.additional_paths,
-                    length,
                 ),
-                AttrType::AS4_PATH => parse_as_path(&mut input, &AsnLength::Bits32, length),
-                AttrType::AS4_AGGREGATOR => parse_aggregator(&mut input, &AsnLength::Bits32, &afi),
+                AttrType::AS4_PATH => parse_as_path(attr_data, &AsnLength::Bits32),
+                AttrType::AS4_AGGREGATOR => parse_aggregator(attr_data, &AsnLength::Bits32, &afi),
 
                 // communities
-                AttrType::COMMUNITIES => parse_regular_communities(&mut input, length),
-                AttrType::LARGE_COMMUNITIES => parse_large_communities(&mut input, length),
-                AttrType::EXTENDED_COMMUNITIES => parse_extended_community(&mut input, length),
+                AttrType::COMMUNITIES => parse_regular_communities(attr_data),
+                AttrType::LARGE_COMMUNITIES => parse_large_communities(attr_data),
+                AttrType::EXTENDED_COMMUNITIES => parse_extended_community(attr_data),
                 AttrType::IPV6_ADDRESS_SPECIFIC_EXTENDED_COMMUNITIES => {
-                    parse_ipv6_extended_community(&mut input, length)
+                    parse_ipv6_extended_community(attr_data)
                 }
                 AttrType::DEVELOPMENT => {
                     let mut value = vec![];
                     for _i in 0..length {
-                        value.push(input.read_8b()?);
+                        value.push(attr_data.get_u8());
                     }
                     Ok(AttributeValue::Development(value))
                 }
-                AttrType::ONLY_TO_CUSTOMER => parse_only_to_customer(&mut input),
+                AttrType::ONLY_TO_CUSTOMER => parse_only_to_customer(attr_data),
                 _ => Err(ParserError::Unsupported(format!(
                     "unsupported attribute type: {:?}",
                     attr_type
                 ))),
             };
 
-            debug!(
-                "seeking position tp {}/{}",
-                attr_end_pos,
-                input.get_ref().len()
-            );
-            // always fast forward to the attribute end position.
-            input.seek(SeekFrom::Start(attr_end_pos))?;
-
             match attr {
                 Ok(value) => {
                     attributes.push(Attribute {
                         value,
                         flag,
                         attr_type,
                     });
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bgp/messages.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bgp/messages.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-use bgp_models::prelude::*;
-use byteorder::{ReadBytesExt, BE};
+use crate::models::*;
+use bytes::{Buf, Bytes};
 use num_traits::FromPrimitive;
-use std::io::{Cursor, Seek, SeekFrom};
 
 use crate::error::ParserError;
 use crate::parser::{parse_nlri_list, AttributeParser, ReadUtils};
 use log::warn;
 
 /// BGP message
 ///
@@ -22,149 +21,156 @@
 /// +                                                               +
 /// |                                                               |
 /// +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 /// |          Length               |      Type     |
 /// +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 /// ```
 pub fn parse_bgp_message(
-    data: &[u8],
+    data: &mut Bytes,
     add_path: bool,
     asn_len: &AsnLength,
 ) -> Result<BgpMessage, ParserError> {
     let total_size = data.len();
-    let mut input = Cursor::new(data);
-    // https://tools.ietf.org/html/rfc4271#section-4
-    // 16 (4 x 4 bytes) octets marker
-    input.read_32b()?;
-    input.read_32b()?;
-    input.read_32b()?;
-    input.read_32b()?;
+    data.has_n_remaining(19)?;
+    data.advance(16);
     /*
     This 2-octet unsigned integer indicates the total length of the
     message, including the header in octets.  Thus, it allows one
     to locate the (Marker field of the) next message in the TCP
     stream.  The value of the Length field MUST always be at least
     19 and no greater than 4096, and MAY be further constrained,
     depending on the message type.  "padding" of extra data after
     the message is not allowed.  Therefore, the Length field MUST
     have the smallest value required, given the rest of the
     message.
     */
-    let length = input.read_u16::<BE>()?;
+    let length = data.get_u16();
     if !(19..=4096).contains(&length) {
         return Err(ParserError::ParseError(format!(
             "invalid BGP message length {}",
             length
         )));
     }
 
     let bgp_msg_length = if (length as usize) > total_size {
-        // return Err(ParserError::TruncatedMsg(format!("Truncated message: {} bytes available, {} bytes to read", total_size, length)))
-        (total_size - 19) as u64
+        total_size - 19
     } else {
-        (length - 19) as u64
+        length as usize - 19
     };
 
-    let msg_type: BgpMessageType = match BgpMessageType::from_u8(input.read_8b()?) {
+    let msg_type: BgpMessageType = match BgpMessageType::from_u8(data.get_u8()) {
         Some(t) => t,
         None => {
             return Err(ParserError::ParseError(
                 "Unknown BGP Message Type".to_string(),
             ))
         }
     };
 
-    // TODO: make sure we don't read over the bound
-    // let mut bgp_msg_input = input.take(bgp_msg_length);
-    Ok(match msg_type {
-        BgpMessageType::OPEN => BgpMessage::Open(parse_bgp_open_message(&mut input)?),
-        BgpMessageType::UPDATE => BgpMessage::Update(parse_bgp_update_message(
-            &mut input,
-            add_path,
-            asn_len,
+    if data.remaining() != bgp_msg_length {
+        warn!(
+            "BGP message length {} does not match the actual length {}",
             bgp_msg_length,
-        )?),
+            data.remaining()
+        );
+    }
+    let mut msg_data = data.split_to(bgp_msg_length);
+
+    Ok(match msg_type {
+        BgpMessageType::OPEN => BgpMessage::Open(parse_bgp_open_message(&mut msg_data)?),
+        BgpMessageType::UPDATE => {
+            BgpMessage::Update(parse_bgp_update_message(msg_data, add_path, asn_len)?)
+        }
         BgpMessageType::NOTIFICATION => {
-            BgpMessage::Notification(parse_bgp_notification_message(&mut input, bgp_msg_length)?)
+            BgpMessage::Notification(parse_bgp_notification_message(msg_data)?)
         }
         BgpMessageType::KEEPALIVE => BgpMessage::KeepAlive(BgpKeepAliveMessage {}),
     })
 }
 
 /// Parse BGP NOTIFICATION messages.
 ///
 /// The BGP NOTIFICATION messages contains BGP error codes received from a connected BGP router. The
 /// error code is parsed into [BgpError] data structure and any unknown codes will produce warning
 /// messages, but not critical errors.
 pub fn parse_bgp_notification_message(
-    input: &mut Cursor<&[u8]>,
-    bgp_msg_length: u64,
+    mut input: Bytes,
 ) -> Result<BgpNotificationMessage, ParserError> {
-    let error_code = input.read_8b()?;
-    let error_subcode = input.read_8b()?;
+    let total_bytes = input.len();
+    let error_code = input.read_u8()?;
+    let error_subcode = input.read_u8()?;
     let error_type = match parse_error_codes(&error_code, &error_subcode) {
         Ok(t) => Some(t),
         Err(e) => {
             warn!("error parsing BGP notification error code: {}", e);
             None
         }
     };
 
-    let data = input.read_n_bytes((bgp_msg_length - 2) as usize)?;
+    let data = input.read_n_bytes(total_bytes - 2)?;
     Ok(BgpNotificationMessage {
         error_code,
         error_subcode,
         error_type,
         data,
     })
 }
 
 /// Parse BGP OPEN messages.
 ///
 /// The parsing of BGP OPEN messages also includes decoding the BGP capabilities.
-pub fn parse_bgp_open_message(input: &mut Cursor<&[u8]>) -> Result<BgpOpenMessage, ParserError> {
-    let version = input.read_8b()?;
+pub fn parse_bgp_open_message(input: &mut Bytes) -> Result<BgpOpenMessage, ParserError> {
+    input.has_n_remaining(10)?;
+    let version = input.get_u8();
     let asn = Asn {
-        asn: input.read_u16::<BE>()? as u32,
+        asn: input.get_u16() as u32,
         len: AsnLength::Bits16,
     };
-    let hold_time = input.read_u16::<BE>()?;
+    let hold_time = input.get_u16();
+
     let sender_ip = input.read_ipv4_address()?;
-    let opt_params_len = input.read_8b()?;
+    let opt_params_len = input.get_u8();
 
-    let pos_end = input.position() + opt_params_len as u64;
+    // let pos_end = input.position() + opt_params_len as u64;
+    if input.remaining() != opt_params_len as usize {
+        warn!(
+            "BGP open message length {} does not match the actual length {}",
+            opt_params_len,
+            input.remaining()
+        );
+    }
 
     let mut extended_length = false;
     let mut first = true;
 
     let mut params: Vec<OptParam> = vec![];
-    while input.position() < pos_end {
-        let param_type = input.read_8b()?;
+    while input.remaining() >= 2 {
+        let param_type = input.get_u8();
         if first {
             // first parameter, check if it is extended length message
             if opt_params_len == 255 && param_type == 255 {
                 extended_length = true;
                 // TODO: handle extended length
                 break;
             } else {
                 first = false;
             }
         }
         // reaching here means all the remain params are regular non-extended-length parameters
 
-        let parm_length = input.read_8b()?;
+        let parm_length = input.get_u8();
         // https://tools.ietf.org/html/rfc3392
         // https://www.iana.org/assignments/bgp-parameters/bgp-parameters.xhtml#bgp-parameters-11
 
         let param_value = match param_type {
             2 => {
                 // capability codes:
                 // https://www.iana.org/assignments/capability-codes/capability-codes.xhtml#capability-codes-2
-                let code = input.read_8b()?;
-                let len = input.read_8b()?;
+                let code = input.read_u8()?;
+                let len = input.read_u8()?;
                 let value = input.read_n_bytes(len as usize)?;
 
                 let capability_type = match parse_capability(&code) {
                     Ok(t) => Some(t),
                     Err(e) => {
                         warn!("error parsing BGP capability code: {}", e.to_string());
                         None
@@ -199,59 +205,59 @@
         extended_length,
         opt_params: params,
     })
 }
 
 /// read nlri portion of a bgp update message.
 fn read_nlri(
-    input: &mut Cursor<&[u8]>,
-    length: usize,
+    mut input: Bytes,
     afi: &Afi,
     add_path: bool,
 ) -> Result<Vec<NetworkPrefix>, ParserError> {
+    let length = input.len();
     if length == 0 {
         return Ok(vec![]);
     }
     if length == 1 {
         // 1 byte does not make sense
         warn!("seeing strange one-byte NLRI field");
-        input.read_8b().unwrap();
+        input.advance(1); // skip the byte
         return Ok(vec![]);
     }
 
-    parse_nlri_list(input, add_path, afi, length as u64)
+    parse_nlri_list(input, add_path, afi)
 }
 
 /// read bgp update message.
+///
+/// RFC: https://tools.ietf.org/html/rfc4271#section-4.3
 pub fn parse_bgp_update_message(
-    input: &mut Cursor<&[u8]>,
+    mut input: Bytes,
     add_path: bool,
     asn_len: &AsnLength,
-    bgp_msg_length: u64,
 ) -> Result<BgpUpdateMessage, ParserError> {
     // AFI for routes out side attributes are IPv4 ONLY.
     let afi = Afi::Ipv4;
 
     // parse withdrawn prefixes nlri
-    let withdrawn_length = input.read_u16::<BE>()? as u64;
-    let withdrawn_prefixes = read_nlri(input, withdrawn_length as usize, &afi, add_path)?;
+    let withdrawn_bytes_length = input.read_u16()? as usize;
+    let withdrawn_bytes = input.split_to(withdrawn_bytes_length);
+    let withdrawn_prefixes = read_nlri(withdrawn_bytes, &afi, add_path)?;
 
     // parse attributes
-    let attribute_length = input.read_u16::<BE>()? as usize;
+    let attribute_length = input.read_u16()? as usize;
     let attr_parser = AttributeParser::new(add_path);
 
-    let pos_start = input.position() as usize;
-    let pos_end = pos_start + attribute_length;
-    let attr_data_slice = &input.get_ref()[pos_start..pos_end];
+    input.has_n_remaining(attribute_length)?;
+    let attr_data_slice = input.split_to(attribute_length);
     let attributes = attr_parser.parse_attributes(attr_data_slice, asn_len, None, None, None)?;
-    input.seek(SeekFrom::Start(pos_end as u64))?;
 
-    // parse announced prefixes nlri
-    let nlri_length = bgp_msg_length - 4 - withdrawn_length - attribute_length as u64;
-    let announced_prefixes = read_nlri(input, nlri_length as usize, &afi, add_path)?;
+    // parse announced prefixes nlri.
+    // the remaining bytes are announced prefixes.
+    let announced_prefixes = read_nlri(input, &afi, add_path)?;
 
     Ok(BgpUpdateMessage {
         withdrawn_prefixes,
         attributes,
         announced_prefixes,
     })
 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/error.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/error.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/headers.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/headers.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+use crate::models::*;
 use crate::parser::bmp::error::ParserBmpError;
 use crate::parser::ReadUtils;
-use bgp_models::prelude::*;
+use bytes::{Buf, Bytes};
 use num_traits::FromPrimitive;
-use std::io::{Cursor, Seek, SeekFrom};
 use std::net::IpAddr;
 
 /// BMP message type enum.
 ///
 /// ```text
 ///    o  Message Type (1 byte): This identifies the type of the BMP
 ///       message.  A BMP implementation MUST ignore unrecognized message
@@ -47,26 +47,24 @@
 #[derive(Debug)]
 pub struct BmpCommonHeader {
     pub version: u8,
     pub msg_len: u32,
     pub msg_type: BmpMsgType,
 }
 
-pub fn parse_bmp_common_header(
-    reader: &mut Cursor<&[u8]>,
-) -> Result<BmpCommonHeader, ParserBmpError> {
-    let version = reader.read_8b()?;
+pub fn parse_bmp_common_header(data: &mut Bytes) -> Result<BmpCommonHeader, ParserBmpError> {
+    let version = data.read_u8()?;
     if version != 3 {
         // has to be 3 per rfc7854
         return Err(ParserBmpError::CorruptedBmpMessage);
     }
 
-    let msg_len = reader.read_32b()?;
+    let msg_len = data.read_u32()?;
 
-    let msg_type = BmpMsgType::from_u8(reader.read_8b()?).unwrap();
+    let msg_type = BmpMsgType::from_u8(data.read_u8()?).unwrap();
     Ok(BmpCommonHeader {
         version,
         msg_len,
         msg_type,
     })
 }
 
@@ -110,54 +108,52 @@
 #[derive(Debug, Primitive)]
 pub enum PeerType {
     GlobalInstancePeer = 0,
     RDInstancePeer = 1,
     LocalInstancePeer = 2,
 }
 
-pub fn parse_per_peer_header(
-    reader: &mut Cursor<&[u8]>,
-) -> Result<BmpPerPeerHeader, ParserBmpError> {
-    let peer_type = PeerType::from_u8(reader.read_8b()?).unwrap();
+pub fn parse_per_peer_header(data: &mut Bytes) -> Result<BmpPerPeerHeader, ParserBmpError> {
+    let peer_type = PeerType::from_u8(data.read_u8()?).unwrap();
 
-    let peer_flags = reader.read_8b()?;
+    let peer_flags = data.read_u8()?;
 
-    let peer_distinguisher = reader.read_64b()?;
+    let peer_distinguisher = data.read_u64()?;
 
     let (is_router_ipv6, is_2byte_asn) = (peer_flags & 0x80 > 0, peer_flags & 0x20 > 0);
 
     let afi = match is_router_ipv6 {
         true => Afi::Ipv6,
         false => Afi::Ipv4,
     };
 
     let asn_len = match is_2byte_asn {
         true => AsnLength::Bits16,
         false => AsnLength::Bits32,
     };
 
     let peer_ip: IpAddr = if is_router_ipv6 {
-        reader.read_ipv6_address()?.into()
+        data.read_ipv6_address()?.into()
     } else {
-        reader.seek(SeekFrom::Current(12))?;
-        let ip = reader.read_ipv4_address()?;
+        data.advance(12);
+        let ip = data.read_ipv4_address()?;
         ip.into()
     };
 
     let peer_asn: u32 = if is_2byte_asn {
-        reader.seek(SeekFrom::Current(2))?;
-        reader.read_16b()? as u32
+        data.advance(2);
+        data.read_u16()? as u32
     } else {
-        reader.read_32b()?
+        data.read_u32()?
     };
 
-    let peer_bgp_id = reader.read_32b()?;
+    let peer_bgp_id = data.read_u32()?;
 
-    let t_sec = reader.read_32b()?;
-    let t_usec = reader.read_32b()?;
+    let t_sec = data.read_u32()?;
+    let t_usec = data.read_u32()?;
     let timestamp = t_sec as f64 + (t_usec as f64) / 1_000_000.0;
 
     Ok(BmpPerPeerHeader {
         peer_type,
         peer_flags,
         peer_distinguisher,
         peer_ip,
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/initiation_message.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/termination_message.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 use crate::parser::bmp::error::ParserBmpError;
 use crate::parser::ReadUtils;
+use bytes::{Buf, Bytes};
 use num_traits::FromPrimitive;
-use std::io::Cursor;
 
 #[derive(Debug)]
-pub struct InitiationMessage {
-    pub tlvs: Vec<InitiationTlv>,
+pub struct TerminationMessage {
+    pub tlvs: Vec<TerminationTlv>,
 }
 
 #[derive(Debug)]
-pub struct InitiationTlv {
-    pub info_type: InitiationTlvType,
+pub struct TerminationTlv {
+    pub info_type: TerminationTlvType,
     pub info_len: u16,
     pub info: String,
 }
 
 ///Type-Length-Value Type
 ///
 /// For more, see: https://datatracker.ietf.org/doc/html/rfc1213
 #[derive(Debug, Primitive)]
-pub enum InitiationTlvType {
+pub enum TerminationTlvType {
     String = 0,
-    SysDescr = 1,
-    SysName = 2,
+    Reason = 1,
 }
 
-pub fn parse_initiation_message(
-    reader: &mut Cursor<&[u8]>,
-) -> Result<InitiationMessage, ParserBmpError> {
+pub fn parse_termination_message(data: &mut Bytes) -> Result<TerminationMessage, ParserBmpError> {
     let mut tlvs = vec![];
-    let total = reader.get_ref().len() as u64;
 
-    while total - reader.position() > 4 {
-        let info_type: InitiationTlvType = InitiationTlvType::from_u16(reader.read_16b()?).unwrap();
-        let info_len = reader.read_16b()?;
-        if total - reader.position() < info_len as u64 {
+    while data.remaining() > 4 {
+        let info_type: TerminationTlvType = TerminationTlvType::from_u16(data.read_u16()?).unwrap();
+        let info_len = data.read_u16()?;
+        if data.remaining() < info_len as usize {
             // not enough bytes to read
             break;
         }
-        let info = reader.read_n_bytes_to_string(info_len as usize)?;
-        tlvs.push(InitiationTlv {
+        let info = data.read_n_bytes_to_string(info_len as usize)?;
+        tlvs.push(TerminationTlv {
             info_type,
             info_len,
             info,
-        });
+        })
     }
 
-    Ok(InitiationMessage { tlvs })
+    Ok(TerminationMessage { tlvs })
 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/mod.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/mod.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/peer_down_notification.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/peer_down_notification.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 use crate::parser::bmp::error::ParserBmpError;
 use crate::parser::ReadUtils;
-use std::io::Cursor;
+use bytes::{Buf, Bytes};
 
 #[derive(Debug)]
 pub struct PeerDownNotification {
     pub reason: u8,
     pub data: Option<Vec<u8>>,
 }
 
 pub fn parse_peer_down_notification(
-    reader: &mut Cursor<&[u8]>,
+    data: &mut Bytes,
 ) -> Result<PeerDownNotification, ParserBmpError> {
-    let reason = reader.read_8b()?;
-    let bytes_left = reader.get_ref().len() - (reader.position() as usize);
+    let reason = data.read_u8()?;
+    let bytes_left = data.remaining();
     let data: Option<Vec<u8>> = match reason {
         1 => {
             /*
             The local system closed the session.  Following the
             Reason is a BGP PDU containing a BGP NOTIFICATION message that
             would have been sent to the peer.
             */
-            Some(reader.read_n_bytes(bytes_left)?)
+            Some(data.read_n_bytes(bytes_left)?)
         }
         2 => {
             /*
             The local system closed the session.  No notification
             message was sent.  Following the reason code is a 2-byte field
             containing the code corresponding to the Finite State Machine
             (FSM) Event that caused the system to close the session (see
             Section 8.1 of [RFC4271]).  Two bytes both set to 0 are used to
             indicate that no relevant Event code is defined.
              */
-            Some(reader.read_n_bytes(bytes_left)?)
+            Some(data.read_n_bytes(bytes_left)?)
         }
         3 => {
             /*
             The remote system closed the session with a notification
             message.  Following the Reason is a BGP PDU containing the BGP
             NOTIFICATION message as received from the peer.
              */
-            Some(reader.read_n_bytes(bytes_left)?)
+            Some(data.read_n_bytes(bytes_left)?)
         }
         4 => {
             /*
             The remote system closed the session without a
             notification message.  This includes any unexpected termination of
             the transport session, so in some cases both the local and remote
             systems might consider this to apply.
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/messages/route_monitoring.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/messages/route_monitoring.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+use crate::models::*;
 use crate::parser::bgp::messages::parse_bgp_message;
 use crate::parser::bmp::error::ParserBmpError;
-use bgp_models::prelude::*;
+use bytes::Bytes;
 
 #[derive(Debug)]
 pub struct RouteMonitoring {
     pub bgp_message: BgpMessage,
 }
 
 pub fn parse_route_monitoring(
-    data: &[u8],
+    data: &mut Bytes,
     asn_len: &AsnLength,
 ) -> Result<RouteMonitoring, ParserBmpError> {
     // let bgp_update = parse_bgp_update_message(reader, false, afi, asn_len, total_len)?;
     let bgp_update = parse_bgp_message(data, false, asn_len)?;
     Ok(RouteMonitoring {
         bgp_message: bgp_update,
     })
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/bmp/mod.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/bmp/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 /*!
 Provides parsing for BMP and OpenBMP binary-formatted messages.
 */
 use crate::parser::bmp::error::ParserBmpError;
 use crate::parser::bmp::messages::*;
 pub use crate::parser::bmp::openbmp::parse_openbmp_header;
-use std::io::Cursor;
+use bytes::Bytes;
 
 pub mod error;
 pub mod messages;
 pub mod openbmp;
 
 /// Parse OpenBMP `raw_bmp` message.
 ///
 /// An OpenBMP `raw_bmp` message contains a [OpenBmpHeader] and a [BmpMessage].
-pub fn parse_openbmp_msg(data: &[u8]) -> Result<BmpMessage, ParserBmpError> {
-    let mut reader = Cursor::new(data);
-    let _header = parse_openbmp_header(&mut reader)?;
-    parse_bmp_msg(&mut reader)
+pub fn parse_openbmp_msg(mut data: Bytes) -> Result<BmpMessage, ParserBmpError> {
+    let _header = parse_openbmp_header(&mut data)?;
+    parse_bmp_msg(&mut data)
 }
 
 /// Parse a BMP message.
-pub fn parse_bmp_msg(reader: &mut Cursor<&[u8]>) -> Result<BmpMessage, ParserBmpError> {
-    let common_header = parse_bmp_common_header(reader)?;
+pub fn parse_bmp_msg(data: &mut Bytes) -> Result<BmpMessage, ParserBmpError> {
+    let common_header = parse_bmp_common_header(data)?;
 
     // let mut buffer ;
     // if total_len>common_header.msg_len {
     //     // truncated message
     //     let diff = total_len - common_header.msg_len;
     //     let bytes_left = reader.get_ref().len() as u32 - reader.position() as u32;
     //     buffer = Vec::with_capacity((bytes_left - diff) as usize);
@@ -34,70 +33,68 @@
     // } else {
     //     return Err(ParserBmpError::CorruptedBmpMessage)
     // };
     // reader.read_exact(&mut buffer)?;
 
     match &common_header.msg_type {
         BmpMsgType::RouteMonitoring => {
-            let per_peer_header = parse_per_peer_header(reader)?;
-            let pos_start = reader.position() as usize;
-            let data_bytes = &reader.get_ref()[pos_start..];
-            let msg = parse_route_monitoring(data_bytes, &per_peer_header.asn_len)?;
+            let per_peer_header = parse_per_peer_header(data)?;
+            let msg = parse_route_monitoring(data, &per_peer_header.asn_len)?;
             Ok(BmpMessage {
                 common_header,
                 per_peer_header: Some(per_peer_header),
                 message_body: MessageBody::RouteMonitoring(msg),
             })
         }
         BmpMsgType::RouteMirroringMessage => {
-            let per_peer_header = parse_per_peer_header(reader)?;
-            let msg = parse_route_mirroring(reader, &per_peer_header.asn_len)?;
+            let per_peer_header = parse_per_peer_header(data)?;
+            let msg = parse_route_mirroring(data, &per_peer_header.asn_len)?;
             Ok(BmpMessage {
                 common_header,
                 per_peer_header: Some(per_peer_header),
                 message_body: MessageBody::RouteMirroring(msg),
             })
         }
         BmpMsgType::StatisticsReport => {
-            let per_peer_header = parse_per_peer_header(reader)?;
-            let msg = parse_stats_report(reader)?;
+            let per_peer_header = parse_per_peer_header(data)?;
+            let msg = parse_stats_report(data)?;
             Ok(BmpMessage {
                 common_header,
                 per_peer_header: Some(per_peer_header),
                 message_body: MessageBody::StatsReport(msg),
             })
         }
         BmpMsgType::PeerDownNotification => {
-            let per_peer_header = parse_per_peer_header(reader)?;
-            let msg = parse_peer_down_notification(reader)?;
+            let per_peer_header = parse_per_peer_header(data)?;
+            let msg = parse_peer_down_notification(data)?;
             Ok(BmpMessage {
                 common_header,
                 per_peer_header: Some(per_peer_header),
                 message_body: MessageBody::PeerDownNotification(msg),
             })
         }
         BmpMsgType::PeerUpNotification => {
-            let per_peer_header = parse_per_peer_header(reader)?;
-            let msg = parse_peer_up_notification(reader, &per_peer_header.afi)?;
+            let per_peer_header = parse_per_peer_header(data)?;
+            let msg = parse_peer_up_notification(data, &per_peer_header.afi)?;
             Ok(BmpMessage {
                 common_header,
                 per_peer_header: Some(per_peer_header),
                 message_body: MessageBody::PeerUpNotification(msg),
             })
         }
         BmpMsgType::InitiationMessage => {
-            let msg = parse_initiation_message(reader)?;
+            let msg = parse_initiation_message(data)?;
             Ok(BmpMessage {
                 common_header,
                 per_peer_header: None,
                 message_body: MessageBody::InitiationMessage(msg),
             })
         }
         BmpMsgType::TerminationMessage => {
-            let msg = parse_termination_message(reader)?;
+            let msg = parse_termination_message(data)?;
             Ok(BmpMessage {
                 common_header,
                 per_peer_header: None,
                 message_body: MessageBody::TerminationMessage(msg),
             })
         }
     }
@@ -109,21 +106,21 @@
     use super::*;
     use crate::parser::bmp::openbmp::parse_openbmp_header;
 
     #[test]
     fn test_peer_down_notification() {
         let input = "4f424d500107006400000033800c6184b9c2000c602cbf4f072f3ae149d23486024bc3dadfc4000a69732d63632d626d7031c677060bdd020a9e92be000200de2e3180df3369000000000000000000000000000c726f7574652d76696577733500000001030000003302000000000000000000000000000000000000000000003fda060e00000da30000000061523c36000c0e1c0200000a";
         let decoded = hex::decode(input).unwrap();
-        let mut reader = Cursor::new(decoded.as_slice());
-        let _header = parse_openbmp_header(&mut reader).unwrap();
-        let _msg = parse_bmp_msg(&mut reader).unwrap();
+        let mut data = Bytes::from(decoded);
+        let _header = parse_openbmp_header(&mut data).unwrap();
+        let _msg = parse_bmp_msg(&mut data).unwrap();
     }
 
     #[test]
     fn test_route_monitoring() {
         let input = "4f424d500107005c000000b0800c618881530002f643fef880938d19e9d632c815d1e95a87e1000a69732d61682d626d7031eb4de4e596b282c6a995b067df4abc8cc342f19200000000000000000000000000046c696e780000000103000000b00000c00000000000000000200107f800040000000000001aae000400001aae5474800e02dddf5d00000000ffffffffffffffffffffffffffffffff00800200000069400101005002001602050000192f00001aae0000232a000328eb00032caec008181aae42681aae44581aae464f1aae59d91aae866543000000900e002c00020120200107f800040000000000001aae0004fe8000000000000082711ffffe7f29f100302a0fca8000010a";
         let decoded = hex::decode(input).unwrap();
-        let mut reader = Cursor::new(decoded.as_slice());
-        let _header = parse_openbmp_header(&mut reader).unwrap();
-        let _msg = parse_bmp_msg(&mut reader).unwrap();
+        let mut data = Bytes::from(decoded);
+        let _header = parse_openbmp_header(&mut data).unwrap();
+        let _msg = parse_bmp_msg(&mut data).unwrap();
     }
 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/filter.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/filter.rs`

 * *Files 0% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 
 ### Note
 
 Currently, only [BgpElem] implements the filtering capability. Support for [MrtRecord] will come in
 later releases.
 
 */
+use crate::models::*;
 use crate::ParserError;
 use crate::ParserError::FilterError;
-use bgp_models::prelude::*;
 use ipnet::IpNet;
 use regex::Regex;
 use std::net::IpAddr;
 use std::str::FromStr;
 
 /// Filter enum: definition o types of filters
 ///
@@ -398,15 +398,15 @@
             .unwrap();
         let count = parser.into_elem_iter().count();
         assert_eq!(count, 3393 + 834);
     }
 
     #[test]
     fn test_prefix_match() {
-        // networks
+        // network
         let p1 = IpNet::from_str("10.1.1.0/24").unwrap();
         let p1_exact = IpNet::from_str("10.1.1.0/24").unwrap();
         let p1_super = IpNet::from_str("10.1.0.0/16").unwrap();
         let p1_sub = IpNet::from_str("10.1.1.0/25").unwrap();
 
         let p2 = IpNet::from_str("2001:0DB8:0000:000b::/64").unwrap();
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/iters.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/iters.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 /*!
 Provides parser iterator implementation.
 */
 use crate::error::ParserError;
+use crate::models::*;
 use crate::parser::BgpkitParser;
-use crate::Filterable;
-use crate::{BgpElem, Elementor};
-use bgp_models::prelude::*;
+use crate::{Elementor, Filterable};
 use log::{error, warn};
 use std::io::Read;
 
 /// Use [BgpElemIterator] as the default iterator to return [BgpElem]s instead of [MrtRecord]s.
 impl<R: Read> IntoIterator for BgpkitParser<R> {
     type Item = BgpElem;
     type IntoIter = ElemIterator<R>;
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mod.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mod.rs`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 pub(crate) use self::utils::*;
 pub(crate) use bgp::attributes::AttributeParser;
 pub(crate) use mrt::{
     parse_bgp4mp, parse_mrt_record, parse_table_dump_message, parse_table_dump_v2_message,
 };
 
 pub use crate::error::{ParserError, ParserErrorWithBytes};
+use crate::models::MrtRecord;
 use crate::Filter;
-use bgp_models::prelude::MrtRecord;
 pub use mrt::mrt_elem::Elementor;
 use oneio::{get_cache_reader, get_reader};
 
 pub struct BgpkitParser<R> {
     reader: R,
     core_dump: bool,
     filters: Vec<Filter>,
@@ -54,25 +54,41 @@
     /// Creating a new parser that also caches the remote content to a local cache directory.
     ///
     /// The cache file name is generated by the following format: `cache-<crc32 of file name>-<file name>`.
     /// For example, the remote file `http://archive.routeviews.org/route-views.chile/bgpdata/2023.03/RIBS/rib.20230326.0600.bz2`
     /// will be cached as `cache-682cb1eb-rib.20230326.0600.bz2` in the cache directory.
     pub fn new_cached(path: &str, cache_dir: &str) -> Result<Self, ParserErrorWithBytes> {
         let file_name = path.rsplit('/').next().unwrap().to_string();
-        let new_file_name = format!("cache-{}-{}", crc32(file_name.as_str()), file_name);
+        let new_file_name = format!(
+            "cache-{}",
+            add_suffix_to_filename(file_name.as_str(), crc32(path).as_str())
+        );
         let reader = get_cache_reader(path, cache_dir, Some(new_file_name), false)?;
         Ok(BgpkitParser {
             reader,
             core_dump: false,
             filters: vec![],
             options: ParserOptions::default(),
         })
     }
 }
 
+fn add_suffix_to_filename(filename: &str, suffix: &str) -> String {
+    let mut parts: Vec<&str> = filename.split('.').collect(); // Split filename by dots
+    if parts.len() > 1 {
+        let last_part = parts.pop().unwrap(); // Remove the last part (suffix) from the parts vector
+        let new_last_part = format!("{}.{}", suffix, last_part); // Add the suffix to the last part
+        parts.push(&new_last_part); // Add the updated last part back to the parts vector
+        parts.join(".") // Join the parts back into a filename string with dots
+    } else {
+        // If the filename does not have any dots, simply append the suffix to the end
+        format!("{}.{}", filename, suffix)
+    }
+}
+
 impl<R: Read> BgpkitParser<R> {
     /// Creating a new parser from a object that implements [Read] trait.
     pub fn from_reader(reader: R) -> Self {
         BgpkitParser {
             reader,
             core_dump: false,
             filters: vec![],
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/messages/bgp4mp.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/bgp4mp.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 use crate::error::ParserError;
+use crate::models::*;
 use crate::parser::bgp::messages::parse_bgp_message;
 use crate::parser::ReadUtils;
-use bgp_models::prelude::*;
-use byteorder::{ReadBytesExt, BE};
+use bytes::{Buf, Bytes};
 use num_traits::FromPrimitive;
-use std::io::Cursor;
 
 /// Parse MRT BGP4MP type
 ///
 /// RFC: https://www.rfc-editor.org/rfc/rfc6396#section-4.4
 ///
-pub fn parse_bgp4mp(sub_type: u16, input: &[u8]) -> Result<Bgp4Mp, ParserError> {
+pub fn parse_bgp4mp(sub_type: u16, input: Bytes) -> Result<Bgp4Mp, ParserError> {
     let bgp4mp_type: Bgp4MpType = match Bgp4MpType::from_u16(sub_type) {
         Some(t) => t,
         None => {
             return Err(ParserError::ParseError(format!(
                 "cannot parse bgp4mp subtype: {}",
                 sub_type
             )))
@@ -79,40 +78,37 @@
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |                      Local IP Address (variable)              |
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |                    BGP Message... (variable)
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 */
 pub fn parse_bgp4mp_message(
-    data: &[u8],
+    mut data: Bytes,
     add_path: bool,
     asn_len: AsnLength,
     msg_type: &Bgp4MpType,
 ) -> Result<Bgp4MpMessage, ParserError> {
     let total_size = data.len();
-    let mut input = Cursor::new(data);
 
-    let peer_asn: Asn = input.read_asn(&asn_len)?;
-    let local_asn: Asn = input.read_asn(&asn_len)?;
-    let interface_index: u16 = input.read_u16::<BE>()?;
-    let afi: Afi = input.read_afi()?;
-    let peer_ip = input.read_address(&afi)?;
-    let local_ip = input.read_address(&afi)?;
+    let peer_asn: Asn = data.read_asn(&asn_len)?;
+    let local_asn: Asn = data.read_asn(&asn_len)?;
+    let interface_index: u16 = data.read_u16()?;
+    let afi: Afi = data.read_afi()?;
+    let peer_ip = data.read_address(&afi)?;
+    let local_ip = data.read_address(&afi)?;
 
     let should_read = total_should_read(&afi, &asn_len, total_size);
-    let current_position = input.position() as usize;
-    let data_slice = &input.into_inner()[current_position..];
-    if should_read != data_slice.len() {
+    if should_read != data.remaining() {
         return Err(ParserError::TruncatedMsg(format!(
             "truncated bgp4mp message: should read {} bytes, have {} bytes available",
             should_read,
-            data_slice.len()
+            data.remaining()
         )));
     }
-    let bgp_message: BgpMessage = parse_bgp_message(data_slice, add_path, &asn_len)?;
+    let bgp_message: BgpMessage = parse_bgp_message(&mut data, add_path, &asn_len)?;
 
     Ok(Bgp4MpMessage {
         msg_type: *msg_type,
         peer_asn,
         local_asn,
         interface_index,
         afi,
@@ -150,34 +146,33 @@
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |                      Local IP Address (variable)              |
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |            Old State          |          New State            |
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 */
 pub fn parse_bgp4mp_state_change(
-    data: &[u8],
+    mut input: Bytes,
     asn_len: AsnLength,
     msg_type: &Bgp4MpType,
 ) -> Result<Bgp4MpStateChange, ParserError> {
-    let mut input = Cursor::new(data);
     let peer_asn: Asn = input.read_asn(&asn_len)?;
     let local_asn: Asn = input.read_asn(&asn_len)?;
-    let interface_index: u16 = input.read_u16::<BE>()?;
+    let interface_index: u16 = input.read_u16()?;
     let address_family: Afi = input.read_afi()?;
     let peer_addr = input.read_address(&address_family)?;
     let local_addr = input.read_address(&address_family)?;
-    let old_state = match BgpState::from_u16(input.read_u16::<BE>()?) {
+    let old_state = match BgpState::from_u16(input.read_u16()?) {
         Some(t) => t,
         None => {
             return Err(ParserError::ParseError(
                 "cannot parse bgp4mp old_state".to_string(),
             ))
         }
     };
-    let new_state = match BgpState::from_u16(input.read_u16::<BE>()?) {
+    let new_state = match BgpState::from_u16(input.read_u16()?) {
         Some(t) => t,
         None => {
             return Err(ParserError::ParseError(
                 "cannot parse bgp4mp new_state".to_string(),
             ))
         }
     };
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_message.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_message.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 use crate::error::*;
+use crate::models::*;
 use crate::parser::bgp::attributes::AttributeParser;
 use crate::parser::ReadUtils;
-use bgp_models::prelude::*;
-use byteorder::{ReadBytesExt, BE};
-use std::io::Cursor;
+use bytes::Bytes;
 use std::net::IpAddr;
 
 /// Parse MRT TABLE_DUMP type message.
 ///
 /// https://www.rfc-editor.org/rfc/rfc6396#section-4.2
 ///
 /// ```text
@@ -33,15 +32,15 @@
 /// |           Peer AS             |       Attribute Length        |
 /// +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 /// |                   BGP Attribute... (variable)
 /// +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 /// ```
 pub fn parse_table_dump_message(
     sub_type: u16,
-    data: &[u8],
+    mut data: Bytes,
 ) -> Result<TableDumpMessage, ParserError> {
     // ####
     // Step 0. prepare
     //   - define AS number length
     //   - determine address family
     //   - create data slice reader cursor
 
@@ -55,52 +54,50 @@
             return Err(ParserError::ParseError(format!(
                 "Invalid subtype found for TABLE_DUMP (V1) message: {}",
                 sub_type
             )))
         }
     };
 
-    // create a reader for the passed in data slice.
-    let mut input = Cursor::new(data);
-
     // ####
     // Step 1. read simple fields
     //   - view number
     //   - sequence number
     //   - prefix
     //   - prefix-length
     //   - status
     //   - originated time
     //   - peer IP address
     //   - peer ASN
     //   - attribute length
 
-    let view_number = input.read_u16::<BE>()?;
-    let sequence_number = input.read_u16::<BE>()?;
+    let view_number = data.read_u16()?;
+    let sequence_number = data.read_u16()?;
     let prefix = match &afi {
-        Afi::Ipv4 => input.read_ipv4_prefix().map(ipnet::IpNet::V4),
-        Afi::Ipv6 => input.read_ipv6_prefix().map(ipnet::IpNet::V6),
+        Afi::Ipv4 => data.read_ipv4_prefix().map(ipnet::IpNet::V4),
+        Afi::Ipv6 => data.read_ipv6_prefix().map(ipnet::IpNet::V6),
     }?;
-    let status = input.read_8b()?;
-    let time = input.read_32b()? as u64;
 
-    let peer_address: IpAddr = input.read_address(&afi)?;
-    let peer_asn = input.read_asn(&asn_len)?;
-    let attribute_length = input.read_u16::<BE>()? as usize;
+    let status = data.read_u8()?;
+    let time = data.read_u32()? as u64;
+
+    let peer_address: IpAddr = data.read_address(&afi)?;
+    let peer_asn = data.read_asn(&asn_len)?;
+
+    let attribute_length = data.read_u16()? as usize;
 
     // ####
     // Step 2. read the attributes
     //   - create subslice based on the cursor's current position
     //   - pass the data into the parser function
 
     let attr_parser = AttributeParser::new(false);
-    let current_position = input.position() as usize;
-    let attr_data_slice = &input.into_inner()[current_position..];
-    // TODO: relax this assertion with error matching later
-    assert_eq!(attr_data_slice.len(), attribute_length);
+
+    data.has_n_remaining(attribute_length)?;
+    let attr_data_slice = data.split_to(attribute_length);
     let attributes = attr_parser.parse_attributes(attr_data_slice, &asn_len, None, None, None)?;
 
     Ok(TableDumpMessage {
         view_number,
         sequence_number,
         prefix: NetworkPrefix::new(prefix, 0),
         status,
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_v2_message.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/messages/table_dump_v2_message.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 use crate::error::ParserError;
+use crate::models::*;
 use crate::parser::{AttributeParser, ReadUtils};
-use bgp_models::prelude::*;
-use byteorder::{ReadBytesExt, BE};
+use bytes::{Buf, Bytes};
 use log::warn;
 use num_traits::FromPrimitive;
 use std::collections::HashMap;
-use std::io::{Cursor, Seek, SeekFrom};
 use std::net::{IpAddr, Ipv4Addr};
 
 /// Parse TABLE_DUMP V2 format MRT message.
 ///
 /// RFC: https://www.rfc-editor.org/rfc/rfc6396#section-4.3
 ///
 /// Subtypes include
@@ -18,15 +17,15 @@
 /// 3. RIB_IPV4_MULTICAST
 /// 4. RIB_IPV6_UNICAST
 /// 5. RIB_IPV6_MULTICAST
 /// 6. RIB_GENERIC
 ///
 pub fn parse_table_dump_v2_message(
     sub_type: u16,
-    input: &[u8],
+    mut input: Bytes,
 ) -> Result<TableDumpV2Message, ParserError> {
     let v2_type: TableDumpV2Type = match TableDumpV2Type::from_u16(sub_type) {
         Some(t) => t,
         None => {
             return Err(ParserError::ParseError(format!(
                 "cannot parse table dump v2 type: {}",
                 sub_type
@@ -43,15 +42,15 @@
         | TableDumpV2Type::RibIpv4Multicast
         | TableDumpV2Type::RibIpv6Unicast
         | TableDumpV2Type::RibIpv6Multicast
         | TableDumpV2Type::RibIpv4UnicastAddPath
         | TableDumpV2Type::RibIpv4MulticastAddPath
         | TableDumpV2Type::RibIpv6UnicastAddPath
         | TableDumpV2Type::RibIpv6MulticastAddPath => {
-            TableDumpV2Message::RibAfiEntries(parse_rib_afi_entries(input, v2_type)?)
+            TableDumpV2Message::RibAfiEntries(parse_rib_afi_entries(&mut input, v2_type)?)
         }
         TableDumpV2Type::RibGeneric
         | TableDumpV2Type::RibGenericAddPath
         | TableDumpV2Type::GeoPeerTable => {
             return Err(ParserError::Unsupported(
                 "TableDumpV2 RibGeneric and GeoPeerTable is not currently supported".to_string(),
             ))
@@ -60,39 +59,37 @@
 
     Ok(msg)
 }
 
 /// Peer index table
 ///
 /// RFC: https://www.rfc-editor.org/rfc/rfc6396#section-4.3.1
-pub fn parse_peer_index_table(data: &[u8]) -> Result<PeerIndexTable, ParserError> {
-    let mut input = Cursor::new(data);
-
-    let collector_bgp_id = Ipv4Addr::from(input.read_32b()?);
+pub fn parse_peer_index_table(mut data: Bytes) -> Result<PeerIndexTable, ParserError> {
+    let collector_bgp_id = Ipv4Addr::from(data.read_u32()?);
     // read and ignore view name
-    let view_name_length = input.read_u16::<BE>()?;
-    // TODO: properly parse view_name
-    input.seek(SeekFrom::Current(view_name_length as i64))?;
+    let view_name_length = data.read_u16()?;
+    let view_name =
+        String::from_utf8(data.read_n_bytes(view_name_length as usize)?).unwrap_or("".to_string());
 
-    let peer_count = input.read_u16::<BE>()?;
+    let peer_count = data.read_u16()?;
     let mut peers = vec![];
     for _index in 0..peer_count {
-        let peer_type = input.read_8b()?;
+        let peer_type = data.read_u8()?;
         let afi = match peer_type & 1 {
             1 => Afi::Ipv6,
             _ => Afi::Ipv4,
         };
         let asn_len = match peer_type & 2 {
             2 => AsnLength::Bits32,
             _ => AsnLength::Bits16,
         };
 
-        let peer_bgp_id = Ipv4Addr::from(input.read_32b()?);
-        let peer_address: IpAddr = input.read_address(&afi)?;
-        let peer_asn = input.read_asn(&asn_len)?;
+        let peer_bgp_id = Ipv4Addr::from(data.read_u32()?);
+        let peer_address: IpAddr = data.read_address(&afi)?;
+        let peer_asn = data.read_asn(&asn_len)?;
         peers.push(Peer {
             peer_type,
             peer_bgp_id,
             peer_address,
             peer_asn,
         })
     }
@@ -102,29 +99,27 @@
     for (id, p) in peers.into_iter().enumerate() {
         peers_map.insert(id as u32, p);
     }
 
     Ok(PeerIndexTable {
         collector_bgp_id,
         view_name_length,
-        view_name: "".to_owned(),
+        view_name,
         peer_count,
         peers_map,
     })
 }
 
 /// RIB AFI-specific entries
 ///
 /// https://tools.ietf.org/html/rfc6396#section-4.3
 pub fn parse_rib_afi_entries(
-    data: &[u8],
+    data: &mut Bytes,
     rib_type: TableDumpV2Type,
 ) -> Result<RibAfiEntries, ParserError> {
-    let mut input = Cursor::new(data);
-
     let afi: Afi;
     let safi: Safi;
     match rib_type {
         TableDumpV2Type::RibIpv4Unicast | TableDumpV2Type::RibIpv4UnicastAddPath => {
             afi = Afi::Ipv4;
             safi = Safi::Unicast
         }
@@ -152,29 +147,29 @@
         rib_type,
         TableDumpV2Type::RibIpv4UnicastAddPath
             | TableDumpV2Type::RibIpv4MulticastAddPath
             | TableDumpV2Type::RibIpv6UnicastAddPath
             | TableDumpV2Type::RibIpv6MulticastAddPath
     );
 
-    let sequence_number = input.read_32b()?;
+    let sequence_number = data.read_u32()?;
 
     // NOTE: here we parse the prefix as only length and prefix, the path identifier for add_path
     //       entry is not handled here. We follow RFC6396 here https://www.rfc-editor.org/rfc/rfc6396.html#section-4.3.2
-    let prefix = input.read_nlri_prefix(&afi, false)?;
+    let prefix = data.read_nlri_prefix(&afi, false)?;
     let prefixes = vec![prefix];
 
-    let entry_count = input.read_u16::<BE>()?;
+    let entry_count = data.read_u16()?;
     let mut rib_entries = Vec::with_capacity((entry_count * 2) as usize);
 
     // get the u8 slice of the rest of the data
     // let attr_data_slice = &input.into_inner()[(input.position() as usize)..];
 
     for _i in 0..entry_count {
-        let entry = match parse_rib_entry(&mut input, add_path, &afi, &safi, &prefixes) {
+        let entry = match parse_rib_entry(data, add_path, &afi, &safi, &prefixes) {
             Ok(entry) => entry,
             Err(e) => {
                 warn!("early break due to error {}", e.to_string());
                 break;
             }
         };
         rib_entries.push(entry);
@@ -185,56 +180,49 @@
         sequence_number,
         prefix,
         rib_entries,
     })
 }
 
 pub fn parse_rib_entry(
-    input: &mut Cursor<&[u8]>,
+    input: &mut Bytes,
     add_path: bool,
     afi: &Afi,
     safi: &Safi,
     prefixes: &[NetworkPrefix],
 ) -> Result<RibEntry, ParserError> {
-    // TODO: fix the implementation here
-    let mut total_bytes_left = input.get_ref().len() - (input.position() as usize);
-    if total_bytes_left < 8 {
+    if input.remaining() < 8 {
         // total length - current position less than 16 --
         // meaning less than 16 bytes available to read
         return Err(ParserError::TruncatedMsg("truncated msg".to_string()));
     }
 
-    let peer_index = input.read_u16::<BE>()?;
-    let originated_time = input.read_32b()?;
-    total_bytes_left -= 6;
+    let peer_index = input.read_u16()?;
+    let originated_time = input.read_u32()?;
     if add_path {
-        let _path_id = input.read_32b()?;
-        total_bytes_left -= 4;
+        let _path_id = input.read_u32()?;
     }
-    let attribute_length = input.read_u16::<BE>()? as usize;
-    total_bytes_left -= 2;
+    let attribute_length = input.read_u16()? as usize;
 
-    // TODO: fix the implementation here
-    if total_bytes_left < attribute_length {
+    if input.remaining() < attribute_length {
         return Err(ParserError::TruncatedMsg("truncated msg".to_string()));
     }
 
     let attr_parser = AttributeParser::new(add_path);
 
-    let pos = input.position() as usize;
-    let pos_end = pos + attribute_length;
-    let attr_data_slice = &input.get_ref()[pos..pos_end];
+    let attr_data_slice = input.split_to(attribute_length);
     let attributes = attr_parser.parse_attributes(
         attr_data_slice,
         &AsnLength::Bits32,
         Some(*afi),
         Some(*safi),
         Some(prefixes),
     )?;
-    input.seek(SeekFrom::Start(pos_end as u64))?;
+
+    input.advance(input.remaining());
 
     Ok(RibEntry {
         peer_index,
         originated_time,
         attributes,
     })
 }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_elem.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_elem.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #![allow(unused)]
 //! This module handles converting MRT records into individual per-prefix BGP elements.
 //!
 //! Each MRT record may contain reachability information for multiple prefixes. This module breaks
 //! down MRT records into corresponding BGP elements, and thus allowing users to more conveniently
 //! process BGP information on a per-prefix basis.
+use crate::models::*;
 use crate::parser::bgp::messages::parse_bgp_update_message;
-use bgp_models::prelude::*;
 use itertools::Itertools;
 use log::warn;
 use std::collections::HashMap;
 use std::fmt::{Display, Formatter};
 use std::net::IpAddr;
 
 pub struct Elementor {
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_record.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/mrt/mrt_record.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 use crate::error::ParserError;
+use crate::models::*;
 use crate::parser::{
     parse_bgp4mp, parse_table_dump_message, parse_table_dump_v2_message, ParserErrorWithBytes,
-    ReadUtils,
 };
-use bgp_models::prelude::*;
-use byteorder::{ReadBytesExt, BE};
-use num_traits::FromPrimitive;
-use std::io::{ErrorKind, Read};
+use bytes::{Buf, Bytes, BytesMut};
+use num_traits::{FromPrimitive, ToPrimitive};
+use std::io::Read;
 
 /// MRT common header
 ///
 /// A MRT record is constructed as the following:
 /// ```text
 ///  0                   1                   2                   3
 ///  0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
@@ -39,38 +38,32 @@
 /// +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 /// |                      Microsecond Timestamp                    |
 /// +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 /// |                      Message... (variable)
 /// +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 /// ```
 pub fn parse_common_header<T: Read>(input: &mut T) -> Result<CommonHeader, ParserError> {
-    let timestamp = match input.read_32b() {
-        Ok(t) => t,
-        Err(e) => {
-            return match e.kind() {
-                ErrorKind::UnexpectedEof => Err(ParserError::EofExpected),
-                _ => Err(ParserError::from(e)),
-            }
-        }
-    };
+    let mut raw_bytes = [0u8; 12];
+    input.read_exact(&mut raw_bytes)?;
+    let mut data = BytesMut::from(&raw_bytes[..]);
+
+    let timestamp = data.get_u32();
+    let entry_type_raw = data.get_u16();
+    let entry_type = EntryType::from_u16(entry_type_raw).ok_or_else(|| {
+        ParserError::ParseError(format!("Failed to parse entry type: {}", entry_type_raw))
+    })?;
+    let entry_subtype = data.get_u16();
+    let mut length = data.get_u32();
 
-    let entry_type_raw = input.read_u16::<BE>()?;
-    let entry_type = match EntryType::from_u16(entry_type_raw) {
-        Some(t) => Ok(t),
-        None => Err(ParserError::ParseError(format!(
-            "Failed to parse entry type: {}",
-            entry_type_raw
-        ))),
-    }?;
-    let entry_subtype = input.read_u16::<BE>()?;
-    let mut length = input.read_32b()?;
     let microsecond_timestamp = match &entry_type {
         EntryType::BGP4MP_ET => {
             length -= 4;
-            Some(input.read_32b()?)
+            let mut raw_bytes: [u8; 4] = [0; 4];
+            input.read_exact(&mut raw_bytes)?;
+            Some(BytesMut::from(&raw_bytes[..]).get_u32())
         }
         _ => None,
     };
 
     Ok(CommonHeader {
         timestamp,
         microsecond_timestamp,
@@ -81,78 +74,110 @@
 }
 
 pub fn parse_mrt_record(input: &mut impl Read) -> Result<MrtRecord, ParserErrorWithBytes> {
     // parse common header
     let common_header = match parse_common_header(input) {
         Ok(v) => v,
         Err(e) => {
+            if let ParserError::EofError(e) = &e {
+                if e.kind() == std::io::ErrorKind::UnexpectedEof {
+                    return Err(ParserErrorWithBytes::from(ParserError::EofExpected));
+                }
+            }
             return Err(ParserErrorWithBytes {
                 error: e,
                 bytes: None,
-            })
+            });
         }
     };
 
     // read the whole message bytes to buffer
-    let mut buffer = Vec::with_capacity(common_header.length as usize);
+    let mut buffer = BytesMut::with_capacity(common_header.length as usize);
+    buffer.resize(common_header.length as usize, 0);
     match input
         .take(common_header.length as u64)
-        .read_to_end(&mut buffer)
+        .read_exact(&mut buffer)
     {
         Ok(_) => {}
         Err(e) => {
             return Err(ParserErrorWithBytes {
                 error: ParserError::IoError(e),
                 bytes: None,
             })
         }
     }
 
-    match parse_raw_bytes(&common_header, buffer.as_slice()) {
+    match parse_mrt_body(
+        common_header.entry_type.to_u16().unwrap(),
+        common_header.entry_subtype,
+        buffer.freeze(), // freeze the BytesMute to Bytes
+    ) {
         Ok(message) => Ok(MrtRecord {
             common_header,
             message,
         }),
         Err(e) => {
-            let mut total_bytes = vec![];
-            if common_header.write_header(&mut total_bytes).is_err() {
-                unreachable!("Vec<u8> will never produce errors when used as a std::io::Write")
-            }
-
-            total_bytes.extend(buffer);
+            // TODO: find more efficient way to preserve the bytes during error
+            // let mut total_bytes = vec![];
+            // if common_header.write_header(&mut total_bytes).is_err() {
+            //     unreachable!("Vec<u8> will never produce errors when used as a std::io::Write")
+            // }
+
+            // total_bytes.extend(buffer);
+            // Err(ParserErrorWithBytes {
+            //     error: e,
+            //     bytes: Some(total_bytes),
+            // })
             Err(ParserErrorWithBytes {
                 error: e,
-                bytes: Some(total_bytes),
+                bytes: None,
             })
         }
     }
 }
 
-fn parse_raw_bytes(common_header: &CommonHeader, data: &[u8]) -> Result<MrtMessage, ParserError> {
-    let message: MrtMessage = match &common_header.entry_type {
+/// Parse MRT message body with given entry type and subtype.
+///
+/// The entry type and subtype are parsed from the common header. The message body is parsed
+/// according to the entry type and subtype. The message body is the remaining bytes after the
+/// common header. The length of the message body is also parsed from the common header.
+fn parse_mrt_body(
+    entry_type: u16,
+    entry_subtype: u16,
+    data: Bytes,
+) -> Result<MrtMessage, ParserError> {
+    let etype = match EntryType::from_u16(entry_type) {
+        Some(t) => Ok(t),
+        None => Err(ParserError::ParseError(format!(
+            "Failed to parse entry type: {}",
+            entry_type
+        ))),
+    }?;
+
+    let message: MrtMessage = match &etype {
         EntryType::TABLE_DUMP => {
-            let msg = parse_table_dump_message(common_header.entry_subtype, data);
+            let msg = parse_table_dump_message(entry_subtype, data);
             match msg {
                 Ok(msg) => MrtMessage::TableDumpMessage(msg),
                 Err(e) => {
                     return Err(e);
                 }
             }
         }
         EntryType::TABLE_DUMP_V2 => {
-            let msg = parse_table_dump_v2_message(common_header.entry_subtype, data);
+            let msg = parse_table_dump_v2_message(entry_subtype, data);
             match msg {
                 Ok(msg) => MrtMessage::TableDumpV2Message(msg),
                 Err(e) => {
                     return Err(e);
                 }
             }
         }
         EntryType::BGP4MP | EntryType::BGP4MP_ET => {
-            let msg = parse_bgp4mp(common_header.entry_subtype, data);
+            let msg = parse_bgp4mp(entry_subtype, data);
             match msg {
                 Ok(msg) => MrtMessage::Bgp4Mp(msg),
                 Err(e) => {
                     return Err(e);
                 }
             }
         }
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/error.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/error.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/mod.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/mod.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/raw_bytes.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/raw_bytes.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+use crate::models::*;
 use crate::parser::bgp::parse_bgp_message;
 use crate::parser::rislive::error::ParserRisliveError;
-use crate::{BgpElem, Elementor};
-use bgp_models::prelude::*;
+use crate::Elementor;
+use bytes::Bytes;
 use serde_json::Value;
 use std::net::IpAddr;
 use std::str::FromStr;
 
 pub fn parse_raw_bytes(msg_str: &str) -> Result<Vec<BgpElem>, ParserRisliveError> {
     let msg: Value = serde_json::from_str(msg_str)?;
     let msg_type = match msg.get("type") {
@@ -19,32 +20,32 @@
             return Err(ParserRisliveError::UnsupportedMessage)
         }
         _ => return Err(ParserRisliveError::IrregularRisLiveFormat),
     }
 
     let data = msg.get("data").unwrap().as_object().unwrap();
 
-    let bytes = hex::decode(data.get("raw").unwrap().as_str().unwrap()).unwrap();
+    let mut bytes = Bytes::from(hex::decode(data.get("raw").unwrap().as_str().unwrap()).unwrap());
 
     let timestamp = data.get("timestamp").unwrap().as_f64().unwrap();
     let peer_str = data.get("peer").unwrap().as_str().unwrap().to_owned();
 
     let peer_ip = peer_str.parse::<IpAddr>().unwrap();
     let afi = match peer_ip.is_ipv4() {
         true => Afi::Ipv4,
         false => Afi::Ipv6,
     };
 
     let peer_asn_str = data.get("peer_asn").unwrap().as_str().unwrap().to_owned();
 
     let peer_asn = peer_asn_str.parse::<i32>().unwrap().into();
 
-    let bgp_msg = match parse_bgp_message(bytes.as_slice(), false, &AsnLength::Bits32) {
+    let bgp_msg = match parse_bgp_message(&mut bytes, false, &AsnLength::Bits32) {
         Ok(m) => m,
-        Err(_) => match parse_bgp_message(bytes.as_slice(), false, &AsnLength::Bits16) {
+        Err(_) => match parse_bgp_message(&mut bytes, false, &AsnLength::Bits16) {
             Ok(m) => m,
             Err(_) => return Err(ParserRisliveError::IncorrectRawBytes),
         },
     };
 
     let t_sec = timestamp as u32;
     let t_msec = get_micro_seconds(timestamp);
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_message.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/messages/ris_message.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-use bgp_models::prelude::AsPathSegment::{AsSequence, AsSet};
-use bgp_models::prelude::*;
+use crate::models::AsPathSegment::{AsSequence, AsSet};
+use crate::models::*;
 use serde::{Deserialize, Serialize};
 use serde_json::Value;
 
 #[derive(Debug, Serialize, Deserialize)]
 pub struct RisMessage {
     pub timestamp: f64,
     pub peer: String,
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/rislive/mod.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/rislive/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 }
 ```
 */
 use crate::parser::rislive::error::ParserRisliveError;
 use crate::parser::rislive::messages::ris_message::path_to_as_path;
 use crate::parser::rislive::messages::{RisLiveMessage, RisMessageEnum};
 
-use crate::BgpElem;
-use bgp_models::prelude::Origin::{EGP, IGP, INCOMPLETE};
-use bgp_models::prelude::*;
+use crate::models::*;
 use ipnet::IpNet;
 use std::net::IpAddr;
 
 pub mod error;
 pub mod messages;
 
 // simple macro to make the code look a bit nicer
@@ -114,17 +112,17 @@
                         }
                     };
 
                     // parse origin
                     let bgp_origin = match origin {
                         None => None,
                         Some(o) => Some(match o.as_str() {
-                            "igp" | "IGP" => IGP,
-                            "egp" | "EGP" => EGP,
-                            "incomplete" | "INCOMPLETE" => INCOMPLETE,
+                            "igp" | "IGP" => Origin::IGP,
+                            "egp" | "EGP" => Origin::EGP,
+                            "incomplete" | "INCOMPLETE" => Origin::INCOMPLETE,
                             other => {
                                 return Err(ParserRisliveError::ElemUnknownOriginType(
                                     other.to_string(),
                                 ))
                             }
                         }),
                     };
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/src/parser/utils.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/parser/utils.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 /*!
 Provides IO utility functions for read bytes of different length and converting to corresponding structs.
 */
 use ipnet::{IpNet, Ipv4Net, Ipv6Net};
-use std::io::{Cursor, Seek, SeekFrom};
 use std::{
     io,
     net::{Ipv4Addr, Ipv6Addr},
 };
 
-use bgp_models::prelude::*;
-use byteorder::{ReadBytesExt, BE};
+use crate::models::*;
+use bytes::{Buf, Bytes};
 use log::debug;
 use num_traits::FromPrimitive;
 use std::net::IpAddr;
 
 use crate::error::ParserError;
+use crate::ParserError::IoNotEnoughBytes;
+
+impl ReadUtils for Bytes {}
 
 // Allow reading IPs from Reads
-pub trait ReadUtils: io::Read {
-    fn read_8b(&mut self) -> io::Result<u8> {
-        self.read_u8()
+pub trait ReadUtils: Buf {
+    #[inline]
+    fn has_n_remaining(&self, n: usize) -> Result<(), ParserError> {
+        if self.remaining() < n {
+            Err(IoNotEnoughBytes())
+        } else {
+            Ok(())
+        }
     }
 
-    fn read_16b(&mut self) -> io::Result<u16> {
-        self.read_u16::<BE>()
+    #[inline]
+    fn read_u8(&mut self) -> Result<u8, ParserError> {
+        self.has_n_remaining(1)?;
+        Ok(self.get_u8())
     }
 
-    fn read_32b(&mut self) -> io::Result<u32> {
-        self.read_u32::<BE>()
+    #[inline]
+    fn read_u16(&mut self) -> Result<u16, ParserError> {
+        self.has_n_remaining(2)?;
+        Ok(self.get_u16())
     }
 
-    fn read_64b(&mut self) -> io::Result<u64> {
-        self.read_u64::<BE>()
+    #[inline]
+    fn read_u32(&mut self) -> Result<u32, ParserError> {
+        self.has_n_remaining(4)?;
+        Ok(self.get_u32())
     }
 
-    fn read_128b(&mut self) -> io::Result<u128> {
-        self.read_u128::<BE>()
+    #[inline]
+    fn read_u64(&mut self) -> Result<u64, ParserError> {
+        self.has_n_remaining(8)?;
+        Ok(self.get_u64())
     }
 
     fn read_address(&mut self, afi: &Afi) -> io::Result<IpAddr> {
         match afi {
             Afi::Ipv4 => match self.read_ipv4_address() {
                 Ok(ip) => Ok(IpAddr::V4(ip)),
                 _ => Err(io::Error::new(
@@ -54,103 +69,106 @@
                     "Cannot parse IPv6 address".to_string(),
                 )),
             },
         }
     }
 
     fn read_ipv4_address(&mut self) -> Result<Ipv4Addr, ParserError> {
-        let addr = self.read_32b()?;
+        let addr = self.read_u32()?;
         Ok(Ipv4Addr::from(addr))
     }
 
     fn read_ipv6_address(&mut self) -> Result<Ipv6Addr, ParserError> {
-        let buf = self.read_u128::<BE>()?;
+        self.has_n_remaining(16)?;
+        let buf = self.get_u128();
         Ok(Ipv6Addr::from(buf))
     }
 
     fn read_ipv4_prefix(&mut self) -> Result<Ipv4Net, ParserError> {
         let addr = self.read_ipv4_address()?;
-        let mask = self.read_8b()?;
+        let mask = self.read_u8()?;
         match Ipv4Net::new(addr, mask) {
             Ok(n) => Ok(n),
             Err(_) => Err(io::Error::new(io::ErrorKind::Other, "Invalid prefix mask").into()),
         }
     }
 
     fn read_ipv6_prefix(&mut self) -> Result<Ipv6Net, ParserError> {
         let addr = self.read_ipv6_address()?;
-        let mask = self.read_8b()?;
+        let mask = self.read_u8()?;
         match Ipv6Net::new(addr, mask) {
             Ok(n) => Ok(n),
             Err(_) => Err(io::Error::new(io::ErrorKind::Other, "Invalid prefix mask").into()),
         }
     }
 
     fn read_asn(&mut self, as_length: &AsnLength) -> Result<Asn, ParserError> {
         match as_length {
             AsnLength::Bits16 => {
-                let asn = self.read_16b()? as u32;
+                let asn = self.read_u16()? as u32;
                 Ok(Asn {
                     asn,
                     len: AsnLength::Bits16,
                 })
             }
             AsnLength::Bits32 => {
-                let asn = self.read_32b()?;
+                let asn = self.read_u32()?;
                 Ok(Asn {
                     asn,
                     len: AsnLength::Bits32,
                 })
             }
         }
     }
 
     fn read_asns(&mut self, as_length: &AsnLength, count: usize) -> Result<Vec<Asn>, ParserError> {
         let mut path = [0; 255];
         Ok(match as_length {
             AsnLength::Bits16 => {
+                self.has_n_remaining(count * 2)?; // 2 bytes for 16-bit ASN
                 for i in 0..count {
-                    path[i] = self.read_u16::<BE>()? as u32;
+                    path[i] = self.get_u16() as u32;
                 }
                 path[..count]
                     .iter()
                     .map(|asn| Asn {
                         asn: *asn,
                         len: *as_length,
                     })
                     .collect::<Vec<Asn>>()
             }
             AsnLength::Bits32 => {
+                self.has_n_remaining(count * 4)?; // 4 bytes for 32-bit ASN
                 for i in 0..count {
-                    path[i] = self.read_32b()?;
+                    path[i] = self.get_u32();
                 }
                 path[..count]
                     .iter()
                     .map(|asn| Asn {
                         asn: *asn,
                         len: *as_length,
                     })
                     .collect::<Vec<Asn>>()
             }
         })
     }
 
     fn read_afi(&mut self) -> Result<Afi, ParserError> {
-        let afi = self.read_u16::<BE>()?;
+        let afi = self.read_u16()?;
         match Afi::from_i16(afi as i16) {
             Some(afi) => Ok(afi),
             None => Err(crate::error::ParserError::Unsupported(format!(
                 "Unknown AFI type: {}",
                 afi
             ))),
         }
     }
 
     fn read_safi(&mut self) -> Result<Safi, ParserError> {
-        let safi = self.read_8b()?;
+        let safi = self.read_u8()?;
         match Safi::from_u8(safi) {
             Some(safi) => Ok(safi),
             None => Err(crate::error::ParserError::Unsupported(format!(
                 "Unknown SAFI type: {}",
                 safi
             ))),
         }
@@ -162,47 +180,49 @@
     /// If the `add_path` is true, it will also first read a 4-byte path id first; otherwise, a path-id of 0
     /// is automatically set.
     fn read_nlri_prefix(
         &mut self,
         afi: &Afi,
         add_path: bool,
     ) -> Result<NetworkPrefix, ParserError> {
-        let path_id = if add_path { self.read_32b()? } else { 0 };
+        let path_id = if add_path { self.read_u32()? } else { 0 };
 
         // Length in bits
-        let bit_len = self.read_8b()?;
+        let bit_len = self.read_u8()?;
 
         // Convert to bytes
         let byte_len: usize = (bit_len as usize + 7) / 8;
         let addr: IpAddr = match afi {
             Afi::Ipv4 => {
                 // 4 bytes -- u32
                 if byte_len > 4 {
                     return Err(ParserError::ParseError(format!(
                         "Invalid byte length for IPv4 prefix. byte_len: {}, bit_len: {}",
                         byte_len, bit_len
                     )));
                 }
                 let mut buff = [0; 4];
+                self.has_n_remaining(byte_len)?;
                 for i in 0..byte_len {
-                    buff[i] = self.read_8b()?
+                    buff[i] = self.get_u8();
                 }
                 IpAddr::V4(Ipv4Addr::from(buff))
             }
             Afi::Ipv6 => {
                 // 16 bytes
                 if byte_len > 16 {
                     return Err(ParserError::ParseError(format!(
                         "Invalid byte length for IPv6 prefix. byte_len: {}, bit_len: {}",
                         byte_len, bit_len
                     )));
                 }
+                self.has_n_remaining(byte_len)?;
                 let mut buff = [0; 16];
                 for i in 0..byte_len {
-                    buff[i] = self.read_8b()?
+                    buff[i] = self.get_u8();
                 }
                 IpAddr::V6(Ipv6Addr::from(buff))
             }
         };
         let prefix = match IpNet::new(addr, bit_len) {
             Ok(p) => p,
             Err(_) => {
@@ -213,56 +233,48 @@
             }
         };
 
         Ok(NetworkPrefix::new(prefix, path_id))
     }
 
     fn read_n_bytes(&mut self, n_bytes: usize) -> Result<Vec<u8>, ParserError> {
-        // TODO: fix the checking
-        // if self.total - self.pos < n_bytes {
-        //     return Err(ParserError::IoNotEnoughBytes())
-        // }
-        let mut bytes = vec![];
-        for _ in 0..n_bytes {
-            bytes.push(self.read_8b()?);
-        }
-        Ok(bytes)
+        self.has_n_remaining(n_bytes)?;
+        Ok(self.copy_to_bytes(n_bytes).into())
     }
 
     fn read_n_bytes_to_string(&mut self, n_bytes: usize) -> Result<String, ParserError> {
         let buffer = self.read_n_bytes(n_bytes)?;
         Ok(buffer
             .into_iter()
             .map(|x: u8| x as char)
             .collect::<String>())
     }
 }
 
 pub fn parse_nlri_list(
-    input: &mut Cursor<&[u8]>,
+    mut input: Bytes,
     add_path: bool,
     afi: &Afi,
-    total_bytes: u64,
 ) -> Result<Vec<NetworkPrefix>, ParserError> {
-    let pos_end = input.position() + total_bytes;
-
     let mut is_add_path = add_path;
     let mut prefixes = vec![];
 
     let mut retry = false;
     let mut guessed = false;
 
-    let pos_save = input.position();
+    let mut input_copy = None;
 
-    while input.position() < pos_end {
-        if !is_add_path && input.get_ref()[input.position() as usize] == 0 {
+    while input.remaining() > 0 {
+        if !is_add_path && input[0] == 0 {
             // it's likely that this is a add-path wrongfully wrapped in non-add-path msg
             debug!("not add-path but with NLRI size to be 0, likely add-path msg in wrong msg type, treat as add-path now");
+            // cloning the data bytes
             is_add_path = true;
             guessed = true;
+            input_copy = Some(input.clone());
         }
         let prefix = match input.read_nlri_prefix(afi, is_add_path) {
             Ok(p) => p,
             Err(e) => {
                 if guessed {
                     retry = true;
                     break;
@@ -273,27 +285,25 @@
         };
         prefixes.push(prefix);
     }
 
     if retry {
         prefixes.clear();
         // try again without attempt to guess add-path
-        input.seek(SeekFrom::Start(pos_save))?;
-        while input.position() < pos_end {
-            let prefix = input.read_nlri_prefix(afi, add_path)?;
+        // if we reach here (retry==true), input_copy must be Some
+        let mut input_2 = input_copy.unwrap();
+        while input_2.remaining() > 0 {
+            let prefix = input_2.read_nlri_prefix(afi, add_path)?;
             prefixes.push(prefix);
         }
     }
 
     Ok(prefixes)
 }
 
-// All types that implement Read can now read prefixes
-impl<R: io::Read> ReadUtils for R {}
-
 /// A CRC32 implementation that converts a string to a hex string.
 ///
 /// CRC32 is a checksum algorithm that is used to verify the integrity of data. It is short in
 /// length and sufficient for generating unique file names based on remote URLs.
 pub fn crc32(input: &str) -> String {
     let input_bytes = input.as_bytes();
     let mut table = [0u32; 256];
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgpkit-parser/tests/bgpkit-parser-tests.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/tests/bgpkit-parser-tests.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #[cfg(test)]
 mod tests {
-    use bgp_models::prelude::BgpElem;
+    use bgpkit_parser::models::BgpElem;
     use bgpkit_parser::BgpkitParser;
 
     #[test]
     fn test_parser_as_paths_conversion() {
         let url = "https://spaces.bgpkit.org/parser/update-example.gz";
         let parser = BgpkitParser::new(url)
             .unwrap()
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/README.md` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,195 +1,199 @@
-00000000: 2320 6267 702d 6d6f 6465 6c73 0a0a 6062  # bgp-models..`b
-00000010: 6770 2d6d 6f64 656c 7360 2069 7320 6120  gp-models` is a 
-00000020: 6c69 6272 6172 7920 7468 6174 2064 6566  library that def
-00000030: 696e 6573 2074 6865 2062 6173 6963 2042  ines the basic B
-00000040: 4750 2061 6e64 204d 5254 206d 6573 7361  GP and MRT messa
-00000050: 6765 2064 6174 6120 7374 7275 6374 7572  ge data structur
-00000060: 6573 2e0a 5468 6973 206c 6962 7261 7279  es..This library
-00000070: 2061 696d 7320 746f 2070 726f 7669 6465   aims to provide
-00000080: 2062 7569 6c64 696e 6720 626c 6f63 6b73   building blocks
-00000090: 2066 6f72 2064 6f77 6e73 7472 6561 6d20   for downstream 
-000000a0: 6c69 6272 6172 6965 7320 776f 726b 696e  libraries workin
-000000b0: 6720 7769 7468 2042 4750 2061 6e64 204d  g with BGP and M
-000000c0: 5254 0a6d 6573 7361 6765 7320 7375 6368  RT.messages such
-000000d0: 2061 7320 4d52 5420 7061 7273 6572 206f   as MRT parser o
-000000e0: 7220 4247 5020 7461 626c 6520 636f 6e73  r BGP table cons
-000000f0: 7472 7563 746f 722e 0a0a 2323 204d 696e  tructor...## Min
-00000100: 696d 756d 2053 7570 706f 7274 6564 2052  imum Supported R
-00000110: 7573 7420 5665 7273 696f 6e0a 0a60 312e  ust Version..`1.
-00000120: 3436 2e30 600a 0a23 2320 5375 7070 6f72  46.0`..## Suppor
-00000130: 7465 6420 5246 4373 0a0a 4d6f 7374 206f  ted RFCs..Most o
-00000140: 6620 7468 6520 7374 7275 6374 7320 6465  f the structs de
-00000150: 6669 6e65 6420 696e 2074 6869 7320 6c69  fined in this li
-00000160: 6272 6172 7920 6172 6520 6e61 6d65 6420  brary are named 
-00000170: 6166 7465 7220 7468 6520 666f 726d 616c  after the formal
-00000180: 2064 6566 696e 6974 696f 6e73 2069 6e20   definitions in 
-00000190: 6120 6e75 6d62 6572 206f 660a 5246 4373  a number of.RFCs
-000001a0: 2e20 4865 7265 2069 7320 6120 6c69 7374  . Here is a list
-000001b0: 206f 6620 7468 656d 3a0a 0a23 2323 2042   of them:..### B
-000001c0: 4750 0a2d 205b 585d 205b 5246 4320 3230  GP.- [X] [RFC 20
-000001d0: 3432 5d28 6874 7470 733a 2f2f 6461 7461  42](https://data
-000001e0: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
-000001f0: 2f64 6f63 2f68 746d 6c2f 7266 6332 3034  /doc/html/rfc204
-00000200: 3229 3a20 5265 6769 7374 6572 696e 6720  2): Registering 
-00000210: 4e65 7720 4247 5020 4174 7472 6962 7574  New BGP Attribut
-00000220: 6520 5479 7065 730a 2d20 5b58 5d20 5b52  e Types.- [X] [R
-00000230: 4643 2033 3339 325d 2868 7474 7073 3a2f  FC 3392](https:/
-00000240: 2f64 6174 6174 7261 636b 6572 2e69 6574  /datatracker.iet
-00000250: 662e 6f72 672f 646f 632f 6874 6d6c 2f72  f.org/doc/html/r
-00000260: 6663 3333 3932 293a 2043 6170 6162 696c  fc3392): Capabil
-00000270: 6974 6965 7320 4164 7665 7274 6973 656d  ities Advertisem
-00000280: 656e 7420 7769 7468 2042 4750 2d34 0a2d  ent with BGP-4.-
-00000290: 205b 585d 205b 5246 4320 3432 3731 5d28   [X] [RFC 4271](
-000002a0: 6874 7470 733a 2f2f 6461 7461 7472 6163  https://datatrac
-000002b0: 6b65 722e 6965 7466 2e6f 7267 2f64 6f63  ker.ietf.org/doc
-000002c0: 2f68 746d 6c2f 7266 6334 3237 3129 3a20  /html/rfc4271): 
-000002d0: 4120 426f 7264 6572 2047 6174 6577 6179  A Border Gateway
-000002e0: 2050 726f 746f 636f 6c20 3420 2842 4750   Protocol 4 (BGP
-000002f0: 2d34 290a 2d20 5b58 5d20 5b52 4643 2034  -4).- [X] [RFC 4
-00000300: 3435 365d 2868 7474 7073 3a2f 2f64 6174  456](https://dat
-00000310: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
-00000320: 672f 646f 632f 6874 6d6c 2f72 6663 3434  g/doc/html/rfc44
-00000330: 3536 293a 2042 4750 2052 6f75 7465 2052  56): BGP Route R
-00000340: 6566 6c65 6374 696f 6e3a 2041 6e20 416c  eflection: An Al
-00000350: 7465 726e 6174 6976 6520 746f 2046 756c  ternative to Ful
-00000360: 6c20 4d65 7368 2049 6e74 6572 6e61 6c20  l Mesh Internal 
-00000370: 4247 5020 2849 4247 5029 0a2d 205b 585d  BGP (IBGP).- [X]
-00000380: 205b 5246 4320 3530 3635 5d28 6874 7470   [RFC 5065](http
-00000390: 733a 2f2f 6461 7461 7472 6163 6b65 722e  s://datatracker.
-000003a0: 6965 7466 2e6f 7267 2f64 6f63 2f68 746d  ietf.org/doc/htm
-000003b0: 6c2f 7266 6335 3036 3529 3a20 4175 746f  l/rfc5065): Auto
-000003c0: 6e6f 6d6f 7573 2053 7973 7465 6d20 436f  nomous System Co
-000003d0: 6e66 6564 6572 6174 696f 6e73 2066 6f72  nfederations for
-000003e0: 2042 4750 0a2d 205b 585d 205b 5246 4320   BGP.- [X] [RFC 
-000003f0: 3637 3933 5d28 6874 7470 733a 2f2f 6461  6793](https://da
-00000400: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
-00000410: 7267 2f64 6f63 2f68 746d 6c2f 7266 6336  rg/doc/html/rfc6
-00000420: 3739 3329 3a20 4247 5020 5375 7070 6f72  793): BGP Suppor
-00000430: 7420 666f 7220 466f 7572 2d4f 6374 6574  t for Four-Octet
-00000440: 2041 7574 6f6e 6f6d 6f75 7320 5379 7374   Autonomous Syst
-00000450: 656d 2028 4153 2920 4e75 6d62 6572 2053  em (AS) Number S
-00000460: 7061 6365 0a2d 205b 585d 205b 5246 4320  pace.- [X] [RFC 
-00000470: 3739 3131 5d28 6874 7470 733a 2f2f 6461  7911](https://da
-00000480: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
-00000490: 7267 2f64 6f63 2f68 746d 6c2f 7266 6337  rg/doc/html/rfc7
-000004a0: 3931 3129 3a20 4164 7665 7274 6973 656d  911): Advertisem
-000004b0: 656e 7420 6f66 204d 756c 7469 706c 6520  ent of Multiple 
-000004c0: 5061 7468 7320 696e 2042 4750 2028 4144  Paths in BGP (AD
-000004d0: 442d 5041 5448 290a 2d20 5b58 5d20 5b52  D-PATH).- [X] [R
-000004e0: 4643 2039 3037 325d 2868 7474 7073 3a2f  FC 9072](https:/
-000004f0: 2f64 6174 6174 7261 636b 6572 2e69 6574  /datatracker.iet
-00000500: 662e 6f72 672f 646f 632f 6874 6d6c 2f72  f.org/doc/html/r
-00000510: 6663 3930 3732 293a 2045 7874 656e 6465  fc9072): Extende
-00000520: 6420 4f70 7469 6f6e 616c 2050 6172 616d  d Optional Param
-00000530: 6574 6572 7320 4c65 6e67 7468 2066 6f72  eters Length for
-00000540: 2042 4750 204f 5045 4e20 4d65 7373 6167   BGP OPEN Messag
-00000550: 6520 5570 6461 7465 730a 2d20 5b58 5d20  e Updates.- [X] 
-00000560: 5b52 4643 2039 3233 345d 2868 7474 7073  [RFC 9234](https
-00000570: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
-00000580: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
-00000590: 2f72 6663 3932 3334 293a 2052 6f75 7465  /rfc9234): Route
-000005a0: 204c 6561 6b20 5072 6576 656e 7469 6f6e   Leak Prevention
-000005b0: 2061 6e64 2044 6574 6563 7469 6f6e 2055   and Detection U
-000005c0: 7369 6e67 2052 6f6c 6573 2069 6e20 5550  sing Roles in UP
-000005d0: 4441 5445 2061 6e64 204f 5045 4e20 4d65  DATE and OPEN Me
-000005e0: 7373 6167 6573 0a0a 2323 2320 4d52 540a  ssages..### MRT.
-000005f0: 0a2d 205b 585d 205b 5246 4320 3633 3936  .- [X] [RFC 6396
-00000600: 5d28 6874 7470 733a 2f2f 6461 7461 7472  ](https://datatr
-00000610: 6163 6b65 722e 6965 7466 2e6f 7267 2f64  acker.ietf.org/d
-00000620: 6f63 2f68 746d 6c2f 7266 6336 3339 3629  oc/html/rfc6396)
-00000630: 3a20 4d75 6c74 692d 5468 7265 6164 6564  : Multi-Threaded
-00000640: 2052 6f75 7469 6e67 2054 6f6f 6c6b 6974   Routing Toolkit
-00000650: 2028 4d52 5429 2052 6f75 7469 6e67 2049   (MRT) Routing I
-00000660: 6e66 6f72 6d61 7469 6f6e 2045 7870 6f72  nformation Expor
-00000670: 7420 466f 726d 6174 0a2d 205b 205d 205b  t Format.- [ ] [
-00000680: 5246 4320 3633 3937 5d28 6874 7470 733a  RFC 6397](https:
-00000690: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
-000006a0: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
-000006b0: 7266 6336 3339 3729 3a20 4d75 6c74 692d  rfc6397): Multi-
-000006c0: 5468 7265 6164 6564 2052 6f75 7469 6e67  Threaded Routing
-000006d0: 2054 6f6f 6c6b 6974 2028 4d52 5429 2042   Toolkit (MRT) B
-000006e0: 6f72 6465 7220 4761 7465 7761 7920 5072  order Gateway Pr
-000006f0: 6f74 6f63 6f6c 2028 4247 5029 2052 6f75  otocol (BGP) Rou
-00000700: 7469 6e67 2049 6e66 6f72 6d61 7469 6f6e  ting Information
-00000710: 2045 7870 6f72 7420 466f 726d 6174 2077   Export Format w
-00000720: 6974 6820 4765 6f2d 4c6f 6361 7469 6f6e  ith Geo-Location
-00000730: 2045 7874 656e 7369 6f6e 730a 2d20 5b58   Extensions.- [X
-00000740: 5d20 5b52 4643 2038 3035 305d 2868 7474  ] [RFC 8050](htt
-00000750: 7073 3a2f 2f64 6174 6174 7261 636b 6572  ps://datatracker
-00000760: 2e69 6574 662e 6f72 672f 646f 632f 6874  .ietf.org/doc/ht
-00000770: 6d6c 2f72 6663 3830 3530 293a 204d 756c  ml/rfc8050): Mul
-00000780: 7469 2d54 6872 6561 6465 6420 526f 7574  ti-Threaded Rout
-00000790: 696e 6720 546f 6f6c 6b69 7420 284d 5254  ing Toolkit (MRT
-000007a0: 2920 526f 7574 696e 6720 496e 666f 726d  ) Routing Inform
-000007b0: 6174 696f 6e20 4578 706f 7274 2046 6f72  ation Export For
-000007c0: 6d61 7420 7769 7468 2042 4750 2041 6464  mat with BGP Add
-000007d0: 6974 696f 6e61 6c20 5061 7468 2045 7874  itional Path Ext
-000007e0: 656e 7369 6f6e 730a 0a23 2323 2043 6f6d  ensions..### Com
-000007f0: 6d75 6e69 7469 6573 0a0a 2d20 5b58 5d20  munities..- [X] 
-00000800: 5b52 4643 2031 3937 375d 2868 7474 7073  [RFC 1977](https
-00000810: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
-00000820: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
-00000830: 2f72 6663 3139 3737 293a 2042 4750 2043  /rfc1977): BGP C
-00000840: 6f6d 6d75 6e69 7469 6573 2041 7474 7269  ommunities Attri
-00000850: 6275 7465 0a2d 205b 585d 205b 5246 4320  bute.- [X] [RFC 
-00000860: 3433 3630 5d28 6874 7470 733a 2f2f 6461  4360](https://da
-00000870: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
-00000880: 7267 2f64 6f63 2f68 746d 6c2f 7266 6334  rg/doc/html/rfc4
-00000890: 3336 3029 3a20 4247 5020 4578 7465 6e64  360): BGP Extend
-000008a0: 6564 2043 6f6d 6d75 6e69 7469 6573 2041  ed Communities A
-000008b0: 7474 7269 6275 7465 0a2d 205b 585d 205b  ttribute.- [X] [
-000008c0: 5246 4320 3536 3638 5d28 6874 7470 733a  RFC 5668](https:
-000008d0: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
-000008e0: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
-000008f0: 7266 6335 3636 3829 3a20 342d 4f63 7465  rfc5668): 4-Octe
-00000900: 7420 4153 2053 7065 6369 6669 6320 4247  t AS Specific BG
-00000910: 5020 4578 7465 6e64 6564 2043 6f6d 6d75  P Extended Commu
-00000920: 6e69 7479 0a2d 205b 585d 205b 5246 4320  nity.- [X] [RFC 
-00000930: 3537 3031 5d28 6874 7470 733a 2f2f 6461  5701](https://da
-00000940: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
-00000950: 7267 2f64 6f63 2f68 746d 6c2f 7266 6335  rg/doc/html/rfc5
-00000960: 3730 3129 3a20 4950 7636 2041 6464 7265  701): IPv6 Addre
-00000970: 7373 2053 7065 6369 6669 6320 4247 5020  ss Specific BGP 
-00000980: 4578 7465 6e64 6564 2043 6f6d 6d75 6e69  Extended Communi
-00000990: 7479 2041 7474 7269 6275 7465 0a2d 205b  ty Attribute.- [
-000009a0: 585d 205b 5246 4320 3731 3533 5d28 6874  X] [RFC 7153](ht
-000009b0: 7470 733a 2f2f 6461 7461 7472 6163 6b65  tps://datatracke
-000009c0: 722e 6965 7466 2e6f 7267 2f64 6f63 2f68  r.ietf.org/doc/h
-000009d0: 746d 6c2f 7266 6337 3135 3329 3a20 4941  tml/rfc7153): IA
-000009e0: 4e41 2052 6567 6973 7472 6965 7320 666f  NA Registries fo
-000009f0: 7220 4247 5020 4578 7465 6e64 6564 2043  r BGP Extended C
-00000a00: 6f6d 6d75 6e69 7469 6573 2055 7064 6174  ommunities Updat
-00000a10: 6573 2034 3336 302c 2035 3730 310a 2d20  es 4360, 5701.- 
-00000a20: 5b58 5d20 5b52 4643 2038 3039 375d 2868  [X] [RFC 8097](h
-00000a30: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
-00000a40: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
-00000a50: 6874 6d6c 2f72 6663 3830 3937 293a 2042  html/rfc8097): B
-00000a60: 4750 2050 7265 6669 7820 4f72 6967 696e  GP Prefix Origin
-00000a70: 2056 616c 6964 6174 696f 6e20 5374 6174   Validation Stat
-00000a80: 6520 4578 7465 6e64 6564 2043 6f6d 6d75  e Extended Commu
-00000a90: 6e69 7479 0a2d 205b 585d 205b 5246 4320  nity.- [X] [RFC 
-00000aa0: 3830 3932 5d28 6874 7470 733a 2f2f 6461  8092](https://da
-00000ab0: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
-00000ac0: 7267 2f64 6f63 2f68 746d 6c2f 7266 6338  rg/doc/html/rfc8
-00000ad0: 3039 3229 3a20 4247 5020 4c61 7267 6520  092): BGP Large 
-00000ae0: 436f 6d6d 756e 6974 6965 730a 0a23 2320  Communities..## 
-00000af0: 5573 6564 2042 790a 0a2d 205b 6267 706b  Used By..- [bgpk
-00000b00: 6974 2d70 6172 7365 725d 2868 7474 7073  it-parser](https
-00000b10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6267  ://github.com/bg
-00000b20: 706b 6974 2f62 6770 6b69 742d 7061 7273  pkit/bgpkit-pars
-00000b30: 6572 290a 2d20 5b72 6973 2d6c 6976 652d  er).- [ris-live-
-00000b40: 7273 5d28 6874 7470 733a 2f2f 6769 7468  rs](https://gith
-00000b50: 7562 2e63 6f6d 2f62 6770 6b69 742f 7269  ub.com/bgpkit/ri
-00000b60: 732d 6c69 7665 2d72 7329 0a0a 2323 2042  s-live-rs)..## B
-00000b70: 7569 6c74 2077 6974 6820 e29d a4ef b88f  uilt with ......
-00000b80: 2062 7920 4247 504b 4954 2054 6561 6d0a   by BGPKIT Team.
-00000b90: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00000ba0: 2f2f 6267 706b 6974 2e63 6f6d 223e 3c69  //bgpkit.com"><i
-00000bb0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000bc0: 6267 706b 6974 2e63 6f6d 2f4f 7269 6769  bgpkit.com/Origi
-00000bd0: 6e61 6c25 3230 4c6f 676f 2532 3043 726f  nal%20Logo%20Cro
-00000be0: 7070 6564 2e70 6e67 2220 616c 743d 2268  pped.png" alt="h
-00000bf0: 7474 7073 3a2f 2f62 6770 6b69 742e 636f  ttps://bgpkit.co
-00000c00: 6d2f 6661 7669 636f 6e2e 6963 6f22 2077  m/favicon.ico" w
-00000c10: 6964 7468 3d22 3230 3022 2f3e 3c2f 613e  idth="200"/></a>
-00000c20: 0a                                       .
+00000000: 2f2a 210a 6062 6770 2d6d 6f64 656c 7360  /*!.`bgp-models`
+00000010: 2069 7320 6120 6c69 6272 6172 7920 7468   is a library th
+00000020: 6174 2064 6566 696e 6573 2074 6865 2062  at defines the b
+00000030: 6173 6963 2042 4750 2061 6e64 204d 5254  asic BGP and MRT
+00000040: 206d 6573 7361 6765 2064 6174 6120 7374   message data st
+00000050: 7275 6374 7572 6573 2e0a 5468 6973 206c  ructures..This l
+00000060: 6962 7261 7279 2061 696d 7320 746f 2070  ibrary aims to p
+00000070: 726f 7669 6465 2062 7569 6c64 696e 6720  rovide building 
+00000080: 626c 6f63 6b73 2066 6f72 2064 6f77 6e73  blocks for downs
+00000090: 7472 6561 6d20 6c69 6272 6172 6965 7320  tream libraries 
+000000a0: 776f 726b 696e 6720 7769 7468 2042 4750  working with BGP
+000000b0: 2061 6e64 204d 5254 0a6d 6573 7361 6765   and MRT.message
+000000c0: 7320 7375 6368 2061 7320 4d52 5420 6267  s such as MRT bg
+000000d0: 706b 6974 2d70 6172 7365 7220 6f72 2042  pkit-parser or B
+000000e0: 4750 2074 6162 6c65 2063 6f6e 7374 7275  GP table constru
+000000f0: 6374 6f72 2e0a 0a23 2320 5375 7070 6f72  ctor...## Suppor
+00000100: 7465 6420 5246 4373 0a0a 4d6f 7374 206f  ted RFCs..Most o
+00000110: 6620 7468 6520 7374 7275 6374 7320 6465  f the structs de
+00000120: 6669 6e65 6420 696e 2074 6869 7320 6c69  fined in this li
+00000130: 6272 6172 7920 6172 6520 6e61 6d65 6420  brary are named 
+00000140: 6166 7465 7220 7468 6520 666f 726d 616c  after the formal
+00000150: 2064 6566 696e 6974 696f 6e73 2069 6e20   definitions in 
+00000160: 6120 6e75 6d62 6572 206f 660a 5246 4373  a number of.RFCs
+00000170: 2e20 4865 7265 2069 7320 6120 6c69 7374  . Here is a list
+00000180: 206f 6620 7468 656d 3a0a 0a23 2323 2042   of them:..### B
+00000190: 4750 0a2d 205b 585d 205b 5246 4320 3230  GP.- [X] [RFC 20
+000001a0: 3432 5d28 6874 7470 733a 2f2f 6461 7461  42](https://data
+000001b0: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
+000001c0: 2f64 6f63 2f68 746d 6c2f 7266 6332 3034  /doc/html/rfc204
+000001d0: 3229 3a20 5265 6769 7374 6572 696e 6720  2): Registering 
+000001e0: 4e65 7720 4247 5020 4174 7472 6962 7574  New BGP Attribut
+000001f0: 6520 5479 7065 730a 2d20 5b58 5d20 5b52  e Types.- [X] [R
+00000200: 4643 2033 3339 325d 2868 7474 7073 3a2f  FC 3392](https:/
+00000210: 2f64 6174 6174 7261 636b 6572 2e69 6574  /datatracker.iet
+00000220: 662e 6f72 672f 646f 632f 6874 6d6c 2f72  f.org/doc/html/r
+00000230: 6663 3333 3932 293a 2043 6170 6162 696c  fc3392): Capabil
+00000240: 6974 6965 7320 4164 7665 7274 6973 656d  ities Advertisem
+00000250: 656e 7420 7769 7468 2042 4750 2d34 0a2d  ent with BGP-4.-
+00000260: 205b 585d 205b 5246 4320 3432 3731 5d28   [X] [RFC 4271](
+00000270: 6874 7470 733a 2f2f 6461 7461 7472 6163  https://datatrac
+00000280: 6b65 722e 6965 7466 2e6f 7267 2f64 6f63  ker.ietf.org/doc
+00000290: 2f68 746d 6c2f 7266 6334 3237 3129 3a20  /html/rfc4271): 
+000002a0: 4120 426f 7264 6572 2047 6174 6577 6179  A Border Gateway
+000002b0: 2050 726f 746f 636f 6c20 3420 2842 4750   Protocol 4 (BGP
+000002c0: 2d34 290a 2d20 5b58 5d20 5b52 4643 2035  -4).- [X] [RFC 5
+000002d0: 3036 355d 2868 7474 7073 3a2f 2f64 6174  065](https://dat
+000002e0: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
+000002f0: 672f 646f 632f 6874 6d6c 2f72 6663 3530  g/doc/html/rfc50
+00000300: 3635 293a 2041 7574 6f6e 6f6d 6f75 7320  65): Autonomous 
+00000310: 5379 7374 656d 2043 6f6e 6665 6465 7261  System Confedera
+00000320: 7469 6f6e 7320 666f 7220 4247 500a 2d20  tions for BGP.- 
+00000330: 5b58 5d20 5b52 4643 2036 3739 335d 2868  [X] [RFC 6793](h
+00000340: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+00000350: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+00000360: 6874 6d6c 2f72 6663 3637 3933 293a 2042  html/rfc6793): B
+00000370: 4750 2053 7570 706f 7274 2066 6f72 2046  GP Support for F
+00000380: 6f75 722d 4f63 7465 7420 4175 746f 6e6f  our-Octet Autono
+00000390: 6d6f 7573 2053 7973 7465 6d20 2841 5329  mous System (AS)
+000003a0: 204e 756d 6265 7220 5370 6163 650a 2d20   Number Space.- 
+000003b0: 5b58 5d20 5b52 4643 2037 3931 315d 2868  [X] [RFC 7911](h
+000003c0: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+000003d0: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+000003e0: 6874 6d6c 2f72 6663 3739 3131 293a 2041  html/rfc7911): A
+000003f0: 6476 6572 7469 7365 6d65 6e74 206f 6620  dvertisement of 
+00000400: 4d75 6c74 6970 6c65 2050 6174 6873 2069  Multiple Paths i
+00000410: 6e20 4247 5020 2841 4444 2d50 4154 4829  n BGP (ADD-PATH)
+00000420: 0a2d 205b 585d 205b 5246 4320 3930 3732  .- [X] [RFC 9072
+00000430: 5d28 6874 7470 733a 2f2f 6461 7461 7472  ](https://datatr
+00000440: 6163 6b65 722e 6965 7466 2e6f 7267 2f64  acker.ietf.org/d
+00000450: 6f63 2f68 746d 6c2f 7266 6339 3037 3229  oc/html/rfc9072)
+00000460: 3a20 4578 7465 6e64 6564 204f 7074 696f  : Extended Optio
+00000470: 6e61 6c20 5061 7261 6d65 7465 7273 204c  nal Parameters L
+00000480: 656e 6774 6820 666f 7220 4247 5020 4f50  ength for BGP OP
+00000490: 454e 204d 6573 7361 6765 2055 7064 6174  EN Message Updat
+000004a0: 6573 0a2d 205b 585d 205b 5246 4320 3932  es.- [X] [RFC 92
+000004b0: 3334 5d28 6874 7470 733a 2f2f 6461 7461  34](https://data
+000004c0: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
+000004d0: 2f64 6f63 2f68 746d 6c2f 7266 6339 3233  /doc/html/rfc923
+000004e0: 3429 3a20 526f 7574 6520 4c65 616b 2050  4): Route Leak P
+000004f0: 7265 7665 6e74 696f 6e20 616e 6420 4465  revention and De
+00000500: 7465 6374 696f 6e20 5573 696e 6720 526f  tection Using Ro
+00000510: 6c65 7320 696e 2055 5044 4154 4520 616e  les in UPDATE an
+00000520: 6420 4f50 454e 204d 6573 7361 6765 730a  d OPEN Messages.
+00000530: 0a23 2323 204d 5254 0a0a 2d20 5b58 5d20  .### MRT..- [X] 
+00000540: 5b52 4643 2036 3339 365d 2868 7474 7073  [RFC 6396](https
+00000550: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
+00000560: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
+00000570: 2f72 6663 3633 3936 293a 204d 756c 7469  /rfc6396): Multi
+00000580: 2d54 6872 6561 6465 6420 526f 7574 696e  -Threaded Routin
+00000590: 6720 546f 6f6c 6b69 7420 284d 5254 2920  g Toolkit (MRT) 
+000005a0: 526f 7574 696e 6720 496e 666f 726d 6174  Routing Informat
+000005b0: 696f 6e20 4578 706f 7274 2046 6f72 6d61  ion Export Forma
+000005c0: 740a 2d20 5b20 5d20 5b52 4643 2036 3339  t.- [ ] [RFC 639
+000005d0: 375d 2868 7474 7073 3a2f 2f64 6174 6174  7](https://datat
+000005e0: 7261 636b 6572 2e69 6574 662e 6f72 672f  racker.ietf.org/
+000005f0: 646f 632f 6874 6d6c 2f72 6663 3633 3937  doc/html/rfc6397
+00000600: 293a 204d 756c 7469 2d54 6872 6561 6465  ): Multi-Threade
+00000610: 6420 526f 7574 696e 6720 546f 6f6c 6b69  d Routing Toolki
+00000620: 7420 284d 5254 2920 426f 7264 6572 2047  t (MRT) Border G
+00000630: 6174 6577 6179 2050 726f 746f 636f 6c20  ateway Protocol 
+00000640: 2842 4750 2920 526f 7574 696e 6720 496e  (BGP) Routing In
+00000650: 666f 726d 6174 696f 6e20 4578 706f 7274  formation Export
+00000660: 2046 6f72 6d61 7420 7769 7468 2047 656f   Format with Geo
+00000670: 2d4c 6f63 6174 696f 6e20 4578 7465 6e73  -Location Extens
+00000680: 696f 6e73 0a2d 205b 585d 205b 5246 4320  ions.- [X] [RFC 
+00000690: 3830 3530 5d28 6874 7470 733a 2f2f 6461  8050](https://da
+000006a0: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
+000006b0: 7267 2f64 6f63 2f68 746d 6c2f 7266 6338  rg/doc/html/rfc8
+000006c0: 3035 3029 3a20 4d75 6c74 692d 5468 7265  050): Multi-Thre
+000006d0: 6164 6564 2052 6f75 7469 6e67 2054 6f6f  aded Routing Too
+000006e0: 6c6b 6974 2028 4d52 5429 2052 6f75 7469  lkit (MRT) Routi
+000006f0: 6e67 2049 6e66 6f72 6d61 7469 6f6e 2045  ng Information E
+00000700: 7870 6f72 7420 466f 726d 6174 2077 6974  xport Format wit
+00000710: 6820 4247 5020 4164 6469 7469 6f6e 616c  h BGP Additional
+00000720: 2050 6174 6820 4578 7465 6e73 696f 6e73   Path Extensions
+00000730: 0a0a 2323 2320 436f 6d6d 756e 6974 6965  ..### Communitie
+00000740: 730a 0a23 2323 2320 436f 6d6d 756e 6974  s..#### Communit
+00000750: 6965 730a 0a2d 205b 585d 205b 5246 4320  ies..- [X] [RFC 
+00000760: 3139 3737 5d28 6874 7470 733a 2f2f 6461  1977](https://da
+00000770: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
+00000780: 7267 2f64 6f63 2f68 746d 6c2f 7266 6331  rg/doc/html/rfc1
+00000790: 3937 3729 3a20 4247 5020 436f 6d6d 756e  977): BGP Commun
+000007a0: 6974 6965 7320 4174 7472 6962 7574 650a  ities Attribute.
+000007b0: 0a23 2323 2320 4578 7465 6e64 6564 2043  .#### Extended C
+000007c0: 6f6d 6d75 6e69 7469 6573 0a0a 2d20 5b58  ommunities..- [X
+000007d0: 5d20 5b52 4643 2034 3336 305d 2868 7474  ] [RFC 4360](htt
+000007e0: 7073 3a2f 2f64 6174 6174 7261 636b 6572  ps://datatracker
+000007f0: 2e69 6574 662e 6f72 672f 646f 632f 6874  .ietf.org/doc/ht
+00000800: 6d6c 2f72 6663 3433 3630 293a 2042 4750  ml/rfc4360): BGP
+00000810: 2045 7874 656e 6465 6420 436f 6d6d 756e   Extended Commun
+00000820: 6974 6965 7320 4174 7472 6962 7574 650a  ities Attribute.
+00000830: 2d20 5b58 5d20 5b52 4643 2035 3636 385d  - [X] [RFC 5668]
+00000840: 2868 7474 7073 3a2f 2f64 6174 6174 7261  (https://datatra
+00000850: 636b 6572 2e69 6574 662e 6f72 672f 646f  cker.ietf.org/do
+00000860: 632f 6874 6d6c 2f72 6663 3536 3638 293a  c/html/rfc5668):
+00000870: 2034 2d4f 6374 6574 2041 5320 5370 6563   4-Octet AS Spec
+00000880: 6966 6963 2042 4750 2045 7874 656e 6465  ific BGP Extende
+00000890: 6420 436f 6d6d 756e 6974 790a 2d20 5b58  d Community.- [X
+000008a0: 5d20 5b52 4643 2035 3730 315d 2868 7474  ] [RFC 5701](htt
+000008b0: 7073 3a2f 2f64 6174 6174 7261 636b 6572  ps://datatracker
+000008c0: 2e69 6574 662e 6f72 672f 646f 632f 6874  .ietf.org/doc/ht
+000008d0: 6d6c 2f72 6663 3537 3031 293a 2049 5076  ml/rfc5701): IPv
+000008e0: 3620 4164 6472 6573 7320 5370 6563 6966  6 Address Specif
+000008f0: 6963 2042 4750 2045 7874 656e 6465 6420  ic BGP Extended 
+00000900: 436f 6d6d 756e 6974 7920 4174 7472 6962  Community Attrib
+00000910: 7574 650a 2d20 5b58 5d20 5b52 4643 2037  ute.- [X] [RFC 7
+00000920: 3135 335d 2868 7474 7073 3a2f 2f64 6174  153](https://dat
+00000930: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
+00000940: 672f 646f 632f 6874 6d6c 2f72 6663 3731  g/doc/html/rfc71
+00000950: 3533 293a 2049 414e 4120 5265 6769 7374  53): IANA Regist
+00000960: 7269 6573 2066 6f72 2042 4750 2045 7874  ries for BGP Ext
+00000970: 656e 6465 6420 436f 6d6d 756e 6974 6965  ended Communitie
+00000980: 7320 5570 6461 7465 7320 3433 3630 2c20  s Updates 4360, 
+00000990: 3537 3031 0a2d 205b 585d 205b 5246 4320  5701.- [X] [RFC 
+000009a0: 3830 3937 5d28 6874 7470 733a 2f2f 6461  8097](https://da
+000009b0: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
+000009c0: 7267 2f64 6f63 2f68 746d 6c2f 7266 6338  rg/doc/html/rfc8
+000009d0: 3039 3729 3a20 4247 5020 5072 6566 6978  097): BGP Prefix
+000009e0: 204f 7269 6769 6e20 5661 6c69 6461 7469   Origin Validati
+000009f0: 6f6e 2053 7461 7465 2045 7874 656e 6465  on State Extende
+00000a00: 6420 436f 6d6d 756e 6974 790a 0a23 2323  d Community..###
+00000a10: 2320 4c61 7267 6520 436f 6d6d 756e 6974  # Large Communit
+00000a20: 6965 730a 0a2d 205b 585d 205b 5246 4320  ies..- [X] [RFC 
+00000a30: 3830 3932 5d28 6874 7470 733a 2f2f 6461  8092](https://da
+00000a40: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
+00000a50: 7267 2f64 6f63 2f68 746d 6c2f 7266 6338  rg/doc/html/rfc8
+00000a60: 3039 3229 3a20 4247 5020 4c61 7267 6520  092): BGP Large 
+00000a70: 436f 6d6d 756e 6974 6965 730a 0a23 2323  Communities..###
+00000a80: 204f 7468 6572 2049 6e66 6f72 6d61 7469   Other Informati
+00000a90: 6f6e 616c 0a0a 2d20 5b52 4643 2034 3338  onal..- [RFC 438
+00000aa0: 345d 2868 7474 7073 3a2f 2f64 6174 6174  4](https://datat
+00000ab0: 7261 636b 6572 2e69 6574 662e 6f72 672f  racker.ietf.org/
+00000ac0: 646f 632f 6874 6d6c 2f72 6663 3433 3834  doc/html/rfc4384
+00000ad0: 293a 2042 4750 2043 6f6d 6d75 6e69 7469  ): BGP Communiti
+00000ae0: 6573 2066 6f72 2044 6174 6120 436f 6c6c  es for Data Coll
+00000af0: 6563 7469 6f6e 2042 4350 2031 3134 0a2d  ection BCP 114.-
+00000b00: 205b 5246 4320 3831 3935 5d28 6874 7470   [RFC 8195](http
+00000b10: 733a 2f2f 6461 7461 7472 6163 6b65 722e  s://datatracker.
+00000b20: 6965 7466 2e6f 7267 2f64 6f63 2f68 746d  ietf.org/doc/htm
+00000b30: 6c2f 7266 6338 3139 3529 3a20 5573 6520  l/rfc8195): Use 
+00000b40: 6f66 2042 4750 204c 6172 6765 2043 6f6d  of BGP Large Com
+00000b50: 6d75 6e69 7469 6573 2028 696e 666f 726d  munities (inform
+00000b60: 6174 696f 6e61 6c29 0a2d 205b 5246 4320  ational).- [RFC 
+00000b70: 3836 3432 5d28 6874 7470 733a 2f2f 6461  8642](https://da
+00000b80: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
+00000b90: 7267 2f64 6f63 2f68 746d 6c2f 7266 6338  rg/doc/html/rfc8
+00000ba0: 3634 3229 3a20 506f 6c69 6379 2042 6568  642): Policy Beh
+00000bb0: 6176 696f 7220 666f 7220 5765 6c6c 2d4b  avior for Well-K
+00000bc0: 6e6f 776e 2042 4750 2043 6f6d 6d75 6e69  nown BGP Communi
+00000bd0: 7469 6573 0a0a 202a 2f0a 0a23 215b 616c  ties.. */..#![al
+00000be0: 6c6f 7728 6465 6164 5f63 6f64 6529 5d0a  low(dead_code)].
+00000bf0: 0a6d 6f64 2062 6770 3b0a 6d6f 6420 6572  .mod bgp;.mod er
+00000c00: 723b 0a6d 6f64 206d 7274 3b0a 6d6f 6420  r;.mod mrt;.mod 
+00000c10: 6e65 7477 6f72 6b3b 0a0a 7075 6220 7573  network;..pub us
+00000c20: 6520 6267 703a 3a2a 3b0a 7075 6220 7573  e bgp::*;.pub us
+00000c30: 6520 6572 723a 3a42 6770 4d6f 6465 6c73  e err::BgpModels
+00000c40: 4572 726f 723b 0a70 7562 2075 7365 206d  Error;.pub use m
+00000c50: 7274 3a3a 2a3b 0a70 7562 2075 7365 206e  rt::*;.pub use n
+00000c60: 6574 776f 726b 3a3a 2a3b 0a              etwork::*;.
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/capabilities.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/capabilities.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/community.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/community.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-use crate::network::Asn;
-use enum_primitive_derive::Primitive;
+use crate::models::Asn;
 use serde::Serialize;
 use std::fmt::Formatter;
 use std::net::{Ipv4Addr, Ipv6Addr};
 
 #[derive(Debug, PartialEq, Copy, Clone, Eq)]
 pub enum MetaCommunity {
     Community(Community),
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/elem.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/elem.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-use crate::bgp::attributes::{AsPath, AtomicAggregate, Origin};
-use crate::bgp::community::*;
-use crate::network::{Asn, NetworkPrefix};
+use crate::models::*;
 use itertools::Itertools;
 use serde::{Serialize, Serializer};
 use std::cmp::Ordering;
 use std::fmt::{Display, Formatter};
 use std::net::IpAddr;
 use std::str::FromStr;
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/error.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/error.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/mod.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/mod.rs`

 * *Files 22% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 pub mod attributes;
 pub mod capabilities;
 pub mod community;
 pub mod elem;
 pub mod error;
 pub mod role;
 
-pub use crate::bgp::attributes::*;
-pub use crate::bgp::capabilities::*;
-pub use crate::bgp::community::*;
-pub use crate::bgp::elem::*;
-pub use crate::bgp::error::*;
-pub use crate::bgp::role::*;
+pub use attributes::*;
+pub use capabilities::*;
+pub use community::*;
+pub use elem::*;
+pub use error::*;
+pub use role::*;
 
-use crate::bgp::capabilities::BgpCapabilityType;
-use crate::bgp::error::BgpError;
-use crate::network::*;
+use crate::models::network::*;
+use capabilities::BgpCapabilityType;
+use error::BgpError;
 use serde::Serialize;
 use std::net::Ipv4Addr;
 
 #[derive(Debug, Primitive, Copy, Clone, Serialize, PartialEq)]
 pub enum BgpMessageType {
     OPEN = 1,
     UPDATE = 2,
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/bgp/role.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/bgp/role.rs`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
-    use crate::bgp::BgpRole::*;
+    use crate::models::BgpRole::*;
 
     #[test]
     fn test_bgp_role_validation() {
         let mut local: BgpRole;
         let mut remote: BgpRole;
 
         local = Provider;
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/err.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/err.rs`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/mrt/bgp4mp.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/bgp4mp.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 //! MRT BGP4MP structs
-use crate::bgp::BgpMessage;
-use crate::network::{Afi, Asn};
+use crate::models::*;
 use serde::Serialize;
 use std::net::IpAddr;
 
 /// BGP states enum.
 #[derive(Debug, Primitive, Copy, Clone, Serialize, PartialEq, Eq)]
 pub enum BgpState {
     Idle = 1,
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/mrt/mod.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 //! MRT message and relevant structs.
 
 pub mod bgp4mp;
 pub mod tabledump;
 
-pub use crate::mrt::bgp4mp::*;
-pub use crate::mrt::tabledump::*;
+pub use bgp4mp::*;
 use serde::Serialize;
 use std::io;
 use std::io::Write;
+pub use tabledump::*;
 
 /// MrtRecord is a wrapper struct that contains a header and a message.
 ///
 /// A MRT record is constructed as the following:
 /// ```text
 ///  0                   1                   2                   3
 ///  0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
```

### Comparing `pybgpkit_parser-0.4.1/local_dependencies/bgp-models/src/mrt/tabledump.rs` & `pybgpkit_parser-0.4.2/local_dependencies/bgpkit-parser/src/models/mrt/tabledump.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 //! MRT table dump version 1 and 2 structs
-use crate::bgp::Attribute;
-use crate::network::{Afi, Asn, NetworkPrefix, Safi};
+use crate::models::*;
 use serde::Serialize;
 use std::collections::HashMap;
 use std::net::{IpAddr, Ipv4Addr};
 
 /// TableDump message version 1
 #[derive(Debug, Clone, Serialize, PartialEq, Eq)]
 pub struct TableDumpMessage {
```

### Comparing `pybgpkit_parser-0.4.1/Cargo.toml` & `pybgpkit_parser-0.4.2/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [package]
 name = "pybgpkit-parser"
 description = "BGPKIT Parser Python Binding"
 keywords = ["bgp", "mrt", "parser"]
 repository = "https://github.com/bgpkit/bgpkit-parser/tree/main/bgpkit-parser-py"
 documentation = "https://github.com/bgpkit/bgpkit-parser/blob/main/bgpkit-parser-py/README.md"
-version = "0.4.1"
+version = "0.4.2"
 authors = ["Mingwei Zhang <mingwei@bgpkit.com>"]
 edition = "2021"
 license = "MIT"
 readme = "README.md"
 
 [lib]
 name = "pybgpkit_parser"
```

### Comparing `pybgpkit_parser-0.4.1/Dockerfile` & `pybgpkit_parser-0.4.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/LICENSE` & `pybgpkit_parser-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/README.md` & `pybgpkit_parser-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/src/lib.rs` & `pybgpkit_parser-0.4.2/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use bgpkit_parser::models::*;
 use bgpkit_parser::*;
 use dict_derive::{FromPyObject, IntoPyObject};
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use std::collections::HashMap;
 use std::io::Read;
```

### Comparing `pybgpkit_parser-0.4.1/Cargo.lock` & `pybgpkit_parser-0.4.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `pybgpkit_parser-0.4.1/PKG-INFO` & `pybgpkit_parser-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpkit-parser
-Version: 0.4.1
+Version: 0.4.2
 Summary: BGPKIT Parser Python Binding
 Keywords: bgp,mrt,parser
 Author: Mingwei Zhang <mingwei@bgpkit.com>
 Author-email: Mingwei Zhang <mingwei@bgpkit.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/bgpkit/bgpkit-parser/tree/main/bgpkit-parser-py
```

