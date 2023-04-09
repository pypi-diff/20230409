# Comparing `tmp/twnet_parser-0.3.3.tar.gz` & `tmp/twnet_parser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twnet_parser-0.3.3.tar", last modified: Fri Apr  7 08:32:30 2023, max compression
+gzip compressed data, was "twnet_parser-0.4.0.tar", last modified: Sun Apr  9 14:27:20 2023, max compression
```

## Comparing `twnet_parser-0.3.3.tar` & `twnet_parser-0.4.0.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.359722 twnet_parser-0.3.3/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.3.3/LICENSE.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3845 2023-04-07 08:32:30.359722 twnet_parser-0.3.3/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3112 2023-04-07 07:40:28.000000 twnet_parser-0.3.3/README.md
--rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.3.3/pyproject.toml
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.349722 twnet_parser-0.3.3/scripts/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)    18321 2023-04-02 18:03:38.000000 twnet_parser-0.3.3/scripts/generate_messages.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-04-07 08:32:30.359722 twnet_parser-0.3.3/setup.cfg
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.349722 twnet_parser-0.3.3/tests/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.3.3/tests/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      693 2023-04-02 18:23:19.000000 twnet_parser-0.3.3/tests/control_packets7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9627 2023-04-06 15:42:28.000000 twnet_parser-0.3.3/tests/ctrl_packets_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-03-19 15:03:24.000000 twnet_parser-0.3.3/tests/int_packer_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.3.3/tests/invalid_packet_header7_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.349722 twnet_parser-0.3.3/tests/msg7/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.3.3/tests/msg7/sv_tune_params_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      716 2023-03-25 13:15:25.000000 twnet_parser-0.3.3/tests/packet_header6_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2118 2023-04-02 18:06:01.000000 twnet_parser-0.3.3/tests/packet_header7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.3.3/tests/packet_invalid_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.3.3/tests/packet_with_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.3.3/tests/repack_chunks7_test.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2525 2023-03-26 09:59:51.000000 twnet_parser-0.3.3/tests/unpacker_state_test.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.349722 twnet_parser-0.3.3/twnet_parser/
--rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/__init__.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      991 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/chunk_header.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      207 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/ctrl_message.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.349722 twnet_parser-0.3.3/twnet_parser/external/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/external/huffman.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/message_parser.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.346389 twnet_parser-0.3.3/twnet_parser/messages7/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.353056 twnet_parser-0.3.3/twnet_parser/messages7/control/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      317 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/control/accept.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      811 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/control/close.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      579 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/control/connect.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      303 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/control/keep_alive.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      716 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/control/token.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.356389 twnet_parser-0.3.3/twnet_parser/messages7/game/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1273 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_call_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      982 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_command.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      854 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      577 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_kill.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      592 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_ready_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1131 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_say.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1049 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_set_spectator_mode.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      833 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_set_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1335 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1770 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_start_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      803 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/cl_vote.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1148 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/de_client_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1143 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/de_client_leave.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      836 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_broadcast.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1305 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_chat.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      815 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_checkpoint.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1154 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_client_drop.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     2385 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_client_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1166 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_command_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      839 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_command_info_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1011 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_emoticon.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      890 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_extra_projectile.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1528 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_game_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      584 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_game_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1276 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_kill_msg.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      826 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_motd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1491 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_race_finish.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      595 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_ready_to_enter.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1703 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_server_settings.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1492 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_skin_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1313 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_team.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7501 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_tune_params.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      603 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_clear_options.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      866 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_option_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      606 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_option_list_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      872 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_option_remove.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1472 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_set.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1207 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_status.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      853 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/game/sv_weapon_pickup.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.356389 twnet_parser-0.3.3/twnet_parser/messages7/system/
--rw-r--r--   0 chiller   (1000) chiller   (1000)      580 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/con_ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      582 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/enter_game.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1237 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1349 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/input.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1024 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/input_timing.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1656 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/map_change.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      763 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      829 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/maplist_entry_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      829 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/maplist_entry_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      571 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/ping.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      582 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/ping_reply.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      834 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_auth.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      587 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_auth_off.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      585 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_auth_on.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      807 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_cmd.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1109 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_cmd_add.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      819 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_cmd_rem.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      814 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_line.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      573 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/ready.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      593 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/request_map_data.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      769 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/server_info.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1507 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/snap.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      970 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/snap_empty.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1231 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/messages7/system/snap_single.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1784 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/msg7.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.356389 twnet_parser-0.3.3/twnet_parser/msg_matcher/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/msg_matcher/control7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/msg_matcher/game7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/msg_matcher/system7.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      275 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/net_message.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3295 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/packer.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)     6164 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/packet.py
--rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.3.3/twnet_parser/pretty_print.py
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.349722 twnet_parser-0.3.3/twnet_parser.egg-info/
--rw-r--r--   0 chiller   (1000) chiller   (1000)     3845 2023-04-07 08:32:30.000000 twnet_parser-0.3.3/twnet_parser.egg-info/PKG-INFO
--rw-r--r--   0 chiller   (1000) chiller   (1000)     4260 2023-04-07 08:32:30.000000 twnet_parser-0.3.3/twnet_parser.egg-info/SOURCES.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-04-07 08:32:30.000000 twnet_parser-0.3.3/twnet_parser.egg-info/dependency_links.txt
--rw-r--r--   0 chiller   (1000) chiller   (1000)       31 2023-04-07 08:32:30.000000 twnet_parser-0.3.3/twnet_parser.egg-info/top_level.txt
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.346389 twnet_parser-0.3.3/venv/
-drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:32:30.359722 twnet_parser-0.3.3/venv/bin/
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2html.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2html4.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2html5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2latex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2man.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2odt.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2s5.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2xetex.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rst2xml.py
--rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-03-16 13:39:00.000000 twnet_parser-0.3.3/venv/bin/rstpep2html.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1324 2023-03-16 13:24:33.000000 twnet_parser-0.4.0/LICENSE.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4557 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     3824 2023-04-09 14:22:31.000000 twnet_parser-0.4.0/README.md
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       86 2023-04-07 08:04:33.000000 twnet_parser-0.4.0/pyproject.toml
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.143050 twnet_parser-0.4.0/scripts/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)    23744 2023-04-09 10:11:42.000000 twnet_parser-0.4.0/scripts/generate_messages.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      857 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/setup.cfg
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/tests/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-03-16 11:52:21.000000 twnet_parser-0.4.0/tests/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      658 2023-04-09 13:58:10.000000 twnet_parser-0.4.0/tests/control_packets7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)    12270 2023-04-07 08:45:32.000000 twnet_parser-0.4.0/tests/ctrl_packets_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     3748 2023-03-19 15:03:24.000000 twnet_parser-0.4.0/tests/int_packer_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      289 2023-04-02 18:22:11.000000 twnet_parser-0.4.0/tests/invalid_packet_header7_test.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/tests/msg7/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     5391 2023-04-02 09:51:19.000000 twnet_parser-0.4.0/tests/msg7/sv_tune_params_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      679 2023-04-09 13:57:19.000000 twnet_parser-0.4.0/tests/packet_header6_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9551 2023-04-09 14:21:22.000000 twnet_parser-0.4.0/tests/packet_header7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      998 2023-04-02 18:06:01.000000 twnet_parser-0.4.0/tests/packet_invalid_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     9723 2023-04-02 08:23:56.000000 twnet_parser-0.4.0/tests/packet_with_chunks7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2942 2023-03-31 07:31:27.000000 twnet_parser-0.4.0/tests/repack_chunks7_test.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     6760 2023-04-09 10:11:10.000000 twnet_parser-0.4.0/tests/unpacker_state_test.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/twnet_parser/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        0 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/__init__.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      991 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/chunk_header.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       25 2023-04-09 13:43:44.000000 twnet_parser-0.4.0/twnet_parser/constants.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      207 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/ctrl_message.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/twnet_parser/external/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     8373 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/external/huffman.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      629 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/message_parser.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.143050 twnet_parser-0.4.0/twnet_parser/messages7/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/twnet_parser/messages7/control/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      317 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/accept.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      811 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/close.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      579 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/connect.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      303 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/keep_alive.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      716 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/messages7/control/token.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.153049 twnet_parser-0.4.0/twnet_parser/messages7/game/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1319 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_call_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1017 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_command.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      854 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      577 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_kill.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      592 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_ready_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1155 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_say.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1049 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_set_spectator_mode.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      833 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_set_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1689 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2136 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_start_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      803 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/cl_vote.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1172 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/de_client_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1178 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/de_client_leave.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      836 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_broadcast.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1329 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_chat.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      815 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_checkpoint.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1178 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_client_drop.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     2751 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_client_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1212 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_command_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      863 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_command_info_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1011 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_emoticon.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      890 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_extra_projectile.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1528 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_game_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      584 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_game_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1276 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_kill_msg.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      826 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_motd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1491 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_race_finish.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      595 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_ready_to_enter.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1703 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_server_settings.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1846 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_skin_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1313 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_team.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7501 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_tune_params.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      603 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_clear_options.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      890 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      606 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_list_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      896 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_remove.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1507 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_set.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1207 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_status.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      853 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/game/sv_weapon_pickup.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/twnet_parser/messages7/system/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      580 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/con_ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      582 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/enter_game.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1201 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1349 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/input.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1024 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/input_timing.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1656 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/map_change.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      763 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      829 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/maplist_entry_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      829 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/maplist_entry_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      571 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/ping.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      582 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/ping_reply.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      834 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      587 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth_off.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      585 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth_on.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      807 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1109 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd_add.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      819 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd_rem.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      814 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_line.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      573 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/ready.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      593 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/request_map_data.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      769 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/server_info.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1747 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/snap.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      970 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/snap_empty.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1471 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/messages7/system/snap_single.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1784 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/msg7.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/twnet_parser/msg_matcher/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     1089 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/msg_matcher/control7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7692 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/msg_matcher/game7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4599 2023-04-09 09:17:19.000000 twnet_parser-0.4.0/twnet_parser/msg_matcher/system7.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      275 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/net_message.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4586 2023-04-07 12:26:53.000000 twnet_parser-0.4.0/twnet_parser/packer.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     7318 2023-04-09 14:18:13.000000 twnet_parser-0.4.0/twnet_parser/packet.py
+-rw-r--r--   0 chiller   (1000) chiller   (1000)      222 2023-04-07 08:13:33.000000 twnet_parser-0.4.0/twnet_parser/pretty_print.py
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.146383 twnet_parser-0.4.0/twnet_parser.egg-info/
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4557 2023-04-09 14:27:20.000000 twnet_parser-0.4.0/twnet_parser.egg-info/PKG-INFO
+-rw-r--r--   0 chiller   (1000) chiller   (1000)     4286 2023-04-09 14:27:20.000000 twnet_parser-0.4.0/twnet_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)        1 2023-04-09 14:27:20.000000 twnet_parser-0.4.0/twnet_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 chiller   (1000) chiller   (1000)       31 2023-04-09 14:27:20.000000 twnet_parser-0.4.0/twnet_parser.egg-info/top_level.txt
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.143050 twnet_parser-0.4.0/venv/
+drwxr-xr-x   0 chiller   (1000) chiller   (1000)        0 2023-04-09 14:27:20.156383 twnet_parser-0.4.0/venv/bin/
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      630 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      752 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1097 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      829 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      652 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      818 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)     1756 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      637 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      673 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      909 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      638 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 chiller   (1000) chiller   (1000)      706 2023-03-16 13:39:00.000000 twnet_parser-0.4.0/venv/bin/rstpep2html.py
```

### Comparing `twnet_parser-0.3.3/LICENSE.txt` & `twnet_parser-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/PKG-INFO` & `twnet_parser-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: twnet_parser
-Version: 0.3.3
-Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
-Home-page: https://gitlab.com/teeworlds-network/twnet_parser
-Author: ChillerDragon
-Author-email: chillerdragon@gmail.com
-License: BSD-2.0
-Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
-Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 
 # THIS LIBRARY IS IN EARLY DEVELOPMENT
 
 ## Do not get bamboozled by the mature looking readme!
 ## This project is not in a very usable state yet. It is in very early development!
 ## APIs might change and many essential features are missing!
