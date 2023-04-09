# Comparing `tmp/agstoolbox-0.3.5.tar.gz` & `tmp/agstoolbox-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agstoolbox-0.3.5.tar", last modified: Sat Apr  8 20:42:29 2023, max compression
+gzip compressed data, was "agstoolbox-0.3.6.tar", last modified: Sun Apr  9 16:06:07 2023, max compression
```

## Comparing `agstoolbox-0.3.5.tar` & `agstoolbox-0.3.6.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.601116 agstoolbox-0.3.5/
--rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/AUTHORS
--rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/COPYING
--rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      101 2023-04-08 20:06:59.000000 agstoolbox-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1189 2023-04-08 20:42:29.600116 agstoolbox-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.5/README.rst
--rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/agstoolbox
--rw-rw-rw-   0        0        0      400 2023-04-08 03:13:15.000000 agstoolbox-0.3.5/atbx
--rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 20:42:29.601116 agstoolbox-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1669 2023-04-08 20:09:20.000000 agstoolbox-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.515118 agstoolbox-0.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.532116 agstoolbox-0.3.5/src/agstoolbox/
--rw-rw-rw-   0        0        0      198 2023-04-08 20:25:10.000000 agstoolbox-0.3.5/src/agstoolbox/__init__.py
--rw-rw-rw-   0        0        0     1017 2023-04-08 04:29:56.000000 agstoolbox-0.3.5/src/agstoolbox/__main__.py
--rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.5/src/agstoolbox/at_icons.py
--rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.5/src/agstoolbox/at_tasks.py
--rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.5/src/agstoolbox/at_trayindicator.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.549117 agstoolbox-0.3.5/src/agstoolbox/core/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:22:20.000000 agstoolbox-0.3.5/src/agstoolbox/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.556115 agstoolbox-0.3.5/src/agstoolbox/core/ags/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/src/agstoolbox/core/ags/__init__.py
--rw-rw-rw-   0        0        0      334 2022-03-20 16:55:45.000000 agstoolbox-0.3.5/src/agstoolbox/core/ags/ags_editor.py
--rw-rw-rw-   0        0        0   201168 2022-01-30 01:21:58.000000 agstoolbox-0.3.5/src/agstoolbox/core/ags/ags_editor_validation_data.py
--rw-rw-rw-   0        0        0      385 2022-04-27 23:52:03.000000 agstoolbox-0.3.5/src/agstoolbox/core/ags/ags_local_run.py
--rw-rw-rw-   0        0        0      361 2022-03-20 16:56:08.000000 agstoolbox-0.3.5/src/agstoolbox/core/ags/game_project.py
--rw-rw-rw-   0        0        0     3086 2023-04-08 16:50:10.000000 agstoolbox-0.3.5/src/agstoolbox/core/ags/get_game_projects.py
--rw-rw-rw-   0        0        0     2545 2023-04-07 21:27:44.000000 agstoolbox-0.3.5/src/agstoolbox/core/ags/get_local_ags_editors.py
--rw-rw-rw-   0        0        0     1328 2022-02-05 18:27:18.000000 agstoolbox-0.3.5/src/agstoolbox/core/ags/validate_ags_editor.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.559116 agstoolbox-0.3.5/src/agstoolbox/core/cmdline/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:10:57.000000 agstoolbox-0.3.5/src/agstoolbox/core/cmdline/__init__.py
--rw-rw-rw-   0        0        0    10551 2023-04-08 17:04:31.000000 agstoolbox-0.3.5/src/agstoolbox/core/cmdline/cmdline.py
--rw-rw-rw-   0        0        0      742 2023-04-08 17:11:05.000000 agstoolbox-0.3.5/src/agstoolbox/core/cmdline/cmdline_download.py
--rw-rw-rw-   0        0        0     1506 2023-04-08 17:09:05.000000 agstoolbox-0.3.5/src/agstoolbox/core/cmdline/progress.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.564118 agstoolbox-0.3.5/src/agstoolbox/core/gh/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/src/agstoolbox/core/gh/__init__.py
--rw-rw-rw-   0        0        0     1093 2023-04-08 02:50:16.000000 agstoolbox-0.3.5/src/agstoolbox/core/gh/download_release.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 02:15:27.000000 agstoolbox-0.3.5/src/agstoolbox/core/gh/install_release.py
--rw-rw-rw-   0        0        0     3474 2023-04-08 02:44:10.000000 agstoolbox-0.3.5/src/agstoolbox/core/gh/list_releases.py
--rw-rw-rw-   0        0        0      530 2023-04-08 02:43:46.000000 agstoolbox-0.3.5/src/agstoolbox/core/gh/release.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.567116 agstoolbox-0.3.5/src/agstoolbox/core/settings/
--rw-rw-rw-   0        0        0        0 2023-04-07 00:44:47.000000 agstoolbox-0.3.5/src/agstoolbox/core/settings/__init__.py
--rw-rw-rw-   0        0        0     5541 2023-04-08 16:42:31.000000 agstoolbox-0.3.5/src/agstoolbox/core/settings/settings.py
--rw-rw-rw-   0        0        0      289 2023-04-07 02:07:43.000000 agstoolbox-0.3.5/src/agstoolbox/core/settings/settings_data.py
--rw-rw-rw-   0        0        0     2286 2023-04-07 02:36:47.000000 agstoolbox-0.3.5/src/agstoolbox/core/settings/settings_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.576120 agstoolbox-0.3.5/src/agstoolbox/core/utils/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:23:07.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/__init__.py
--rw-rw-rw-   0        0        0      796 2023-04-07 01:04:11.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/basics.py
--rw-rw-rw-   0        0        0      797 2023-04-08 02:50:26.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/downloader.py
--rw-rw-rw-   0        0        0     4237 2023-04-08 03:40:39.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/file.py
--rw-rw-rw-   0        0        0      139 2022-01-27 21:57:07.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/math.py
--rw-rw-rw-   0        0        0       99 2023-04-05 02:07:05.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/open_in_browser.py
--rw-rw-rw-   0        0        0     1581 2022-01-29 21:55:33.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/pe.py
--rw-rw-rw-   0        0        0      246 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/singleton.py
--rw-rw-rw-   0        0        0     1836 2023-04-07 02:47:18.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/startup.py
--rw-rw-rw-   0        0        0      641 2023-04-08 16:41:22.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/systemdirs.py
--rw-rw-rw-   0        0        0     1008 2023-04-05 23:29:30.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/time.py
--rw-rw-rw-   0        0        0     1256 2023-04-03 01:20:15.000000 agstoolbox-0.3.5/src/agstoolbox/core/utils/win_registry.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.579116 agstoolbox-0.3.5/src/agstoolbox/core/version/
--rw-rw-rw-   0        0        0        0 2022-03-20 16:16:18.000000 agstoolbox-0.3.5/src/agstoolbox/core/version/__init__.py
--rw-rw-rw-   0        0        0      258 2023-04-08 01:38:27.000000 agstoolbox-0.3.5/src/agstoolbox/core/version/version.py
--rw-rw-rw-   0        0        0     3313 2023-04-08 01:43:53.000000 agstoolbox-0.3.5/src/agstoolbox/core/version/version_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.585116 agstoolbox-0.3.5/src/agstoolbox/data/
--rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.5/src/agstoolbox/data/at_ags_editor_icon.png
--rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/src/agstoolbox/data/at_ags_engine_icon.png
--rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.5/src/agstoolbox/data/at_icon.png
--rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.5/src/agstoolbox/data/at_icon_big.png
--rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.5/src/agstoolbox/data/exit_icon.png
--rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.5/src/agstoolbox/data/refresh_icon.png
--rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.5/src/agstoolbox/data/settings_icon.png
--rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/src/agstoolbox/getdata.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.588115 agstoolbox-0.3.5/src/agstoolbox/panels/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/src/agstoolbox/panels/__init__.py
--rw-rw-rw-   0        0        0     5446 2023-04-07 02:51:49.000000 agstoolbox-0.3.5/src/agstoolbox/panels/at_mainpanel.py
--rw-rw-rw-   0        0        0     7540 2023-04-07 03:11:46.000000 agstoolbox-0.3.5/src/agstoolbox/panels/at_settings_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.590116 agstoolbox-0.3.5/src/agstoolbox/system/
--rw-rw-rw-   0        0        0        0 2023-04-02 19:34:00.000000 agstoolbox-0.3.5/src/agstoolbox/system/__init__.py
--rw-rw-rw-   0        0        0      394 2023-04-02 20:12:53.000000 agstoolbox-0.3.5/src/agstoolbox/system/at_runguard.py
--rw-rw-rw-   0        0        0     1210 2023-04-03 00:55:58.000000 agstoolbox-0.3.5/src/agstoolbox/system/at_unique_application.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.596119 agstoolbox-0.3.5/src/agstoolbox/wdgts/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts/__init__.py
--rw-rw-rw-   0        0        0     7388 2023-04-07 02:54:37.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts/at_dirlist_wdgt.py
--rw-rw-rw-   0        0        0     2528 2023-04-07 02:54:50.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts/at_single_dir_wdgt.py
--rw-rw-rw-   0        0        0     5943 2022-04-27 23:52:03.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts/at_tree_item_project.py
--rw-rw-rw-   0        0        0     8291 2023-04-05 02:14:45.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts/at_tree_item_tool.py
--rw-rw-rw-   0        0        0     1428 2023-04-04 01:42:57.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts/at_tree_projects_wdgt.py
--rw-rw-rw-   0        0        0     6505 2023-04-05 02:02:50.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts/at_tree_tools_wdgt.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.599116 agstoolbox-0.3.5/src/agstoolbox/wdgts_utils/
--rw-rw-rw-   0        0        0        0 2022-04-27 23:21:51.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts_utils/__init__.py
--rw-rw-rw-   0        0        0      358 2022-04-27 23:30:17.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts_utils/action_utils.py
--rw-rw-rw-   0        0        0      467 2022-04-27 23:52:03.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts_utils/ags_local_extra.py
--rw-rw-rw-   0        0        0      899 2022-04-27 23:49:42.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts_utils/file_explorer.py
--rw-rw-rw-   0        0        0      149 2023-04-02 23:02:36.000000 agstoolbox-0.3.5/src/agstoolbox/wdgts_utils/get_self_path.py
-drwxrwxrwx   0        0        0        0 2023-04-08 20:42:29.548120 agstoolbox-0.3.5/src/agstoolbox.egg-info/
--rw-rw-rw-   0        0        0     1189 2023-04-08 20:42:29.000000 agstoolbox-0.3.5/src/agstoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2942 2023-04-08 20:42:29.000000 agstoolbox-0.3.5/src/agstoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 20:42:29.000000 agstoolbox-0.3.5/src/agstoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-08 20:42:29.000000 agstoolbox-0.3.5/src/agstoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 20:42:29.000000 agstoolbox-0.3.5/src/agstoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.637252 agstoolbox-0.3.6/
+-rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/AUTHORS
+-rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/COPYING
+-rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-04-08 20:06:59.000000 agstoolbox-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1189 2023-04-09 16:06:07.636251 agstoolbox-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.6/README.rst
+-rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/agstoolbox
+-rw-rw-rw-   0        0        0      416 2023-04-08 22:53:12.000000 agstoolbox-0.3.6/atbx
+-rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 16:06:07.637252 agstoolbox-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1678 2023-04-09 02:05:29.000000 agstoolbox-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.396505 agstoolbox-0.3.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.431505 agstoolbox-0.3.6/src/agstoolbox/
+-rw-rw-rw-   0        0        0      198 2023-04-09 16:02:35.000000 agstoolbox-0.3.6/src/agstoolbox/__init__.py
+-rw-rw-rw-   0        0        0     1023 2023-04-09 03:43:47.000000 agstoolbox-0.3.6/src/agstoolbox/__main__.py
+-rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.6/src/agstoolbox/at_icons.py
+-rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.6/src/agstoolbox/at_tasks.py
+-rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.6/src/agstoolbox/at_trayindicator.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.447043 agstoolbox-0.3.6/src/agstoolbox/core/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:22:20.000000 agstoolbox-0.3.6/src/agstoolbox/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.470252 agstoolbox-0.3.6/src/agstoolbox/core/ags/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-04-09 03:06:08.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_editor.py
+-rw-rw-rw-   0        0        0   201168 2022-01-30 01:21:58.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_editor_validation_data.py
+-rw-rw-rw-   0        0        0      673 2023-04-09 15:56:14.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_local_run.py
+-rw-rw-rw-   0        0        0      361 2022-03-20 16:56:08.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/game_project.py
+-rw-rw-rw-   0        0        0     3561 2023-04-09 03:08:16.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/get_game_projects.py
+-rw-rw-rw-   0        0        0     2545 2023-04-07 21:27:44.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/get_local_ags_editors.py
+-rw-rw-rw-   0        0        0     1328 2022-02-05 18:27:18.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/validate_ags_editor.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.482250 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:10:57.000000 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/__init__.py
+-rw-rw-rw-   0        0        0    13079 2023-04-09 15:46:59.000000 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/cmdline.py
+-rw-rw-rw-   0        0        0      742 2023-04-08 17:11:05.000000 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/cmdline_download.py
+-rw-rw-rw-   0        0        0     1506 2023-04-08 17:09:05.000000 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/progress.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.495251 agstoolbox-0.3.6/src/agstoolbox/core/gh/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/__init__.py
+-rw-rw-rw-   0        0        0     1093 2023-04-08 02:50:16.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/download_release.py
+-rw-rw-rw-   0        0        0     1115 2023-04-09 03:46:16.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/install_release.py
+-rw-rw-rw-   0        0        0     3474 2023-04-08 02:44:10.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/list_releases.py
+-rw-rw-rw-   0        0        0      497 2023-04-09 03:35:53.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/release.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.508250 agstoolbox-0.3.6/src/agstoolbox/core/settings/
+-rw-rw-rw-   0        0        0        0 2023-04-07 00:44:47.000000 agstoolbox-0.3.6/src/agstoolbox/core/settings/__init__.py
+-rw-rw-rw-   0        0        0     5600 2023-04-08 22:11:07.000000 agstoolbox-0.3.6/src/agstoolbox/core/settings/settings.py
+-rw-rw-rw-   0        0        0      287 2023-04-09 03:39:13.000000 agstoolbox-0.3.6/src/agstoolbox/core/settings/settings_data.py
+-rw-rw-rw-   0        0        0     2286 2023-04-07 02:36:47.000000 agstoolbox-0.3.6/src/agstoolbox/core/settings/settings_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.555252 agstoolbox-0.3.6/src/agstoolbox/core/utils/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:23:07.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-04-07 01:04:11.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/basics.py
+-rw-rw-rw-   0        0        0      797 2023-04-08 02:50:26.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/downloader.py
+-rw-rw-rw-   0        0        0     4532 2023-04-09 15:55:35.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/file.py
+-rw-rw-rw-   0        0        0      139 2022-01-27 21:57:07.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/math.py
+-rw-rw-rw-   0        0        0       99 2023-04-05 02:07:05.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/open_in_browser.py
+-rw-rw-rw-   0        0        0     1581 2022-01-29 21:55:33.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/pe.py
+-rw-rw-rw-   0        0        0      246 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/singleton.py
+-rw-rw-rw-   0        0        0     1836 2023-04-07 02:47:18.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/startup.py
+-rw-rw-rw-   0        0        0      641 2023-04-08 16:41:22.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/systemdirs.py
+-rw-rw-rw-   0        0        0     1008 2023-04-09 03:44:30.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/time.py
+-rw-rw-rw-   0        0        0     1256 2023-04-09 03:44:51.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/win_registry.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.565250 agstoolbox-0.3.6/src/agstoolbox/core/version/
+-rw-rw-rw-   0        0        0        0 2022-03-20 16:16:18.000000 agstoolbox-0.3.6/src/agstoolbox/core/version/__init__.py
+-rw-rw-rw-   0        0        0      258 2023-04-08 01:38:27.000000 agstoolbox-0.3.6/src/agstoolbox/core/version/version.py
+-rw-rw-rw-   0        0        0     3313 2023-04-08 01:43:53.000000 agstoolbox-0.3.6/src/agstoolbox/core/version/version_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.584250 agstoolbox-0.3.6/src/agstoolbox/data/
+-rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.6/src/agstoolbox/data/at_ags_editor_icon.png
+-rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/data/at_ags_engine_icon.png
+-rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.6/src/agstoolbox/data/at_icon.png
+-rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.6/src/agstoolbox/data/at_icon_big.png
+-rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.6/src/agstoolbox/data/exit_icon.png
+-rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.6/src/agstoolbox/data/refresh_icon.png
+-rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.6/src/agstoolbox/data/settings_icon.png
+-rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/getdata.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.591253 agstoolbox-0.3.6/src/agstoolbox/panels/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/panels/__init__.py
+-rw-rw-rw-   0        0        0     5446 2023-04-07 02:51:49.000000 agstoolbox-0.3.6/src/agstoolbox/panels/at_mainpanel.py
+-rw-rw-rw-   0        0        0     7533 2023-04-09 03:39:22.000000 agstoolbox-0.3.6/src/agstoolbox/panels/at_settings_dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.601251 agstoolbox-0.3.6/src/agstoolbox/system/
+-rw-rw-rw-   0        0        0        0 2023-04-02 19:34:00.000000 agstoolbox-0.3.6/src/agstoolbox/system/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-02 20:12:53.000000 agstoolbox-0.3.6/src/agstoolbox/system/at_runguard.py
+-rw-rw-rw-   0        0        0     1210 2023-04-03 00:55:58.000000 agstoolbox-0.3.6/src/agstoolbox/system/at_unique_application.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.616250 agstoolbox-0.3.6/src/agstoolbox/wdgts/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/__init__.py
+-rw-rw-rw-   0        0        0     7381 2023-04-09 03:39:13.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_dirlist_wdgt.py
+-rw-rw-rw-   0        0        0     2510 2023-04-09 03:40:47.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_single_dir_wdgt.py
+-rw-rw-rw-   0        0        0     6290 2023-04-09 16:00:52.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_item_project.py
+-rw-rw-rw-   0        0        0     8291 2023-04-05 02:14:45.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_item_tool.py
+-rw-rw-rw-   0        0        0     1428 2023-04-04 01:42:57.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_projects_wdgt.py
+-rw-rw-rw-   0        0        0     7062 2023-04-09 15:59:58.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_tools_wdgt.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.635250 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/
+-rw-rw-rw-   0        0        0        0 2022-04-27 23:21:51.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/__init__.py
+-rw-rw-rw-   0        0        0      358 2022-04-27 23:30:17.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/action_utils.py
+-rw-rw-rw-   0        0        0      467 2022-04-27 23:52:03.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/ags_local_extra.py
+-rw-rw-rw-   0        0        0      899 2022-04-27 23:49:42.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/file_explorer.py
+-rw-rw-rw-   0        0        0      149 2023-04-02 23:02:36.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/get_self_path.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.446042 agstoolbox-0.3.6/src/agstoolbox.egg-info/
+-rw-rw-rw-   0        0        0     1189 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2942 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/top_level.txt
```

### Comparing `agstoolbox-0.3.5/COPYING` & `agstoolbox-0.3.6/COPYING`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/LICENSE` & `agstoolbox-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/PKG-INFO` & `agstoolbox-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.5
+Version: 0.3.6
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.5
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.6
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `agstoolbox-0.3.5/README.rst` & `agstoolbox-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/pyproject.toml` & `agstoolbox-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/setup.py` & `agstoolbox-0.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from codecs import open
 from pathlib import Path
 
 from setuptools import setup, find_packages
 import re
 