@@ -46,36 +29,49 @@
 
 ## Features
 
 | Feature                        | Status             |
 | ------------------------------ | ------------------ |
 | Deserialize 0.7 packet headers | :heavy_check_mark: |
 | Deserialize 0.7 chunk headers  | :heavy_check_mark: |
-| Deserialize 0.7 messages       | 70%                |
+| Deserialize 0.7 messages       | 80%                |
 | Deserialize 0.7 snapshots      |                    |
-| Serialize 0.7 packet headers   |                    |
+| Serialize 0.7 packet headers   | :heavy_check_mark: |
 | Serialize 0.7 chunk headers    |                    |
-| Serialize 0.7 messages         | 70%                |
+| Serialize 0.7 messages         | 80%                |
 | Deserialize 0.6 packet headers |                    |
 | Deserialize 0.6 chunk headers  |                    |
 | Deserialize 0.6 messages       |                    |
 | Deserialize 0.6 snapshots      |                    |
 | Serialize 0.6 packet headers   |                    |
 | Serialize 0.6 chunk headers    |                    |
 | Serialize 0.6 messages         |                    |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
+| Track sequence number state    | :x:     | TODO: link if someone implemented it on top |
+| Track connection state         | :x:     | TODO: link if someone implemented it on top |
 
 Look elsewhere for these features. Or use this library to implement them on top.
 
+This project is intentionally only covering parsing the protocol.
+Not fully implemeting a state machine of the protocol.
+Or a fully working client / server software.
+
+If you want to build something with this library
+you do have to understand how the protocol works
+and when the client and server have to send what.
+
+This [protocol documentation](https://chillerdragon.github.io/teeworlds-protocol/index.html)
+should get you started to understand the basics.
+
 ## development setup
 
 ```bash
 git clone https://gitlab.com/teeworlds-network/twnet_parser
 cd twnet_parser
 python -m venv venv
 source venv/bin/activate
@@ -92,14 +88,17 @@
 pytest .
 
 # run style linter
 pylint src/
 
 # run type checker
 mypy src/
+
+# or use the bundle script that runs all tests
+./scripts/run_tests.sh
 ```
 
 ## package and release
 
 ```bash
 # manual
 pip install -r requirements/dev.txt
```

### Comparing `twnet_parser-0.3.3/scripts/generate_messages.py` & `twnet_parser-0.4.0/scripts/generate_messages.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 #!/usr/bin/env python3
 
 import os
 import json
 
 from typing import TypedDict, Literal, Optional, Dict, Union
 
-class ConstantJson(TypedDict):
-    name: list[str]
-    type: str
-    value: int
-
-class NetEnumValuesJson(TypedDict):
-    value: str
-    name: list[str]
-
-class NetEnumJson(TypedDict):
-    name: list[str]
-    values: list[NetEnumValuesJson]
-
-class InnerNetMessageMemberTypeJson(TypedDict):
-    # TODO: define this literal as type
-    #       so it can be reused
-    kind: Literal[ \
+KIND = Literal[ \
             'int32', \
             'tick', \
             'string', \
             'raw', \
             'sha256', \
             'data', \
             'rest', \
             'enum', \
             'boolean', \
             'tune_param', \
             'snapshot_object', \
             'array', \
             'flags', \
             'optional']
+
+class ConstantJson(TypedDict):
+    name: list[str]
+    type: str
+    value: int
+
+class NetEnumValuesJson(TypedDict):
+    value: str
+    name: list[str]
+
+class NetEnumJson(TypedDict):
+    name: list[str]
+    values: list[NetEnumValuesJson]
+
+class InnerNetMessageMemberTypeJson(TypedDict):
+    kind: KIND
+    disallow_cc: bool
+
+class ArrayMemberTypeJson(TypedDict):
+    kind: KIND
+    # strings
     disallow_cc: bool
 
 class NetMessageMemberTypeJson(TypedDict):
-    kind: Literal[ \
-            'int32', \
-            'tick', \
-            'string', \
-            'raw', \
-            'sha256', \
-            'data', \
-            'rest', \
-            'enum', \
-            'boolean', \
-            'tune_param', \
-            'snapshot_object', \
-            'array', \
-            'flags', \
-            'optional']
+    kind: KIND
     inner: InnerNetMessageMemberTypeJson
+    # strings
     disallow_cc: bool
 
+    # arrays
+    count: int
+    member_type: ArrayMemberTypeJson
+
+    # data
+    size: Literal['specified_before']
+
 class NetMessageMemberJson(TypedDict):
     name: list[str]
     type: NetMessageMemberTypeJson
 
 class NetMessageJson(TypedDict):
     id: int
     name: list[str]
@@ -168,21 +167,28 @@
         out_file.write('    def __init__(\n')
         out_file.write('            self,\n')
         args: list[str] = []
         for member in msg['members']:
             # {'name': ['message'], 'type': {'kind': 'string', 'disallow_cc': False}} 
             ftype = 'int'
             default = '-1'
-            if member['type']['kind'] == 'string': # TODO: sanitize cc
+            if member['type']['kind'] == 'string':
                 ftype = 'str'
                 default = "'default'"
             elif member['type']['kind'] in \
-                ('raw', 'sha256', 'rest', 'data'): # TODO: data has a size field
+                ('raw', 'sha256', 'rest'): # TODO: rest sha256 and raw
+                ftype = 'bytes'
+                default = "b'\\x00'"
+            elif member['type']['kind'] == 'data':
                 ftype = 'bytes'
                 default = "b'\\x00'"
+                if member['type']['size'] == 'specified_before':
+                    args.append('            data_size: Optional[int] = None')
+                else:
+                    raise ValueError(f"Error: unknown data size {member['type']}")
             # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
             elif member['type']['kind'] == 'enum':
                 ftype = 'int'
                 default = '0'
                 # TODO: use ENUM_NAME_SOME_VALUE as default here
             elif member['type']['kind'] in ('int32', 'tick'):
                 ftype = 'int'
@@ -193,22 +199,42 @@
             elif member['type']['kind'] == 'tune_param':
                 ftype = 'float'
                 default = '0.0'
             elif member['type']['kind'] == 'snapshot_object':
                 # TODO: think about snapshot_object
                 ftype = 'int'
                 default = '0'
-            elif member['type']['kind'] == 'array': # TODO: think about array
-                ftype = 'int'
-                default = '0'
+            elif member['type']['kind'] == 'array':
+                size: int = member['type']['count']
+                if size is None:
+                    print("Error: size is none for the following message")
+                    print(msg)
+                    exit(1)
+                arr_member: ArrayMemberTypeJson = member['type']['member_type']
+                if arr_member['kind'] == 'string':
+                    ftype = f'Annotated[list[str], {size}]'
+                    default = '[' + ', '.join(["''"] * size) + ']'
+                elif arr_member['kind'] == 'boolean':
+                    ftype = f'Annotated[list[bool], {size}]'
+                    default = '[' + ', '.join(["False"] * size) + ']'
+                elif arr_member['kind'] in ('int32', 'tick', 'enum'):
+                    ftype = f'Annotated[list[int], {size}]'
+                    default = '[' + ', '.join(["0"] * size) + ']'
+                else:
+                    raise ValueError( \
+                        f"Error: unknown array member type {member['type']}")
+                # Initializing lists with defaults
+                # And type annotation can get quite long
+                # So split it in two lines
+                default = f'\\\n                {default}'
             elif member['type']['kind'] == 'flags': # TODO: think about flags
                 ftype = 'int'
                 default = '0'
             elif member['type']['kind'] == 'optional':
-                if member['type']['inner']['kind'] == 'string': # TODO: sanitize cc
+                if member['type']['inner']['kind'] == 'string':
                     ftype = 'str'
                     default = "''"
                 elif member['type']['inner']['kind'] in ('int32', 'tick'):
                     ftype = 'int'
                     default = '0'
                 else:
                     raise ValueError(f"Error: unknown optional type {member['type']}")
@@ -228,157 +254,255 @@
         out_file.write('\n')
         for member in msg['members']:
             # {'name': ['message'], 'type': {'kind': 'string', 'disallow_cc': False}} 
             ftype = 'int'
             if member['type']['kind'] == 'string':
                 ftype = 'str'
             elif member['type']['kind'] in \
-                ('raw', 'sha256', 'rest', 'data'): # TODO: data has a size field
+                    ('raw', 'sha256', 'rest'): # TODO: sha256 and raw
+                ftype = 'bytes'
+            elif member['type']['kind'] == 'data':
                 ftype = 'bytes'
+                if member['type']['size'] == 'specified_before':
+                    out_file.write("        " \
+                        "self.data_size: int = data_size if data_size else len(data)\n")
+                else:
+                    raise ValueError(f"Error: unknown data size {member['type']}")
             # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
             elif member['type']['kind'] == 'enum':
                 ftype = 'int'
             elif member['type']['kind'] in ('int32', 'tick'):
                 ftype = 'int'
             elif member['type']['kind'] == 'boolean':
                 ftype = 'bool'
             elif member['type']['kind'] == 'tune_param':
                 ftype = 'float'
             elif member['type']['kind'] == 'snapshot_object':
                 # TODO: think about snapshot_object
                 ftype = 'int'
-            elif member['type']['kind'] == 'array': # TODO: think about array
-                ftype = 'int'
+            elif member['type']['kind'] == 'array':
+                # Array type annotations are so annoyingly long
+                # also there is a planned refactor
+                # https://gitlab.com/teeworlds-network/twnet_parser/-/issues/4
+                # so inherit type from constructor arguments
+                ftype = ''
             elif member['type']['kind'] == 'flags': # TODO: think about flags
                 ftype = 'int'
             elif member['type']['kind'] == 'optional':
-                if member['type']['inner']['kind'] == 'string': # TODO: sanitize cc
+                if member['type']['inner']['kind'] == 'string':
                     ftype = 'str'
                 elif member['type']['inner']['kind'] in ('int32', 'tick'):
                     ftype = 'int'
                 else:
                     raise ValueError(f"Error: unknown optional type {member['type']}")
             else:
                 raise ValueError(f"Error: unknown type {member['type']}")
             name = name_to_snake(member["name"])
-            out_file.write(f"        self.{name}: {ftype} = {name}\n")
+            if ftype != '':
+                ftype = f': {ftype}'
+            out_file.write(f"        self.{name}{ftype} = {name}\n")
         out_file.write('\n')
         out_file.write('    # first byte of data\n')
         out_file.write('    # has to be the first byte of the message payload\n')
         out_file.write('    # NOT the chunk header and NOT the message id\n')
         out_file.write('    def unpack(self, data: bytes) -> bool:\n')
         if len(msg['members']) > 0:
             out_file.write('        unpacker = Unpacker(data)\n')
-        for member in msg['members']:
-            # {'name': ['message'], 'type': {'kind': 'string', 'disallow_cc': False}} 
-            unpacker = 'int()'
-            if member['type']['kind'] == 'string': # TODO: sanitize cc
+        out_file.write(gen_unpack_members(msg))
+        out_file.write('        return True\n')
+        out_file.write('\n')
+        out_file.write('    def pack(self) -> bytes:\n')
+        out_file.write(gen_pack_return(msg))
+
+def gen_unpack_members(msg: NetMessageJson) -> str:
+    res: str = ''
+    for member in msg['members']:
+        # {'name': ['message'], 'type': {'kind': 'string', 'disallow_cc': False}} 
+        unpacker = 'int()'
+        if member['type']['kind'] == 'string':
+            if member['type']['disallow_cc']:
+                unpacker = 'str(SANITIZE_CC)'
+            else:
                 unpacker = 'str()'
-            elif member['type']['kind'] in \
-                ('raw', 'sha256', 'rest', 'data'): # TODO: data has a size field
-                unpacker = 'raw()'
-            # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
-            elif member['type']['kind'] == 'enum':
+        elif member['type']['kind'] in \
+            ('raw', 'sha256', 'rest'): # TODO: do we need to fix size for sha256?
+            unpacker = 'raw()'
+        elif member['type']['kind'] == 'data':
+            if member['type']['size'] == 'specified_before':
+                res += '        self.data_size = unpacker.get_int()\n'
+                unpacker = 'raw(self.data_size)'
+            else:
+                raise ValueError(f"Error: unknown data size {member['type']}")
+        # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
+        elif member['type']['kind'] == 'enum':
+            unpacker = 'int() # TODO: this is a enum'
+        elif member['type']['kind'] in ('int32', 'tick'):
+            unpacker = 'int()'
+        elif member['type']['kind'] == 'boolean':
+            unpacker = 'int() == 1'
+        elif member['type']['kind'] == 'tune_param':
+            unpacker = 'int() / 100.0'
+        elif member['type']['kind'] == 'snapshot_object':
+            # TODO: think about snapshot_object
+            unpacker = 'int() # TODO: this is a snapshot object'
+        elif member['type']['kind'] == 'array':
+            size: int = member['type']['count']
+            if size is None:
+                print("Error: size is none for the following message")
+                print(msg)
+                exit(1)
+            arr_member: ArrayMemberTypeJson = member['type']['member_type']
+            if arr_member['kind'] == 'string':
+                if arr_member['disallow_cc']:
+                    unpacker = 'str(SANITIZE_CC)'
+                else:
+                    unpacker = 'str()'
+            elif arr_member['kind'] == 'enum':
                 unpacker = 'int() # TODO: this is a enum'
-            elif member['type']['kind'] in ('int32', 'tick'):
-                unpacker = 'int()'
-            elif member['type']['kind'] == 'boolean':
+            elif arr_member['kind'] == 'boolean':
                 unpacker = 'int() == 1'
-            elif member['type']['kind'] == 'tune_param':
-                unpacker = 'int() / 100.0'
-            elif member['type']['kind'] == 'snapshot_object':
-                # TODO: think about snapshot_object
-                unpacker = 'int() # TODO: this is a snapshot object'
-            elif member['type']['kind'] == 'array': # TODO: think about array
-                unpacker = 'int() # TODO: this is an array'
-            elif member['type']['kind'] == 'flags': # TODO: think about flags
-                unpacker = 'int() # TODO: this is a flag'
-            elif member['type']['kind'] == 'optional':
-                # TODO: unpacker should not crash on missing optional fields
-                #       check how tw code does it and be smart here
-                if member['type']['inner']['kind'] == 'string': # TODO: sanitize cc
-                    unpacker = 'str() # TODO: this can fail for optionals'
-                elif member['type']['inner']['kind'] in ('int32', 'tick'):
-                    unpacker = 'int() # TODO: this can fail for optionals'
+            elif arr_member['kind'] in ('int32', 'tick'):
+                unpacker = 'int()'
             else:
-                raise ValueError(f"Error: unknown type {member['type']}")
+                raise ValueError(f"Error: unknown array member type {member['type']}")
             name = name_to_snake(member["name"])
-            out_file.write(f'        self.{name} = unpacker.get_{unpacker}\n')
-        out_file.write('        return True\n')
-        out_file.write('\n')
-        out_file.write('    def pack(self) -> bytes:\n')
-        out_file.write(gen_pack_return(msg))
+            res += f'        for i in range(0, {size}):\n'
+            res += f'            self.{name}[i] = unpacker.get_{unpacker}\n'
+            continue
+        elif member['type']['kind'] == 'flags': # TODO: think about flags
+            unpacker = 'int() # TODO: this is a flag'
+        elif member['type']['kind'] == 'optional':
+            # TODO: unpacker should not crash on missing optional fields
+            #       check how tw code does it and be smart here
+            if member['type']['inner']['kind'] == 'string':
+                if member['type']['inner']['disallow_cc']:
+                    unpacker = 'str(SANITIZE_CC)'
+                    unpacker += ' # TODO: optionals'
+                else:
+                    unpacker = 'str() # TODO: optionals'
+            elif member['type']['inner']['kind'] in ('int32', 'tick'):
+                unpacker = 'int() # TODO: optionals'
+        else:
+            raise ValueError(f"Error: unknown type {member['type']}")
+        name = name_to_snake(member["name"])
+        res += f'        self.{name} = unpacker.get_{unpacker}\n'
+    return res
 
 def get_dependencies(msg: NetMessageJson) -> str:
     packer_deps: list[str] = []
+    typing_deps: list[str] = []
     for member in msg['members']:
-        if member['type']['kind'] == 'string': # TODO: sanitize cc
+        if member['type']['kind'] == 'string':
             packer_deps.append('pack_str')
+            if member['type']['disallow_cc']:
+                packer_deps.append('SANITIZE_CC')
         elif member['type']['kind'] in \
-            ('raw', 'sha256', 'rest', 'data'): # TODO: data has a size field
+            ('raw', 'sha256', 'rest'):
             pass
+        elif member['type']['kind'] == 'data':
+            if member['type']['size'] == 'specified_before':
+                typing_deps.append('Optional')
+            else:
+                raise ValueError(f"Error: unknown data size {member['type']}")
         # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
         elif member['type']['kind'] == 'enum':
             packer_deps.append('pack_int')
         elif member['type']['kind'] in ('int32', 'tick'):
             packer_deps.append('pack_int')
         elif member['type']['kind'] == 'boolean':
             packer_deps.append('pack_int')
         elif member['type']['kind'] == 'tune_param':
             packer_deps.append('pack_int')
         elif member['type']['kind'] == 'snapshot_object':
             # TODO: think about snapshot_object
             packer_deps.append('pack_int')
-        elif member['type']['kind'] == 'array': # TODO: think about array
+        elif member['type']['kind'] == 'array':
             packer_deps.append('pack_int')
+            typing_deps.append('Annotated')
+            arr_member: ArrayMemberTypeJson = member['type']['member_type']
+            if arr_member['kind'] == 'string':
+                packer_deps.append('pack_str')
+                if arr_member['disallow_cc']:
+                    packer_deps.append('SANITIZE_CC')
+            elif arr_member['kind'] == 'enum':
+                packer_deps.append('pack_int')
+            elif arr_member['kind'] == 'boolean':
+                packer_deps.append('pack_int')
+            elif arr_member['kind'] in ('int32', 'tick'):
+                packer_deps.append('pack_int')
+            else:
+                raise ValueError(f"Error: unknown array member type {member['type']}")
         elif member['type']['kind'] == 'flags': # TODO: think about flags
             packer_deps.append('pack_int')
         elif member['type']['kind'] == 'optional':
             if member['type']['inner']['kind'] == 'string':
                 packer_deps.append('pack_str')
+                if member['type']['inner']['disallow_cc']:
+                    packer_deps.append('SANITIZE_CC')
             elif member['type']['inner']['kind'] in ('int32', 'tick'):
                 packer_deps.append('pack_int')
         else:
             raise ValueError(f"Error: unknown type {member['type']}")
-    if len(packer_deps) == 0:
-        return ''
-    return 'from twnet_parser.packer import ' + \
-        ', '.join(sorted(set(packer_deps))) + '\n'
+    res: str = ''
+    if len(packer_deps) > 0:
+        res += 'from twnet_parser.packer import ' + \
+            ', '.join(sorted(set(packer_deps))) + '\n'
+    if len(typing_deps) > 0:
+        res += 'from typing import ' + \
+            ', '.join(sorted(set(typing_deps))) + '\n'
+    return res
 
 def pack_field(member: NetMessageMemberJson) -> str:
     name: str = name_to_snake(member["name"])
     field: str = f'self.{name}'
     packer = 'int'
-    if member['type']['kind'] == 'string': # TODO: sanitize cc
+    if member['type']['kind'] == 'string':
         packer = 'str'
     elif member['type']['kind'] in \
-        ('raw', 'sha256', 'rest', 'data'): # TODO: data has a size field
+        ('raw', 'sha256', 'rest'): # TODO: raw sha256 rest
         return f'self.{name}'
+    elif member['type']['kind'] == 'data':
+        if member['type']['size'] == 'specified_before':
+            return f'pack_int(self.data_size) + \\\n' \
+                f'            self.{name}'
+        else:
+            raise ValueError(f"Error: unknown data size {member['type']}")
     # {"name": ["mode"], "type": {"kind": "enum", "enum": ["chat"]}},
     elif member['type']['kind'] == 'enum':
         packer = 'int'
     elif member['type']['kind'] in ('int32', 'tick'):
         packer = 'int'
     elif member['type']['kind'] == 'boolean':
         packer = 'int'
     elif member['type']['kind'] == 'tune_param':
         packer = 'int'
         field = f'int({field} * 100.0)'
     elif member['type']['kind'] == 'snapshot_object':
         # TODO: think about snapshot_object
         packer = 'int'
-    elif member['type']['kind'] == 'array': # TODO: think about array
-        packer = 'int'
+    elif member['type']['kind'] == 'array':
+        arr_member: ArrayMemberTypeJson = member['type']['member_type']
+        if arr_member['kind'] == 'string':
+           packer = 'str'
+        elif arr_member['kind'] == 'enum':
+           packer = 'int'
+        elif arr_member['kind'] == 'boolean':
+           packer = 'int'
+        elif arr_member['kind'] in ('int32', 'tick'):
+           packer = 'int'
+        else:
+           raise ValueError(f"Error: unknown array member type {member['type']}")
+        return f"b''.join([pack_{packer}(x) for x in {field}])"
     elif member['type']['kind'] == 'flags': # TODO: think about flags
         packer = 'int'
     elif member['type']['kind'] == 'optional':
         packer = 'int'
         # TODO: unpacker should allow not packing optional fields
         #       check how tw code does it and be smart here
-        if member['type']['inner']['kind'] == 'string': # TODO: sanitize cc
+        if member['type']['inner']['kind'] == 'string':
             packer = 'str'
         elif member['type']['inner']['kind'] in ('int32', 'tick'):
             packer = 'int'
     else:
         raise ValueError(f"Error: unknown type {member['type']}")
     return f'pack_{packer}({field})'
```

### Comparing `twnet_parser-0.3.3/setup.cfg` & `twnet_parser-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = twnet_parser
-version = 0.3.3
+version = 0.4.0
 author = ChillerDragon
 author_email = chillerdragon@gmail.com
 description = A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/teeworlds-network/twnet_parser
 license = BSD-2.0
```

### Comparing `twnet_parser-0.3.3/tests/control_packets7_test.py` & `twnet_parser-0.4.0/tests/control_packets7_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from twnet_parser.packet import *
 
 def test_parse_7_close_with_reason():
     packet = parse7(b'\x04\x0a\x00\xcf\x2e\xde\x1d\04shutdown\x00') # 0.7 close
 
     assert packet.version == '0.7'
 
-    assert packet.header.size == 0
     assert packet.header.ack == 10
     assert packet.header.token == b'\xcf.\xde\x1d'
     assert packet.header.num_chunks == 0
 
     assert packet.header.flags.control is True
     assert packet.header.flags.resend is False
     assert packet.header.flags.compression is False
```

### Comparing `twnet_parser-0.3.3/tests/int_packer_test.py` & `twnet_parser-0.4.0/tests/int_packer_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/tests/msg7/sv_tune_params_test.py` & `twnet_parser-0.4.0/tests/msg7/sv_tune_params_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/tests/packet_header6_test.py` & `twnet_parser-0.4.0/tests/packet_header6_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # TODO: uncomment and adjust ack/size when 0.6 is done
 
 # def test_parse_065_close():
 #     packet = parse7(b'\x10\x10\x00\x04\x9a\xcb\x09\xc9') # 0.6.5 close
 # 
 #     assert packet.version == '0.6.5'
 # 
-#     assert packet.header.size == 0
 #     assert packet.header.ack == 10
 #     assert packet.header.token == b'\x9a\xcb\x09\xc9'
 #     assert packet.header.num_chunks == 0
 # 
 #     assert packet.header.flags.control == True
 #     assert packet.header.flags.resend == False
 #     assert packet.header.flags.compression == False
```

### Comparing `twnet_parser-0.3.3/tests/packet_invalid_test.py` & `twnet_parser-0.4.0/tests/packet_invalid_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/tests/packet_with_chunks7_test.py` & `twnet_parser-0.4.0/tests/packet_with_chunks7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/tests/repack_chunks7_test.py` & `twnet_parser-0.4.0/tests/repack_chunks7_test.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/chunk_header.py` & `twnet_parser-0.4.0/twnet_parser/chunk_header.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/external/huffman.py` & `twnet_parser-0.4.0/twnet_parser/external/huffman.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/message_parser.py` & `twnet_parser-0.4.0/twnet_parser/message_parser.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/control/close.py` & `twnet_parser-0.4.0/twnet_parser/messages7/control/close.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/control/connect.py` & `twnet_parser-0.4.0/twnet_parser/messages7/control/connect.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/control/token.py` & `twnet_parser-0.4.0/twnet_parser/messages7/control/token.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_call_vote.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_call_vote.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
 class MsgClCallVote(PrettyPrint):
     def __init__(
             self,
             type: str = 'default',
             value: str = 'default',
             reason: str = 'default',
@@ -23,17 +23,17 @@
         self.force: bool = force
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.type = unpacker.get_str()
-        self.value = unpacker.get_str()
-        self.reason = unpacker.get_str()
+        self.type = unpacker.get_str(SANITIZE_CC)
+        self.value = unpacker.get_str(SANITIZE_CC)
+        self.reason = unpacker.get_str(SANITIZE_CC)
         self.force = unpacker.get_int() == 1
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.type) + \
             pack_str(self.value) + \
             pack_str(self.reason) + \
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_command.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd_add.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
 
-class MsgClCommand(PrettyPrint):
+class MsgRconCmdAdd(PrettyPrint):
     def __init__(
             self,
             name: str = 'default',
-            arguments: str = 'default'
+            help: str = 'default',
+            params: str = 'default'
     ) -> None:
-        self.message_name = 'cl_command'
-        self.system_message = False
+        self.message_name = 'rcon_cmd_add'
+        self.system_message = True
         self.header: ChunkHeader
 
         self.name: str = name
-        self.arguments: str = arguments
+        self.help: str = help
+        self.params: str = params
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.name = unpacker.get_str()
-        self.arguments = unpacker.get_str()
+        self.help = unpacker.get_str()
+        self.params = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.name) + \
-            pack_str(self.arguments)
+            pack_str(self.help) + \
+            pack_str(self.params)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_emoticon.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_emoticon.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_kill.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_kill.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_ready_change.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_ready_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_say.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_say.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
 class MsgClSay(PrettyPrint):
     def __init__(
             self,
             mode: int = 0,
             target: int = 0,
             message: str = 'default'
@@ -23,14 +23,14 @@
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.mode = unpacker.get_int() # TODO: this is a enum
         self.target = unpacker.get_int()
-        self.message = unpacker.get_str()
+        self.message = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.mode) + \
             pack_int(self.target) + \
             pack_str(self.message)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_set_spectator_mode.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_set_spectator_mode.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_set_team.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_set_team.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_skin_change.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_skin_change.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Annotated
 
-class MsgClSkinChange(PrettyPrint):
+class MsgSvSkinChange(PrettyPrint):
     def __init__(
             self,
-            skin_part_names: int = 0,
-            use_custom_colors: int = 0,
-            skin_part_colors: int = 0
+            client_id: int = 0,
+            skin_part_names: Annotated[list[str], 6] = \
+                ['', '', '', '', '', ''],
+            use_custom_colors: Annotated[list[bool], 6] = \
+                [False, False, False, False, False, False],
+            skin_part_colors: Annotated[list[int], 6] = \
+                [0, 0, 0, 0, 0, 0]
     ) -> None:
-        self.message_name = 'cl_skin_change'
+        self.message_name = 'sv_skin_change'
         self.system_message = False
         self.header: ChunkHeader
 
-        self.skin_part_names: int = skin_part_names
-        self.use_custom_colors: int = use_custom_colors
-        self.skin_part_colors: int = skin_part_colors
+        self.client_id: int = client_id
+        self.skin_part_names = skin_part_names
+        self.use_custom_colors = use_custom_colors
+        self.skin_part_colors = skin_part_colors
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.skin_part_names = unpacker.get_int() # TODO: this is an array
-        self.use_custom_colors = unpacker.get_int() # TODO: this is an array
-        self.skin_part_colors = unpacker.get_int() # TODO: this is an array
+        self.client_id = unpacker.get_int()
+        for i in range(0, 6):
+            self.skin_part_names[i] = unpacker.get_str(SANITIZE_CC)
+        for i in range(0, 6):
+            self.use_custom_colors[i] = unpacker.get_int() == 1
+        for i in range(0, 6):
+            self.skin_part_colors[i] = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.skin_part_names) + \
-            pack_int(self.use_custom_colors) + \
-            pack_int(self.skin_part_colors)
+        return pack_int(self.client_id) + \
+            b''.join([pack_str(x) for x in self.skin_part_names]) + \
+            b''.join([pack_int(x) for x in self.use_custom_colors]) + \
+            b''.join([pack_int(x) for x in self.skin_part_colors])
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_start_info.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_skin_change.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
+from typing import Annotated
 