-
 with open('src/agstoolbox/__init__.py', 'r') as fd:
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
                         fd.read(), re.MULTILINE).group(1)
 
-
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name='agstoolbox',
     version=version,
     description='Utility to help manage Adventure Game Studio Projects and Editors.',
@@ -23,28 +21,38 @@
     author='erico',
     author_email='eri0onpm@gmail.com',
     license='MIT',
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License'
     ],
-    keywords=['AGS Toolbox', 'Adventure Game Studio', 'development', 'ags', 'Game Development',
-              'gamedev'],
-    install_requires=['pyqt6', 'requests', 'defusedxml', 'platformdirs', 'pefile'],
-    packages=['agstoolbox',
-              'agstoolbox.core',
-              'agstoolbox.core.ags',
-              'agstoolbox.core.cmdline',
-              'agstoolbox.core.gh',
-              'agstoolbox.core.settings',
-              'agstoolbox.core.utils',
-              'agstoolbox.core.version',
-              'agstoolbox.panels',
-              'agstoolbox.system',
-              'agstoolbox.wdgts',
-              'agstoolbox.wdgts_utils'],
+    keywords=[
+        'AGS Toolbox', 'Adventure Game Studio', 'development', 'ags', 'Game Development', 'gamedev'
+    ],
+    install_requires=[
+        'pyqt6',
+        'requests',
+        'defusedxml',
+        'platformdirs',
+        'pefile',
+        'shtab'
+    ],
+    packages=[
+        'agstoolbox',
+        'agstoolbox.core',
+        'agstoolbox.core.ags',
+        'agstoolbox.core.cmdline',
+        'agstoolbox.core.gh',
+        'agstoolbox.core.settings',
+        'agstoolbox.core.utils',
+        'agstoolbox.core.version',
+        'agstoolbox.panels',
+        'agstoolbox.system',
+        'agstoolbox.wdgts',
+        'agstoolbox.wdgts_utils'
+    ],
     package_dir={"": "src"},
     scripts=["agstoolbox", "atbx"],
     package_data={
         'agstoolbox': ['data/*.png']
     },
 )
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/__main__.py` & `agstoolbox-0.3.6/src/agstoolbox/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-#!/usr/bin/python3
-# -*- coding: utf-8 -*-
-"""
-.. module:: agstoolbox
-   :platform: Windows
-   :synopsis: An application to help managing AGS Editor versions
-.. moduleauthor:: Érico Vieira Porto
-"""
-
-from os import environ as environ
-
-# TODO: figure out how to avoid import when no graphical environment exists
-from agstoolbox.at_trayindicator import run_tray_indicator
-from agstoolbox.core.cmdline.cmdline import cmdline
-
-
-def main():
-    """"
-    agstoolbox main routine
-    When you use `python -m agstoolbox`, the main routine is called.
-    If you use `pip install agstoolbox`, typing agstoolbox will also call this routine.
-    The objective of this function is to:
-    1. load agstoolbox when called without args
-    2. seeing the current version by using `--version`, and not opening agstoolbox
-    """
-    environ["LIBOVERLAY_SCROLLBAR"] = "0"
-
-    ap_args = cmdline(False)
-    run_tray_indicator(ap_args)
-
-
-def Run():
-    main()
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/python3
+# -*- coding: utf-8 -*-
+"""
+.. module:: agstoolbox
+   :platform: Windows
+   :synopsis: An application to help managing AGS Editor versions
+.. moduleauthor:: Érico Vieira Porto
+"""
+
+from os import environ as environ
+
+# TODO: figure out how to avoid import when no graphical environment exists
+from agstoolbox.at_trayindicator import run_tray_indicator
+from agstoolbox.core.cmdline.cmdline import cmdline
+from agstoolbox import __title__
+
+
+def main():
+    """
+    agstoolbox main routine
+    When you use `python -m agstoolbox`, the main routine is called.
+    If you use `pip install agstoolbox`, typing agstoolbox will also call this routine.
+    The objective of this function is to:
+    1. load agstoolbox when called without args
+    2. seeing the current version by using `--version`, and not opening agstoolbox
+    """
+    environ["LIBOVERLAY_SCROLLBAR"] = "0"
+
+    ap_args = cmdline(False, __title__)
+    run_tray_indicator(ap_args)
+
+
+def Run():
+    main()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/at_icons.py` & `agstoolbox-0.3.6/src/agstoolbox/at_icons.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/at_tasks.py` & `agstoolbox-0.3.6/src/agstoolbox/at_tasks.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/at_trayindicator.py` & `agstoolbox-0.3.6/src/agstoolbox/at_trayindicator.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/ags/ags_editor_validation_data.py` & `agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_editor_validation_data.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/ags/get_local_ags_editors.py` & `agstoolbox-0.3.6/src/agstoolbox/core/ags/get_local_ags_editors.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/ags/validate_ags_editor.py` & `agstoolbox-0.3.6/src/agstoolbox/core/ags/validate_ags_editor.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/cmdline/cmdline_download.py` & `agstoolbox-0.3.6/src/agstoolbox/core/cmdline/cmdline_download.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/cmdline/progress.py` & `agstoolbox-0.3.6/src/agstoolbox/core/cmdline/progress.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/gh/download_release.py` & `agstoolbox-0.3.6/src/agstoolbox/core/gh/download_release.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/gh/install_release.py` & `agstoolbox-0.3.6/src/agstoolbox/core/gh/install_release.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 def get_release_install_dir(release: Release) -> str:
     base_install_dir = Settings().get_editor_install_dir()
     return os.path.join(base_install_dir, release.version.as_str)
 
 
 def is_install_dir_busy(release: Release) -> bool:
     install_dir = get_release_install_dir(release)