-class MsgClStartInfo(PrettyPrint):
+class MsgClSkinChange(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default',
-            clan: str = 'default',
-            country: int = 0,
-            skin_part_names: int = 0,
-            use_custom_colors: int = 0,
-            skin_part_colors: int = 0
+            skin_part_names: Annotated[list[str], 6] = \
+                ['', '', '', '', '', ''],
+            use_custom_colors: Annotated[list[bool], 6] = \
+                [False, False, False, False, False, False],
+            skin_part_colors: Annotated[list[int], 6] = \
+                [0, 0, 0, 0, 0, 0]
     ) -> None:
-        self.message_name = 'cl_start_info'
+        self.message_name = 'cl_skin_change'
         self.system_message = False
         self.header: ChunkHeader
 
-        self.name: str = name
-        self.clan: str = clan
-        self.country: int = country
-        self.skin_part_names: int = skin_part_names
-        self.use_custom_colors: int = use_custom_colors
-        self.skin_part_colors: int = skin_part_colors
+        self.skin_part_names = skin_part_names
+        self.use_custom_colors = use_custom_colors
+        self.skin_part_colors = skin_part_colors
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
-        self.clan = unpacker.get_str()
-        self.country = unpacker.get_int()
-        self.skin_part_names = unpacker.get_int() # TODO: this is an array
-        self.use_custom_colors = unpacker.get_int() # TODO: this is an array
-        self.skin_part_colors = unpacker.get_int() # TODO: this is an array
+        for i in range(0, 6):
+            self.skin_part_names[i] = unpacker.get_str(SANITIZE_CC)
+        for i in range(0, 6):
+            self.use_custom_colors[i] = unpacker.get_int() == 1
+        for i in range(0, 6):
+            self.skin_part_colors[i] = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name) + \
-            pack_str(self.clan) + \
-            pack_int(self.country) + \
-            pack_int(self.skin_part_names) + \
-            pack_int(self.use_custom_colors) + \
-            pack_int(self.skin_part_colors)
+        return b''.join([pack_str(x) for x in self.skin_part_names]) + \
+            b''.join([pack_int(x) for x in self.use_custom_colors]) + \
+            b''.join([pack_int(x) for x in self.skin_part_colors])
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/cl_vote.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/cl_vote.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/de_client_enter.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
-class MsgDeClientEnter(PrettyPrint):
+class MsgSvChat(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default',
+            mode: int = 0,
             client_id: int = 0,
-            team: int = 0
+            target_id: int = 0,
+            message: str = 'default'
     ) -> None:
-        self.message_name = 'de_client_enter'
+        self.message_name = 'sv_chat'
         self.system_message = False
         self.header: ChunkHeader
 
-        self.name: str = name
+        self.mode: int = mode
         self.client_id: int = client_id
-        self.team: int = team
+        self.target_id: int = target_id
+        self.message: str = message
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
+        self.mode = unpacker.get_int() # TODO: this is a enum
         self.client_id = unpacker.get_int()
-        self.team = unpacker.get_int() # TODO: this is a enum
+        self.target_id = unpacker.get_int()
+        self.message = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name) + \
+        return pack_int(self.mode) + \
             pack_int(self.client_id) + \
-            pack_int(self.team)
+            pack_int(self.target_id) + \
+            pack_str(self.message)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/de_client_leave.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/de_client_enter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
-class MsgDeClientLeave(PrettyPrint):
+class MsgDeClientEnter(PrettyPrint):
     def __init__(
             self,
             name: str = 'default',
             client_id: int = 0,
-            reason: str = 'default'
+            team: int = 0
     ) -> None:
-        self.message_name = 'de_client_leave'
+        self.message_name = 'de_client_enter'
         self.system_message = False
         self.header: ChunkHeader
 
         self.name: str = name
         self.client_id: int = client_id
-        self.reason: str = reason
+        self.team: int = team
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
+        self.name = unpacker.get_str(SANITIZE_CC)
         self.client_id = unpacker.get_int()
-        self.reason = unpacker.get_str()
+        self.team = unpacker.get_int() # TODO: this is a enum
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.name) + \
             pack_int(self.client_id) + \
-            pack_str(self.reason)
+            pack_int(self.team)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_broadcast.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_broadcast.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_chat.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_kill_msg.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import pack_int
 
-class MsgSvChat(PrettyPrint):
+class MsgSvKillMsg(PrettyPrint):
     def __init__(
             self,
-            mode: int = 0,
-            client_id: int = 0,
-            target_id: int = 0,
-            message: str = 'default'
+            killer: int = 0,
+            victim: int = 0,
+            weapon: int = 0,
+            mode_special: int = 0
     ) -> None:
-        self.message_name = 'sv_chat'
+        self.message_name = 'sv_kill_msg'
         self.system_message = False
         self.header: ChunkHeader
 
-        self.mode: int = mode
-        self.client_id: int = client_id
-        self.target_id: int = target_id
-        self.message: str = message
+        self.killer: int = killer
+        self.victim: int = victim
+        self.weapon: int = weapon
+        self.mode_special: int = mode_special
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.mode = unpacker.get_int() # TODO: this is a enum
-        self.client_id = unpacker.get_int()
-        self.target_id = unpacker.get_int()
-        self.message = unpacker.get_str()
+        self.killer = unpacker.get_int()
+        self.victim = unpacker.get_int()
+        self.weapon = unpacker.get_int()
+        self.mode_special = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.mode) + \
-            pack_int(self.client_id) + \
-            pack_int(self.target_id) + \
-            pack_str(self.message)
+        return pack_int(self.killer) + \
+            pack_int(self.victim) + \
+            pack_int(self.weapon) + \
+            pack_int(self.mode_special)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_checkpoint.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_checkpoint.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_client_drop.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/input_timing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import pack_int
 
-class MsgSvClientDrop(PrettyPrint):
+class MsgInputTiming(PrettyPrint):
     def __init__(
             self,
-            client_id: int = 0,
-            reason: str = 'default',
-            silent: bool = False
+            input_pred_tick: int = 0,
+            time_left: int = 0
     ) -> None:
-        self.message_name = 'sv_client_drop'
-        self.system_message = False
+        self.message_name = 'input_timing'
+        self.system_message = True
         self.header: ChunkHeader
 
-        self.client_id: int = client_id
-        self.reason: str = reason
-        self.silent: bool = silent
+        self.input_pred_tick: int = input_pred_tick
+        self.time_left: int = time_left
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.client_id = unpacker.get_int()
-        self.reason = unpacker.get_str()
-        self.silent = unpacker.get_int() == 1
+        self.input_pred_tick = unpacker.get_int()
+        self.time_left = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.client_id) + \
-            pack_str(self.reason) + \
-            pack_int(self.silent)
+        return pack_int(self.input_pred_tick) + \
+            pack_int(self.time_left)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_client_info.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_server_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,48 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import pack_int
 
-class MsgSvClientInfo(PrettyPrint):
+class MsgSvServerSettings(PrettyPrint):
     def __init__(
             self,
-            client_id: int = 0,
-            local: bool = False,
-            team: int = 0,
-            name: str = 'default',
-            clan: str = 'default',
-            country: int = 0,
-            skin_part_names: int = 0,
-            use_custom_colors: int = 0,
-            skin_part_colors: int = 0,
-            silent: bool = False
+            kick_vote: bool = False,
+            kick_min: int = 0,
+            spec_vote: bool = False,
+            team_lock: bool = False,
+            team_balance: bool = False,
+            player_slots: int = 0
     ) -> None:
-        self.message_name = 'sv_client_info'
+        self.message_name = 'sv_server_settings'
         self.system_message = False
         self.header: ChunkHeader
 