-    dir_doesn_exist: bool = not os.path.exists(install_dir)
-    if dir_doesn_exist:
+    dir_doesnt_exist: bool = not os.path.exists(install_dir)
+    if dir_doesnt_exist:
         return False
     dir_exists_but_empty: bool = os.path.isdir(install_dir) and not os.listdir(install_dir)
     return not dir_exists_but_empty
 
 
 def install_release_from_cache(release: Release):
     filepath_in_cache = get_zip_archive_cache_path(release)
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/gh/list_releases.py` & `agstoolbox-0.3.6/src/agstoolbox/core/gh/list_releases.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/settings/settings.py` & `agstoolbox-0.3.6/src/agstoolbox/core/settings/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,27 +114,29 @@
 
     def get_editor_install_dir(self):
         return self.editor_install_dir
 
     def get_run_when_os_starts(self):
         return self.run_when_os_starts
 
-    def save(self):
-        settings_dir = get_settings_dir()
-        settings_path = get_settings_path()
-
-        mkdirp(settings_dir)
-
+    def dump(self) -> str:
         data = SettingsData()
         data.run_when_os_starts = self.run_when_os_starts
         data.project_search_dirs = self.project_search_dirs
         data.manually_installed_editors_search_dirs = self.manually_installed_editors_search_dirs
         data.tools_install_dir = self.tools_install_dir
 
-        data_string = save_settings_data_to_json_string(data)
+        return save_settings_data_to_json_string(data)
+
+    def save(self):
+        settings_dir = get_settings_dir()
+        settings_path = get_settings_path()
+
+        mkdirp(settings_dir)
+        data_string: str = self.dump()
 
         with open(settings_path, 'w+', encoding="utf-8") as f:
             f.write(data_string)
             f.flush()
 
     def load(self):
         settings_path: str = get_settings_path()
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/settings/settings_utils.py` & `agstoolbox-0.3.6/src/agstoolbox/core/settings/settings_utils.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/utils/basics.py` & `agstoolbox-0.3.6/src/agstoolbox/core/utils/basics.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/utils/downloader.py` & `agstoolbox-0.3.6/src/agstoolbox/core/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/utils/file.py` & `agstoolbox-0.3.6/src/agstoolbox/core/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,19 +63,24 @@
 
     return None
 
 
 def internal_run_fast_scandir(directory: str, filename: str):  # dir: str, ext: list
     sub_folders, files = [], []
 
-    directory = Path(directory).as_posix()
+    if Path(directory).is_dir() and Path(directory).exists():
+        directory = Path(directory).as_posix()
+    else:
+        directory = get_dir(directory)
 
     os_scandir_res = []
     try:
         os_scandir_res = os.scandir(directory)