-        self.client_id: int = client_id
-        self.local: bool = local
-        self.team: int = team
-        self.name: str = name
-        self.clan: str = clan
-        self.country: int = country
-        self.skin_part_names: int = skin_part_names
-        self.use_custom_colors: int = use_custom_colors
-        self.skin_part_colors: int = skin_part_colors
-        self.silent: bool = silent
+        self.kick_vote: bool = kick_vote
+        self.kick_min: int = kick_min
+        self.spec_vote: bool = spec_vote
+        self.team_lock: bool = team_lock
+        self.team_balance: bool = team_balance
+        self.player_slots: int = player_slots
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.client_id = unpacker.get_int()
-        self.local = unpacker.get_int() == 1
-        self.team = unpacker.get_int() # TODO: this is a enum
-        self.name = unpacker.get_str()
-        self.clan = unpacker.get_str()
-        self.country = unpacker.get_int()
-        self.skin_part_names = unpacker.get_int() # TODO: this is an array
-        self.use_custom_colors = unpacker.get_int() # TODO: this is an array
-        self.skin_part_colors = unpacker.get_int() # TODO: this is an array
-        self.silent = unpacker.get_int() == 1
+        self.kick_vote = unpacker.get_int() == 1
+        self.kick_min = unpacker.get_int()
+        self.spec_vote = unpacker.get_int() == 1
+        self.team_lock = unpacker.get_int() == 1
+        self.team_balance = unpacker.get_int() == 1
+        self.player_slots = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.client_id) + \
-            pack_int(self.local) + \
-            pack_int(self.team) + \
-            pack_str(self.name) + \
-            pack_str(self.clan) + \
-            pack_int(self.country) + \
-            pack_int(self.skin_part_names) + \
-            pack_int(self.use_custom_colors) + \
-            pack_int(self.skin_part_colors) + \
-            pack_int(self.silent)
+        return pack_int(self.kick_vote) + \
+            pack_int(self.kick_min) + \
+            pack_int(self.spec_vote) + \
+            pack_int(self.team_lock) + \
+            pack_int(self.team_balance) + \
+            pack_int(self.player_slots)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_command_info.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_command_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_str
 
 class MsgSvCommandInfo(PrettyPrint):
     def __init__(
             self,
             name: str = 'default',
             args_format: str = 'default',
             help_text: str = 'default'
@@ -21,16 +21,16 @@
         self.help_text: str = help_text
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
-        self.args_format = unpacker.get_str()
-        self.help_text = unpacker.get_str()
+        self.name = unpacker.get_str(SANITIZE_CC)
+        self.args_format = unpacker.get_str(SANITIZE_CC)
+        self.help_text = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.name) + \
             pack_str(self.args_format) + \
             pack_str(self.help_text)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_command_info_remove.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_command_info_remove.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_str
 
 class MsgSvCommandInfoRemove(PrettyPrint):
     def __init__(
             self,
             name: str = 'default'
     ) -> None:
         self.message_name = 'sv_command_info_remove'
@@ -17,12 +17,12 @@
         self.name: str = name
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
+        self.name = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.name)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_emoticon.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_emoticon.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_extra_projectile.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_extra_projectile.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_game_info.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_game_info.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_game_msg.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_game_msg.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_kill_msg.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_race_finish.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
-class MsgSvKillMsg(PrettyPrint):
+class MsgSvRaceFinish(PrettyPrint):
     def __init__(
             self,
-            killer: int = 0,
-            victim: int = 0,
-            weapon: int = 0,
-            mode_special: int = 0
+            client_id: int = 0,
+            time: int = 0,
+            diff: int = 0,
+            record_personal: bool = False,
+            record_server: bool = False
     ) -> None:
-        self.message_name = 'sv_kill_msg'
+        self.message_name = 'sv_race_finish'
         self.system_message = False
         self.header: ChunkHeader
 
-        self.killer: int = killer
-        self.victim: int = victim
-        self.weapon: int = weapon
-        self.mode_special: int = mode_special
+        self.client_id: int = client_id
+        self.time: int = time
+        self.diff: int = diff
+        self.record_personal: bool = record_personal
+        self.record_server: bool = record_server
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.killer = unpacker.get_int()
-        self.victim = unpacker.get_int()
-        self.weapon = unpacker.get_int()
-        self.mode_special = unpacker.get_int()
+        self.client_id = unpacker.get_int()
+        self.time = unpacker.get_int()
+        self.diff = unpacker.get_int()
+        self.record_personal = unpacker.get_int() == 1
+        self.record_server = unpacker.get_int() == 1
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.killer) + \
-            pack_int(self.victim) + \
-            pack_int(self.weapon) + \
-            pack_int(self.mode_special)
+        return pack_int(self.client_id) + \
+            pack_int(self.time) + \
+            pack_int(self.diff) + \
+            pack_int(self.record_personal) + \
+            pack_int(self.record_server)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_motd.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_motd.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_race_finish.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_team.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
-class MsgSvRaceFinish(PrettyPrint):
+class MsgSvTeam(PrettyPrint):
     def __init__(
             self,
             client_id: int = 0,
-            time: int = 0,
-            diff: int = 0,
-            record_personal: bool = False,
-            record_server: bool = False
+            team: int = 0,
+            silent: bool = False,
+            cooldown_tick: int = 0
     ) -> None:
-        self.message_name = 'sv_race_finish'
+        self.message_name = 'sv_team'
         self.system_message = False
         self.header: ChunkHeader
 
         self.client_id: int = client_id
-        self.time: int = time
-        self.diff: int = diff
-        self.record_personal: bool = record_personal
-        self.record_server: bool = record_server
+        self.team: int = team
+        self.silent: bool = silent
+        self.cooldown_tick: int = cooldown_tick
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
-        self.time = unpacker.get_int()
-        self.diff = unpacker.get_int()
-        self.record_personal = unpacker.get_int() == 1
-        self.record_server = unpacker.get_int() == 1
+        self.team = unpacker.get_int() # TODO: this is a enum
+        self.silent = unpacker.get_int() == 1
+        self.cooldown_tick = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.client_id) + \
-            pack_int(self.time) + \
-            pack_int(self.diff) + \
-            pack_int(self.record_personal) + \
-            pack_int(self.record_server)
+            pack_int(self.team) + \
+            pack_int(self.silent) + \
+            pack_int(self.cooldown_tick)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_ready_to_enter.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_ready_to_enter.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_team.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/snap_empty.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
 
-class MsgSvTeam(PrettyPrint):
+class MsgSnapEmpty(PrettyPrint):
     def __init__(
             self,
-            client_id: int = 0,
-            team: int = 0,
-            silent: bool = False,
-            cooldown_tick: int = 0
+            tick: int = 0,
+            delta_tick: int = 0
     ) -> None:
-        self.message_name = 'sv_team'
-        self.system_message = False
+        self.message_name = 'snap_empty'
+        self.system_message = True
         self.header: ChunkHeader
 
-        self.client_id: int = client_id
-        self.team: int = team
-        self.silent: bool = silent
-        self.cooldown_tick: int = cooldown_tick
+        self.tick: int = tick
+        self.delta_tick: int = delta_tick
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.client_id = unpacker.get_int()
-        self.team = unpacker.get_int() # TODO: this is a enum
-        self.silent = unpacker.get_int() == 1
-        self.cooldown_tick = unpacker.get_int()
+        self.tick = unpacker.get_int()
+        self.delta_tick = unpacker.get_int()
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.client_id) + \
-            pack_int(self.team) + \
-            pack_int(self.silent) + \
-            pack_int(self.cooldown_tick)
+        return pack_int(self.tick) + \
+            pack_int(self.delta_tick)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_tune_params.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_tune_params.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_clear_options.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_clear_options.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_option_add.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/map_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
 
-class MsgSvVoteOptionAdd(PrettyPrint):
+class MsgMapData(PrettyPrint):
     def __init__(
             self,
-            description: str = 'default'
+            data: bytes = b'\x00'
     ) -> None:
-        self.message_name = 'sv_vote_option_add'
-        self.system_message = False
+        self.message_name = 'map_data'
+        self.system_message = True
         self.header: ChunkHeader
 
-        self.description: str = description
+        self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.description = unpacker.get_str()
+        self.data = unpacker.get_raw()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.description)
+        return self.data
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_option_list_add.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_list_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_option_remove.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_option_remove.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_str
 
 class MsgSvVoteOptionRemove(PrettyPrint):
     def __init__(
             self,
             description: str = 'default'
     ) -> None:
         self.message_name = 'sv_vote_option_remove'
@@ -17,12 +17,12 @@
         self.description: str = description
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.description = unpacker.get_str()
+        self.description = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.description)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_set.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int, pack_str
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
 class MsgSvVoteSet(PrettyPrint):
     def __init__(
             self,
             client_id: int = 0,
             type: int = 0,
             timeout: int = 0,
@@ -28,16 +28,16 @@
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.client_id = unpacker.get_int()
         self.type = unpacker.get_int() # TODO: this is a enum
         self.timeout = unpacker.get_int()
-        self.description = unpacker.get_str()
-        self.reason = unpacker.get_str()
+        self.description = unpacker.get_str(SANITIZE_CC)
+        self.reason = unpacker.get_str(SANITIZE_CC)
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.client_id) + \
             pack_int(self.type) + \
             pack_int(self.timeout) + \
             pack_str(self.description) + \
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_vote_status.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_vote_status.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/game/sv_weapon_pickup.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_weapon_pickup.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/con_ready.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/con_ready.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/enter_game.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/enter_game.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/info.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/info.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.version = unpacker.get_str()
-        self.password = unpacker.get_str() # TODO: this can fail for optionals
-        self.client_version = unpacker.get_int() # TODO: this can fail for optionals
+        self.password = unpacker.get_str() # TODO: optionals
+        self.client_version = unpacker.get_int() # TODO: optionals
         return True
 
     def pack(self) -> bytes:
         return pack_str(self.version) + \
             pack_str(self.password) + \
             pack_int(self.client_version)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/input.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/input.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/input_timing.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/snap_single.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Optional
 