+    except NotADirectoryError:
+        os_scandir_res = []
     except PermissionError:
         os_scandir_res = []
 
     for f in os_scandir_res:
         if f.is_dir():
             sub_folders.append(f.path)
         if f.is_file():
@@ -148,7 +153,12 @@
             pass
 
 
 def mkdirp(path_dir: str):
     _mk_dir_recursive(path_dir)
     # alternate implementation if needed
     # Path(path_dir).mkdir(parents=True, exist_ok=True)
+
+
+def get_absolute_path(a_path: str) -> str:
+    return os.path.abspath(os.path.expanduser(os.path.expandvars(a_path)))
+
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/utils/pe.py` & `agstoolbox-0.3.6/src/agstoolbox/core/utils/pe.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/utils/startup.py` & `agstoolbox-0.3.6/src/agstoolbox/core/utils/startup.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/utils/systemdirs.py` & `agstoolbox-0.3.6/src/agstoolbox/core/utils/systemdirs.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/utils/time.py` & `agstoolbox-0.3.6/src/agstoolbox/core/utils/time.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
     if diff.days >= 5:
         return t.strftime("%d/%m/%Y")
 
     for unit in units:
         dur = units[unit](diff)  # Run the lambda function to get a duration
         if dur > 0:
-            unit = unit[:-dur] if dur == 1 else unit  # De-pluralize if duration is 1 ('1 day' vs
-            # '2 days')
+            # if duration is 1 ('1 day' vs '2 days')
+            unit = unit[:-dur] if dur == 1 else unit  # De-pluralize
             return '%s %s ago' % (dur, unit)
     return 'just now'
 
 
 def s_ago(ft: float) -> str:
     t = datetime.utcfromtimestamp(ft)
     diff = datetime.utcnow() - t
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/utils/win_registry.py` & `agstoolbox-0.3.6/src/agstoolbox/core/utils/win_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import winreg
 from pathlib import PureWindowsPath
 
 
 def set_run_key(key, value):
     """
-    Set/Remove Run Key in windows registry.
+    Set/Remove Run Key in Windows registry.
 
     :param key: Run Key Name
     :param value: Program to Run
     :return: None
     """
     # This is for the system run variable
     reg_key = winreg.OpenKey(
         winreg.HKEY_CURRENT_USER,
         r'Software\Microsoft\Windows\CurrentVersion\Run',
         0, winreg.KEY_WRITE | winreg.KEY_READ)
 