-class MsgInputTiming(PrettyPrint):
+class MsgSnapSingle(PrettyPrint):
     def __init__(
             self,
-            input_pred_tick: int = 0,
-            time_left: int = 0
+            tick: int = 0,
+            delta_tick: int = 0,
+            crc: int = 0,
+            data_size: Optional[int] = None,
+            data: bytes = b'\x00'
     ) -> None:
-        self.message_name = 'input_timing'
+        self.message_name = 'snap_single'
         self.system_message = True
         self.header: ChunkHeader
 
-        self.input_pred_tick: int = input_pred_tick
-        self.time_left: int = time_left
+        self.tick: int = tick
+        self.delta_tick: int = delta_tick
+        self.crc: int = crc
+        self.data_size: int = data_size if data_size else len(data)
+        self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.input_pred_tick = unpacker.get_int()
-        self.time_left = unpacker.get_int()
+        self.tick = unpacker.get_int()
+        self.delta_tick = unpacker.get_int()
+        self.crc = unpacker.get_int()
+        self.data_size = unpacker.get_int()
+        self.data = unpacker.get_raw(self.data_size)
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.input_pred_tick) + \
-            pack_int(self.time_left)
+        return pack_int(self.tick) + \
+            pack_int(self.delta_tick) + \
+            pack_int(self.crc) + \
+            pack_int(self.data_size) + \
+            self.data
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/map_change.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/map_change.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/map_data.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/server_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 
-class MsgMapData(PrettyPrint):
+class MsgServerInfo(PrettyPrint):
     def __init__(
             self,
             data: bytes = b'\x00'
     ) -> None:
-        self.message_name = 'map_data'
+        self.message_name = 'server_info'
         self.system_message = True
         self.header: ChunkHeader
 
         self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/maplist_entry_add.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/maplist_entry_add.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/maplist_entry_rem.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/maplist_entry_rem.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/ping.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/ping.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/ping_reply.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/ping_reply.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_auth.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_auth_off.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth_off.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_auth_on.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_auth_on.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_cmd.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_cmd_add.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_cmd_rem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
 
-class MsgRconCmdAdd(PrettyPrint):
+class MsgRconCmdRem(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default',
-            help: str = 'default',
-            params: str = 'default'
+            name: str = 'default'
     ) -> None:
-        self.message_name = 'rcon_cmd_add'
+        self.message_name = 'rcon_cmd_rem'
         self.system_message = True
         self.header: ChunkHeader
 
         self.name: str = name
-        self.help: str = help
-        self.params: str = params
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.name = unpacker.get_str()
-        self.help = unpacker.get_str()
-        self.params = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name) + \
-            pack_str(self.help) + \
-            pack_str(self.params)
+        return pack_str(self.name)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_cmd_rem.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/rcon_line.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_str
 
-class MsgRconCmdRem(PrettyPrint):
+class MsgRconLine(PrettyPrint):
     def __init__(
             self,
-            name: str = 'default'
+            line: str = 'default'
     ) -> None:
-        self.message_name = 'rcon_cmd_rem'
+        self.message_name = 'rcon_line'
         self.system_message = True
         self.header: ChunkHeader
 
-        self.name: str = name
+        self.line: str = line
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.name = unpacker.get_str()
+        self.line = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.name)
+        return pack_str(self.line)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/rcon_line.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/request_map_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
-from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_str
 
-class MsgRconLine(PrettyPrint):
+class MsgRequestMapData(PrettyPrint):
     def __init__(
             self,
-            line: str = 'default'
+
     ) -> None:
-        self.message_name = 'rcon_line'
+        self.message_name = 'request_map_data'
         self.system_message = True
         self.header: ChunkHeader
 
-        self.line: str = line
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
-        unpacker = Unpacker(data)
-        self.line = unpacker.get_str()
         return True
 
     def pack(self) -> bytes:
-        return pack_str(self.line)
+        return b''
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/ready.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/ready.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/snap.py` & `twnet_parser-0.4.0/twnet_parser/messages7/system/snap.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
 from twnet_parser.packer import pack_int
+from typing import Optional
 
 class MsgSnap(PrettyPrint):
     def __init__(
             self,
             tick: int = 0,
             delta_tick: int = 0,
             num_parts: int = 0,
             part: int = 0,
             crc: int = 0,
+            data_size: Optional[int] = None,
             data: bytes = b'\x00'
     ) -> None:
         self.message_name = 'snap'
         self.system_message = True
         self.header: ChunkHeader
 
         self.tick: int = tick
         self.delta_tick: int = delta_tick
         self.num_parts: int = num_parts
         self.part: int = part
         self.crc: int = crc
+        self.data_size: int = data_size if data_size else len(data)
         self.data: bytes = data
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
         self.tick = unpacker.get_int()
         self.delta_tick = unpacker.get_int()
         self.num_parts = unpacker.get_int()
         self.part = unpacker.get_int()
         self.crc = unpacker.get_int()
-        self.data = unpacker.get_raw()
+        self.data_size = unpacker.get_int()
+        self.data = unpacker.get_raw(self.data_size)
         return True
 
     def pack(self) -> bytes:
         return pack_int(self.tick) + \
             pack_int(self.delta_tick) + \
             pack_int(self.num_parts) + \
             pack_int(self.part) + \
             pack_int(self.crc) + \
+            pack_int(self.data_size) + \
             self.data
```

### Comparing `twnet_parser-0.3.3/twnet_parser/messages7/system/snap_single.py` & `twnet_parser-0.4.0/twnet_parser/messages7/game/sv_client_drop.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 # generated by scripts/generate_messages.py
 
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.packer import Unpacker
 from twnet_parser.chunk_header import ChunkHeader
-from twnet_parser.packer import pack_int
+from twnet_parser.packer import SANITIZE_CC, pack_int, pack_str
 
-class MsgSnapSingle(PrettyPrint):
+class MsgSvClientDrop(PrettyPrint):
     def __init__(
             self,
-            tick: int = 0,
-            delta_tick: int = 0,
-            crc: int = 0,
-            data: bytes = b'\x00'
+            client_id: int = 0,
+            reason: str = 'default',
+            silent: bool = False
     ) -> None:
-        self.message_name = 'snap_single'
-        self.system_message = True
+        self.message_name = 'sv_client_drop'
+        self.system_message = False
         self.header: ChunkHeader
 
-        self.tick: int = tick
-        self.delta_tick: int = delta_tick
-        self.crc: int = crc
-        self.data: bytes = data
+        self.client_id: int = client_id
+        self.reason: str = reason
+        self.silent: bool = silent
 
     # first byte of data
     # has to be the first byte of the message payload
     # NOT the chunk header and NOT the message id
     def unpack(self, data: bytes) -> bool:
         unpacker = Unpacker(data)
-        self.tick = unpacker.get_int()
-        self.delta_tick = unpacker.get_int()
-        self.crc = unpacker.get_int()
-        self.data = unpacker.get_raw()
+        self.client_id = unpacker.get_int()
+        self.reason = unpacker.get_str(SANITIZE_CC)
+        self.silent = unpacker.get_int() == 1
         return True
 
     def pack(self) -> bytes:
-        return pack_int(self.tick) + \
-            pack_int(self.delta_tick) + \
-            pack_int(self.crc) + \
-            self.data
+        return pack_int(self.client_id) + \
+            pack_str(self.reason) + \
+            pack_int(self.silent)
```

### Comparing `twnet_parser-0.3.3/twnet_parser/msg7.py` & `twnet_parser-0.4.0/twnet_parser/msg7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/msg_matcher/control7.py` & `twnet_parser-0.4.0/twnet_parser/msg_matcher/control7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/msg_matcher/game7.py` & `twnet_parser-0.4.0/twnet_parser/msg_matcher/game7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/msg_matcher/system7.py` & `twnet_parser-0.4.0/twnet_parser/msg_matcher/system7.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/twnet_parser/packer.py` & `twnet_parser-0.4.0/twnet_parser/packer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 #!/usr/bin/env python
 
+from typing import Final
+
 # Before chaning the current packer code to extend it
 # Consider having two packers
 #
 # One being this one. That is simple and fast.
 # Has no state or side effects.
 # Does no error checking.
 #
 # And another one that sanitizes the data
 # will throw errors unexpected data
 # return the amount of read and written bytes
 # and is attached to a class instance that
 # keeps track of a state
 
+NO_SANITIZE: Final[int] = 0
+SANITIZE: Final[int]  = 1
+SANITIZE_CC: Final[int] = 2
+SKIP_START_WHITESPACES: Final[int] = 3
+
 class Unpacker():
     def __init__(self, data: bytes) -> None:
         self._data = data
         self.idx = 0
 
     # first byte of the current buffer
     def byte(self) -> int:
@@ -60,20 +67,45 @@
             res |= (self.byte() & 0x7F) << (6 + 7 + 7 + 7)
             break
 
         self.idx += 1
         res ^= -sign
         return res
 
-    def get_str(self) -> str:
+    # TODO: optimize performance
+    #       I am highly confident iterating byte by byte is very
+    #       expensive in python
+    #       and something common as byte filtering has to have
+    #       a fast alternative
+    #
+    #       If there is nothing from the python standard
+    #       this might be worth writing in Cython
+    #       external C or rust
+    # TODO: make literals work currently passing in SANITIZE as arg
+    #       to unpacker.get_str() does not work because its not a literal ._.
+    # def get_str(self, sanitize: Literal[0,1,2,3] = 1) -> str:
+    def get_str(self, sanitize: int = SANITIZE) -> str:
         str_end: int = self.data().find(b'\x00')
         res: bytes = self.data()[:str_end]
         self.idx += str_end + 1