-    if not value is None:
+    if value is not None:
         value = str(PureWindowsPath(value))
 
     with reg_key:
         if value is None:
             winreg.DeleteValue(reg_key, key)
         else:
             if '%' in value:
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/core/version/version_utils.py` & `agstoolbox-0.3.6/src/agstoolbox/core/version/version_utils.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/data/at_ags_editor_icon.png` & `agstoolbox-0.3.6/src/agstoolbox/data/at_ags_editor_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/data/at_ags_engine_icon.png` & `agstoolbox-0.3.6/src/agstoolbox/data/at_ags_engine_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/data/at_icon.png` & `agstoolbox-0.3.6/src/agstoolbox/data/at_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/data/at_icon_big.png` & `agstoolbox-0.3.6/src/agstoolbox/data/at_icon_big.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/data/exit_icon.png` & `agstoolbox-0.3.6/src/agstoolbox/data/exit_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/data/refresh_icon.png` & `agstoolbox-0.3.6/src/agstoolbox/data/refresh_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/data/settings_icon.png` & `agstoolbox-0.3.6/src/agstoolbox/data/settings_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/getdata.py` & `agstoolbox-0.3.6/src/agstoolbox/getdata.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/panels/at_mainpanel.py` & `agstoolbox-0.3.6/src/agstoolbox/panels/at_mainpanel.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/panels/at_settings_dialog.py` & `agstoolbox-0.3.6/src/agstoolbox/panels/at_settings_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtWidgets
 from PyQt6.QtWidgets import QDialog, QSizePolicy, QFormLayout, QHBoxLayout, QVBoxLayout, \
     QSpacerItem, QLabel, QDialogButtonBox
 
 from agstoolbox.core.settings.settings import Settings, ConstSettings
 from agstoolbox.wdgts.at_dirlist_wdgt import DirListWidget
 from agstoolbox.wdgts.at_single_dir_wdgt import DirEditWidget
 from agstoolbox.wdgts_utils.get_self_path import get_app_path
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/system/at_unique_application.py` & `agstoolbox-0.3.6/src/agstoolbox/system/at_unique_application.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/wdgts/at_dirlist_wdgt.py` & `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_dirlist_wdgt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations  # for python 3.8
 from pathlib import Path
 
-from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtWidgets
 from PyQt6.QtWidgets import QWidget, QFileDialog, QStyle, QFrame
 
 from agstoolbox.core.settings.settings import ConstSettings
 from agstoolbox.core.utils.file import dir_is_valid
 
 
 class DirListWidget(QWidget):
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/wdgts/at_single_dir_wdgt.py` & `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_single_dir_wdgt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations  # for python 3.8
 from pathlib import Path
 
-from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore
 from PyQt6.QtWidgets import QWidget, QFileDialog, QLineEdit, QPushButton, QHBoxLayout
 
 from agstoolbox.core.settings.settings import ConstSettings
 from agstoolbox.core.utils.file import dir_is_valid
 
 
 class DirEditWidget(QWidget):
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/wdgts/at_tree_item_project.py` & `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_item_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,60 +90,69 @@
         main_qgrid.addLayout(vbox, 0, 1)
 
         self.setLayout(main_qgrid)
 
     def quick_open_project(self):
         self.parent().parent().tools_tree.open_project_tool(self.project)
 
+    def quick_build_project(self):
+        self.parent().parent().tools_tree.build_project_tool(self.project)
+
     def mouseDoubleClickEvent(self, event):
         self.quick_open_project()
 
     def get_managed_editors(self) -> list[LocalAgsEditor]:
         return self.parent().parent().tools_tree.managed_editors_list
 
     def get_unmanaged_editors(self) -> list[LocalAgsEditor]:
         return self.parent().parent().tools_tree.unmanaged_editors_list
 