-        # TODO: add saitize and sanitize cc
-        return res.decode('utf-8')
+        if sanitize == NO_SANITIZE:
+            return res.decode('utf-8', 'ignore')
+        if sanitize == SANITIZE:
+            return bytes( \
+                [x if x > 32 or x in (9, 10, 13) else 32 for x in res]) \
+                .decode('utf-8', 'ignore' \
+            )
+        if sanitize == SANITIZE_CC:
+            return bytes( \
+                [x if x > 32 else 32 for x in res]) \
+                .decode('utf-8', 'ignore' \
+            )
+        if sanitize == SKIP_START_WHITESPACES:
+            return res.decode('utf-8').lstrip()
+        raise ValueError(f"Error: invalid sanitize mode {sanitize}")
 
 # TODO: optimize performance and benchmark in tests
 def pack_int(num: int) -> bytes:
     res: bytearray = bytearray(b'\x00')
     if num < 0:
         res[0] |= 0x40 # set sign bit
         num = ~num
```

### Comparing `twnet_parser-0.3.3/twnet_parser/packet.py` & `twnet_parser-0.4.0/twnet_parser/packet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 
 from typing import Union
 from typing import cast
 
-from twnet_parser import packer
+from twnet_parser.packer import Unpacker
 from twnet_parser.pretty_print import PrettyPrint
 from twnet_parser.message_parser import MessageParser
 from twnet_parser.net_message import NetMessage
 from twnet_parser.ctrl_message import CtrlMessage
 from twnet_parser.chunk_header import ChunkHeader, ChunkFlags
 from twnet_parser.msg_matcher.control7 import match_control7
+from twnet_parser.constants import NET_MAX_SEQUENCE
 
 from twnet_parser.external.huffman import huffman
 
 # TODO: what is a nice pythonic way of storing those?
 #       also does some version:: namespace thing make sense?
 PACKETFLAG7_CONTROL = 1
 PACKETFLAG7_RESEND = 2
@@ -37,20 +38,60 @@
         self.token = False
         self.control = False
         self.resend = False
         self.compression = False
         self.connless = False
 
 class PacketHeader(PrettyPrint):
-    def __init__(self) -> None:
-        self.flags: PacketFlags7 = PacketFlags7()
-        self.size: int = 0
-        self.ack: int = 0
-        self.token: bytes = b'\xff\xff\xff\xff'
-        self.num_chunks: int = 0
+    def __init__(
+            self,
+            flags: PacketFlags7 = PacketFlags7(),
+            ack: int = 0,
+            token: bytes = b'\xff\xff\xff\xff',
+            num_chunks: int = 0
+    ) -> None:
+        self.flags: PacketFlags7 = flags
+        self.ack: int = ack % NET_MAX_SEQUENCE
+        self.token: bytes = token
+        self.num_chunks: int = num_chunks
+
+    def pack(self) -> bytes:
+        """
+        Generate 7 byte teeworlds 0.7 packet header
+        based on the current instance variable
+        values.
+
+        The layout is as follows
+        6bit flags, 2bit ack
+        8bit ack
+        8bit chunks
+        32bit token
+
+        ffffffaa
+        aaaaaaaa
+        NNNNNNNN
+        TTTTTTTT
+        TTTTTTTT
+        TTTTTTTT
+        TTTTTTTT
+        """
+        flags = 0
+        if self.flags.control:
+            flags |= PACKETFLAG7_CONTROL
+        if self.flags.resend:
+            flags |= PACKETFLAG7_RESEND
+        if self.flags.compression:
+            flags |= PACKETFLAG7_COMPRESSION
+        if self.flags.connless:
+            flags |= PACKETFLAG7_CONNLESS
+        return bytes([ \
+            ((flags << 2)&0xfc) | ((self.ack>>8)&0x03), \
+            self.ack&0xff, \
+            self.num_chunks \
+        ]) + self.token
 
 class TwPacket(PrettyPrint):
     def __init__(self) -> None:
         self.version: str = 'unknown'
         self.payload_raw: bytes = b''
         self.payload_decompressed: bytes = b''
         self.header: PacketHeader = PacketHeader()
@@ -130,23 +171,24 @@
     # first byte of a message chunk
     # NOT the whole packet with packet header
     def get_message(self, data: bytes) -> NetMessage:
         chunk_header = ChunkHeaderParser().parse_header7(data)
         i = 2
         if chunk_header.flags.vital:
             i += 1
-        msg_id: int = packer.unpack_int(data[i:])
+        unpacker = Unpacker(data[i:])
+        msg_id: int = unpacker.get_int()
         i += 1
         sys: bool = (msg_id & 1) == 1
         msg_id >>= 1
         msg: NetMessage
         if sys:
-            msg = MessageParser().parse_sys_message(msg_id, data[i:])
+            msg = MessageParser().parse_sys_message(msg_id, unpacker.get_raw())
         else:
-            msg = MessageParser().parse_game_message(msg_id, data[i:])
+            msg = MessageParser().parse_game_message(msg_id, unpacker.get_raw())
         msg.header = chunk_header
         return msg
 
     def parse7(self, data: bytes, client: bool) -> TwPacket:
         pck = TwPacket()
         pck.version = '0.7'
         # TODO: what is the most performant way in python to do this?
```

### Comparing `twnet_parser-0.3.3/twnet_parser.egg-info/PKG-INFO` & `twnet_parser-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: twnet-parser
-Version: 0.3.3
+Name: twnet_parser
+Version: 0.4.0
 Summary: A teeworlds network protocol library, designed according to sans I/O (http://sans-io.readthedocs.io/) principles
 Home-page: https://gitlab.com/teeworlds-network/twnet_parser
 Author: ChillerDragon
 Author-email: chillerdragon@gmail.com
 License: BSD-2.0
 Project-URL: Bug Tracker, https://gitlab.com/teeworlds-network/twnet_parser/-/issues
 Project-URL: repository, https://gitlab.com/teeworlds-network/twnet_parser
@@ -46,36 +46,49 @@
 
 ## Features
 
 | Feature                        | Status             |
 | ------------------------------ | ------------------ |
 | Deserialize 0.7 packet headers | :heavy_check_mark: |
 | Deserialize 0.7 chunk headers  | :heavy_check_mark: |
-| Deserialize 0.7 messages       | 70%                |
+| Deserialize 0.7 messages       | 80%                |
 | Deserialize 0.7 snapshots      |                    |
-| Serialize 0.7 packet headers   |                    |
+| Serialize 0.7 packet headers   | :heavy_check_mark: |
 | Serialize 0.7 chunk headers    |                    |
-| Serialize 0.7 messages         | 70%                |
+| Serialize 0.7 messages         | 80%                |
 | Deserialize 0.6 packet headers |                    |
 | Deserialize 0.6 chunk headers  |                    |
 | Deserialize 0.6 messages       |                    |
 | Deserialize 0.6 snapshots      |                    |
 | Serialize 0.6 packet headers   |                    |
 | Serialize 0.6 chunk headers    |                    |
 | Serialize 0.6 messages         |                    |
 
 ## Non-Features (also not planned for this library)
 
 | Feature                        | Status  | Where to find it                            |
 | ------------------------------ | ------- | ------------------------------------------- |
 | Networking                     | :x:     | TODO: link if someone implemented it on top |
 | Protocol version detection     | :x:     | TODO: link if someone implemented it on top |
+| Track sequence number state    | :x:     | TODO: link if someone implemented it on top |
+| Track connection state         | :x:     | TODO: link if someone implemented it on top |
 
 Look elsewhere for these features. Or use this library to implement them on top.
 
+This project is intentionally only covering parsing the protocol.
+Not fully implemeting a state machine of the protocol.
+Or a fully working client / server software.
+
+If you want to build something with this library
+you do have to understand how the protocol works
+and when the client and server have to send what.
+
+This [protocol documentation](https://chillerdragon.github.io/teeworlds-protocol/index.html)
+should get you started to understand the basics.
+
 ## development setup
 
 ```bash
 git clone https://gitlab.com/teeworlds-network/twnet_parser
 cd twnet_parser
 python -m venv venv
 source venv/bin/activate
@@ -92,14 +105,17 @@
 pytest .
 
 # run style linter
 pylint src/
 
 # run type checker
 mypy src/
+
+# or use the bundle script that runs all tests
+./scripts/run_tests.sh
 ```
 
 ## package and release
 
 ```bash
 # manual
 pip install -r requirements/dev.txt
```

### Comparing `twnet_parser-0.3.3/twnet_parser.egg-info/SOURCES.txt` & `twnet_parser-0.4.0/twnet_parser.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 tests/packet_invalid_test.py
 tests/packet_with_chunks7_test.py
 tests/repack_chunks7_test.py
 tests/unpacker_state_test.py
 tests/msg7/sv_tune_params_test.py
 twnet_parser/__init__.py
 twnet_parser/chunk_header.py
+twnet_parser/constants.py
 twnet_parser/ctrl_message.py
 twnet_parser/message_parser.py
 twnet_parser/msg7.py
 twnet_parser/net_message.py
 twnet_parser/packer.py
 twnet_parser/packet.py
 twnet_parser/pretty_print.py
```

### Comparing `twnet_parser-0.3.3/venv/bin/rst2html.py` & `twnet_parser-0.4.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2html4.py` & `twnet_parser-0.4.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2html5.py` & `twnet_parser-0.4.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2latex.py` & `twnet_parser-0.4.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2man.py` & `twnet_parser-0.4.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2odt.py` & `twnet_parser-0.4.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2odt_prepstyles.py` & `twnet_parser-0.4.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2pseudoxml.py` & `twnet_parser-0.4.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2s5.py` & `twnet_parser-0.4.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2xetex.py` & `twnet_parser-0.4.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rst2xml.py` & `twnet_parser-0.4.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `twnet_parser-0.3.3/venv/bin/rstpep2html.py` & `twnet_parser-0.4.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