-    def set_managed_editors_menu(self, parent_menu: QtWidgets.QMenu = None) -> list[ActionEditorPair]:
+    def set_managed_editors_menu(self,
+                                 parent_menu: QtWidgets.QMenu = None) -> list[ActionEditorPair]:
         submenu = QtWidgets.QMenu("Open in Managed Editor", parent_menu)
         parent_menu.addMenu(submenu)
         editors = self.get_managed_editors()
         actions: list[ActionEditorPair] = list()
         for editor in editors:
             action = submenu.addAction(editor.name)
             actions.append(ActionEditorPair(action=action, editor=editor))
 
         return actions
 
-    def set_unmanaged_editors_menu(self, parent_menu: QtWidgets.QMenu = None) -> list[ActionEditorPair]:
+    def set_unmanaged_editors_menu(self,
+                                   parent_menu: QtWidgets.QMenu = None) -> list[ActionEditorPair]:
         submenu = QtWidgets.QMenu("Open in External Editor", parent_menu)
         parent_menu.addMenu(submenu)
         editors = self.get_unmanaged_editors()
         actions: list[ActionEditorPair] = list()
         for editor in editors:
             action = submenu.addAction(editor.name)
             actions.append(ActionEditorPair(action=action, editor=editor))
 
         return actions
 
     def contextMenuEvent(self, event):
         menu = QtWidgets.QMenu(self)
         quick_open_action = DefaultMenuQAction(menu, "Quick Open Project")
+        quick_build_action = menu.addAction("Quick Build Project")
         open_folder_action = menu.addAction("Open Folder in File Explorer")
         menu.addSeparator()
         managed_actions = self.set_managed_editors_menu(menu)
         unmanaged_actions = self.set_unmanaged_editors_menu(menu)
 
         action = menu.exec(self.mapToGlobal(event.pos()))
         if action == open_folder_action:
             ags_project_folder_in_explorer(self.project)
             return
         elif action == quick_open_action:
             self.quick_open_project()
             return
+        elif action == quick_build_action:
+            self.quick_build_project()
+            return
         else:
             for a_pair in managed_actions:
                 if a_pair.action == action:
                     ags_editor_load_project(a_pair.editor, self.project)
                     return
 
             for a_pair in unmanaged_actions:
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/wdgts/at_tree_item_tool.py` & `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_item_tool.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/wdgts/at_tree_projects_wdgt.py` & `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_projects_wdgt.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox/wdgts/at_tree_tools_wdgt.py` & `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_tools_wdgt.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from PyQt6 import QtCore
 from PyQt6.QtWidgets import QTreeWidget, QWidget, QAbstractScrollArea, QFrame, QTreeWidgetItem
 
 from agstoolbox.at_tasks import do_update_tools_downloads, do_update_tools_unmanaged, \
     do_update_tools_managed
 from agstoolbox.core.ags.ags_editor import LocalAgsEditor
-from agstoolbox.core.ags.ags_local_run import ags_editor_load_project
+from agstoolbox.core.ags.ags_local_run import ags_editor_load_project, ags_editor_build_project
 from agstoolbox.core.ags.game_project import GameProject
 from agstoolbox.core.version.version import Version
 from agstoolbox.wdgts.at_tree_item_tool import TreeItemTool_Header, ToolType, \
     TreeItemTool_Download, TreeItemTool_ExternallyInstalled, TreeItemTool_Managed
 
 
 class ToolsTree(QTreeWidget):
@@ -155,7 +155,20 @@
                 ags_editor_load_project(editor, game_project)
                 return
 
         for editor in self.unmanaged_editors_list:
             if editor.version.as_int == project_version.as_int:
                 ags_editor_load_project(editor, game_project)
                 return
+
+    def build_project_tool(self, game_project: GameProject):
+        project_version: Version = game_project.ags_editor_version
+
+        for editor in self.managed_editors_list:
+            if editor.version.as_int == project_version.as_int:
+                ags_editor_build_project(editor, game_project)
+                return
+
+        for editor in self.unmanaged_editors_list:
+            if editor.version.as_int == project_version.as_int:
+                ags_editor_build_project(editor, game_project)
+                return
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox/wdgts_utils/file_explorer.py` & `agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/file_explorer.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.5/src/agstoolbox.egg-info/PKG-INFO` & `agstoolbox-0.3.6/src/agstoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.5
+Version: 0.3.6
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.5
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.6
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `agstoolbox-0.3.5/src/agstoolbox.egg-info/SOURCES.txt` & `agstoolbox-0.3.6/src/agstoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

