# Comparing `tmp/agstoolbox-0.3.6.tar.gz` & `tmp/agstoolbox-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agstoolbox-0.3.6.tar", last modified: Sun Apr  9 16:06:07 2023, max compression
+gzip compressed data, was "agstoolbox-0.3.7.tar", last modified: Sun Apr  9 16:23:46 2023, max compression
```

## Comparing `agstoolbox-0.3.6.tar` & `agstoolbox-0.3.7.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.637252 agstoolbox-0.3.6/
--rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/AUTHORS
--rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/COPYING
--rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.6/LICENSE
--rw-rw-rw-   0        0        0      101 2023-04-08 20:06:59.000000 agstoolbox-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1189 2023-04-09 16:06:07.636251 agstoolbox-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.6/README.rst
--rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/agstoolbox
--rw-rw-rw-   0        0        0      416 2023-04-08 22:53:12.000000 agstoolbox-0.3.6/atbx
--rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 16:06:07.637252 agstoolbox-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1678 2023-04-09 02:05:29.000000 agstoolbox-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.396505 agstoolbox-0.3.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.431505 agstoolbox-0.3.6/src/agstoolbox/
--rw-rw-rw-   0        0        0      198 2023-04-09 16:02:35.000000 agstoolbox-0.3.6/src/agstoolbox/__init__.py
--rw-rw-rw-   0        0        0     1023 2023-04-09 03:43:47.000000 agstoolbox-0.3.6/src/agstoolbox/__main__.py
--rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.6/src/agstoolbox/at_icons.py
--rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.6/src/agstoolbox/at_tasks.py
--rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.6/src/agstoolbox/at_trayindicator.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.447043 agstoolbox-0.3.6/src/agstoolbox/core/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:22:20.000000 agstoolbox-0.3.6/src/agstoolbox/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.470252 agstoolbox-0.3.6/src/agstoolbox/core/ags/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/__init__.py
--rw-rw-rw-   0        0        0      340 2023-04-09 03:06:08.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_editor.py
--rw-rw-rw-   0        0        0   201168 2022-01-30 01:21:58.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_editor_validation_data.py
--rw-rw-rw-   0        0        0      673 2023-04-09 15:56:14.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_local_run.py
--rw-rw-rw-   0        0        0      361 2022-03-20 16:56:08.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/game_project.py
--rw-rw-rw-   0        0        0     3561 2023-04-09 03:08:16.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/get_game_projects.py
--rw-rw-rw-   0        0        0     2545 2023-04-07 21:27:44.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/get_local_ags_editors.py
--rw-rw-rw-   0        0        0     1328 2022-02-05 18:27:18.000000 agstoolbox-0.3.6/src/agstoolbox/core/ags/validate_ags_editor.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.482250 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/
--rw-rw-rw-   0        0        0        0 2023-04-08 03:10:57.000000 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/__init__.py
--rw-rw-rw-   0        0        0    13079 2023-04-09 15:46:59.000000 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/cmdline.py
--rw-rw-rw-   0        0        0      742 2023-04-08 17:11:05.000000 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/cmdline_download.py
--rw-rw-rw-   0        0        0     1506 2023-04-08 17:09:05.000000 agstoolbox-0.3.6/src/agstoolbox/core/cmdline/progress.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.495251 agstoolbox-0.3.6/src/agstoolbox/core/gh/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/__init__.py
--rw-rw-rw-   0        0        0     1093 2023-04-08 02:50:16.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/download_release.py
--rw-rw-rw-   0        0        0     1115 2023-04-09 03:46:16.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/install_release.py
--rw-rw-rw-   0        0        0     3474 2023-04-08 02:44:10.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/list_releases.py
--rw-rw-rw-   0        0        0      497 2023-04-09 03:35:53.000000 agstoolbox-0.3.6/src/agstoolbox/core/gh/release.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.508250 agstoolbox-0.3.6/src/agstoolbox/core/settings/
--rw-rw-rw-   0        0        0        0 2023-04-07 00:44:47.000000 agstoolbox-0.3.6/src/agstoolbox/core/settings/__init__.py
--rw-rw-rw-   0        0        0     5600 2023-04-08 22:11:07.000000 agstoolbox-0.3.6/src/agstoolbox/core/settings/settings.py
--rw-rw-rw-   0        0        0      287 2023-04-09 03:39:13.000000 agstoolbox-0.3.6/src/agstoolbox/core/settings/settings_data.py
--rw-rw-rw-   0        0        0     2286 2023-04-07 02:36:47.000000 agstoolbox-0.3.6/src/agstoolbox/core/settings/settings_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.555252 agstoolbox-0.3.6/src/agstoolbox/core/utils/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:23:07.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/__init__.py
--rw-rw-rw-   0        0        0      796 2023-04-07 01:04:11.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/basics.py
--rw-rw-rw-   0        0        0      797 2023-04-08 02:50:26.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/downloader.py
--rw-rw-rw-   0        0        0     4532 2023-04-09 15:55:35.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/file.py
--rw-rw-rw-   0        0        0      139 2022-01-27 21:57:07.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/math.py
--rw-rw-rw-   0        0        0       99 2023-04-05 02:07:05.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/open_in_browser.py
--rw-rw-rw-   0        0        0     1581 2022-01-29 21:55:33.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/pe.py
--rw-rw-rw-   0        0        0      246 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/singleton.py
--rw-rw-rw-   0        0        0     1836 2023-04-07 02:47:18.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/startup.py
--rw-rw-rw-   0        0        0      641 2023-04-08 16:41:22.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/systemdirs.py
--rw-rw-rw-   0        0        0     1008 2023-04-09 03:44:30.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/time.py
--rw-rw-rw-   0        0        0     1256 2023-04-09 03:44:51.000000 agstoolbox-0.3.6/src/agstoolbox/core/utils/win_registry.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.565250 agstoolbox-0.3.6/src/agstoolbox/core/version/
--rw-rw-rw-   0        0        0        0 2022-03-20 16:16:18.000000 agstoolbox-0.3.6/src/agstoolbox/core/version/__init__.py
--rw-rw-rw-   0        0        0      258 2023-04-08 01:38:27.000000 agstoolbox-0.3.6/src/agstoolbox/core/version/version.py
--rw-rw-rw-   0        0        0     3313 2023-04-08 01:43:53.000000 agstoolbox-0.3.6/src/agstoolbox/core/version/version_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.584250 agstoolbox-0.3.6/src/agstoolbox/data/
--rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.6/src/agstoolbox/data/at_ags_editor_icon.png
--rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/data/at_ags_engine_icon.png
--rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.6/src/agstoolbox/data/at_icon.png
--rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.6/src/agstoolbox/data/at_icon_big.png
--rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.6/src/agstoolbox/data/exit_icon.png
--rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.6/src/agstoolbox/data/refresh_icon.png
--rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.6/src/agstoolbox/data/settings_icon.png
--rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/getdata.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.591253 agstoolbox-0.3.6/src/agstoolbox/panels/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/panels/__init__.py
--rw-rw-rw-   0        0        0     5446 2023-04-07 02:51:49.000000 agstoolbox-0.3.6/src/agstoolbox/panels/at_mainpanel.py
--rw-rw-rw-   0        0        0     7533 2023-04-09 03:39:22.000000 agstoolbox-0.3.6/src/agstoolbox/panels/at_settings_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.601251 agstoolbox-0.3.6/src/agstoolbox/system/
--rw-rw-rw-   0        0        0        0 2023-04-02 19:34:00.000000 agstoolbox-0.3.6/src/agstoolbox/system/__init__.py
--rw-rw-rw-   0        0        0      394 2023-04-02 20:12:53.000000 agstoolbox-0.3.6/src/agstoolbox/system/at_runguard.py
--rw-rw-rw-   0        0        0     1210 2023-04-03 00:55:58.000000 agstoolbox-0.3.6/src/agstoolbox/system/at_unique_application.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.616250 agstoolbox-0.3.6/src/agstoolbox/wdgts/
--rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/__init__.py
--rw-rw-rw-   0        0        0     7381 2023-04-09 03:39:13.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_dirlist_wdgt.py
--rw-rw-rw-   0        0        0     2510 2023-04-09 03:40:47.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_single_dir_wdgt.py
--rw-rw-rw-   0        0        0     6290 2023-04-09 16:00:52.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_item_project.py
--rw-rw-rw-   0        0        0     8291 2023-04-05 02:14:45.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_item_tool.py
--rw-rw-rw-   0        0        0     1428 2023-04-04 01:42:57.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_projects_wdgt.py
--rw-rw-rw-   0        0        0     7062 2023-04-09 15:59:58.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_tools_wdgt.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.635250 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/
--rw-rw-rw-   0        0        0        0 2022-04-27 23:21:51.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/__init__.py
--rw-rw-rw-   0        0        0      358 2022-04-27 23:30:17.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/action_utils.py
--rw-rw-rw-   0        0        0      467 2022-04-27 23:52:03.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/ags_local_extra.py
--rw-rw-rw-   0        0        0      899 2022-04-27 23:49:42.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/file_explorer.py
--rw-rw-rw-   0        0        0      149 2023-04-02 23:02:36.000000 agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/get_self_path.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:06:07.446042 agstoolbox-0.3.6/src/agstoolbox.egg-info/
--rw-rw-rw-   0        0        0     1189 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2942 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 16:06:07.000000 agstoolbox-0.3.6/src/agstoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.566718 agstoolbox-0.3.7/
+-rw-rw-rw-   0        0        0       33 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/AUTHORS
+-rw-rw-rw-   0        0        0     1090 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/COPYING
+-rw-rw-rw-   0        0        0     1069 2023-04-07 14:40:56.000000 agstoolbox-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-04-08 20:06:59.000000 agstoolbox-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1189 2023-04-09 16:23:46.566718 agstoolbox-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-04-07 14:56:20.000000 agstoolbox-0.3.7/README.rst
+-rw-rw-rw-   0        0        0      386 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/agstoolbox
+-rw-rw-rw-   0        0        0      416 2023-04-08 22:53:12.000000 agstoolbox-0.3.7/atbx
+-rw-rw-rw-   0        0        0     1561 2023-04-08 03:22:39.000000 agstoolbox-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 16:23:46.566718 agstoolbox-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1678 2023-04-09 02:05:29.000000 agstoolbox-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.483056 agstoolbox-0.3.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.500058 agstoolbox-0.3.7/src/agstoolbox/
+-rw-rw-rw-   0        0        0      198 2023-04-09 16:22:49.000000 agstoolbox-0.3.7/src/agstoolbox/__init__.py
+-rw-rw-rw-   0        0        0     1023 2023-04-09 03:43:47.000000 agstoolbox-0.3.7/src/agstoolbox/__main__.py
+-rw-rw-rw-   0        0        0     1270 2022-02-06 18:41:53.000000 agstoolbox-0.3.7/src/agstoolbox/at_icons.py
+-rw-rw-rw-   0        0        0     4322 2023-04-07 02:56:06.000000 agstoolbox-0.3.7/src/agstoolbox/at_tasks.py
+-rw-rw-rw-   0        0        0     3874 2023-04-07 02:56:23.000000 agstoolbox-0.3.7/src/agstoolbox/at_trayindicator.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.515434 agstoolbox-0.3.7/src/agstoolbox/core/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:22:20.000000 agstoolbox-0.3.7/src/agstoolbox/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.521433 agstoolbox-0.3.7/src/agstoolbox/core/ags/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/src/agstoolbox/core/ags/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-04-09 03:06:08.000000 agstoolbox-0.3.7/src/agstoolbox/core/ags/ags_editor.py
+-rw-rw-rw-   0        0        0   201168 2022-01-30 01:21:58.000000 agstoolbox-0.3.7/src/agstoolbox/core/ags/ags_editor_validation_data.py
+-rw-rw-rw-   0        0        0      673 2023-04-09 15:56:14.000000 agstoolbox-0.3.7/src/agstoolbox/core/ags/ags_local_run.py
+-rw-rw-rw-   0        0        0      361 2022-03-20 16:56:08.000000 agstoolbox-0.3.7/src/agstoolbox/core/ags/game_project.py
+-rw-rw-rw-   0        0        0     3561 2023-04-09 03:08:16.000000 agstoolbox-0.3.7/src/agstoolbox/core/ags/get_game_projects.py
+-rw-rw-rw-   0        0        0     2545 2023-04-07 21:27:44.000000 agstoolbox-0.3.7/src/agstoolbox/core/ags/get_local_ags_editors.py
+-rw-rw-rw-   0        0        0     1328 2022-02-05 18:27:18.000000 agstoolbox-0.3.7/src/agstoolbox/core/ags/validate_ags_editor.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.524434 agstoolbox-0.3.7/src/agstoolbox/core/cmdline/
+-rw-rw-rw-   0        0        0        0 2023-04-08 03:10:57.000000 agstoolbox-0.3.7/src/agstoolbox/core/cmdline/__init__.py
+-rw-rw-rw-   0        0        0    13189 2023-04-09 16:20:46.000000 agstoolbox-0.3.7/src/agstoolbox/core/cmdline/cmdline.py
+-rw-rw-rw-   0        0        0      742 2023-04-08 17:11:05.000000 agstoolbox-0.3.7/src/agstoolbox/core/cmdline/cmdline_download.py
+-rw-rw-rw-   0        0        0     1506 2023-04-08 17:09:05.000000 agstoolbox-0.3.7/src/agstoolbox/core/cmdline/progress.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.528433 agstoolbox-0.3.7/src/agstoolbox/core/gh/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/src/agstoolbox/core/gh/__init__.py
+-rw-rw-rw-   0        0        0     1093 2023-04-08 02:50:16.000000 agstoolbox-0.3.7/src/agstoolbox/core/gh/download_release.py
+-rw-rw-rw-   0        0        0     1115 2023-04-09 03:46:16.000000 agstoolbox-0.3.7/src/agstoolbox/core/gh/install_release.py
+-rw-rw-rw-   0        0        0     3474 2023-04-08 02:44:10.000000 agstoolbox-0.3.7/src/agstoolbox/core/gh/list_releases.py
+-rw-rw-rw-   0        0        0      497 2023-04-09 03:35:53.000000 agstoolbox-0.3.7/src/agstoolbox/core/gh/release.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.532434 agstoolbox-0.3.7/src/agstoolbox/core/settings/
+-rw-rw-rw-   0        0        0        0 2023-04-07 00:44:47.000000 agstoolbox-0.3.7/src/agstoolbox/core/settings/__init__.py
+-rw-rw-rw-   0        0        0     5600 2023-04-08 22:11:07.000000 agstoolbox-0.3.7/src/agstoolbox/core/settings/settings.py
+-rw-rw-rw-   0        0        0      287 2023-04-09 03:39:13.000000 agstoolbox-0.3.7/src/agstoolbox/core/settings/settings_data.py
+-rw-rw-rw-   0        0        0     2286 2023-04-07 02:36:47.000000 agstoolbox-0.3.7/src/agstoolbox/core/settings/settings_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.541412 agstoolbox-0.3.7/src/agstoolbox/core/utils/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:23:07.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-04-07 01:04:11.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/basics.py
+-rw-rw-rw-   0        0        0      797 2023-04-08 02:50:26.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/downloader.py
+-rw-rw-rw-   0        0        0     4532 2023-04-09 15:55:35.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/file.py
+-rw-rw-rw-   0        0        0      139 2022-01-27 21:57:07.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/math.py
+-rw-rw-rw-   0        0        0       99 2023-04-05 02:07:05.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/open_in_browser.py
+-rw-rw-rw-   0        0        0     1581 2022-01-29 21:55:33.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/pe.py
+-rw-rw-rw-   0        0        0      246 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/singleton.py
+-rw-rw-rw-   0        0        0     1836 2023-04-07 02:47:18.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/startup.py
+-rw-rw-rw-   0        0        0      641 2023-04-08 16:41:22.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/systemdirs.py
+-rw-rw-rw-   0        0        0     1008 2023-04-09 03:44:30.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/time.py
+-rw-rw-rw-   0        0        0     1256 2023-04-09 03:44:51.000000 agstoolbox-0.3.7/src/agstoolbox/core/utils/win_registry.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.544510 agstoolbox-0.3.7/src/agstoolbox/core/version/
+-rw-rw-rw-   0        0        0        0 2022-03-20 16:16:18.000000 agstoolbox-0.3.7/src/agstoolbox/core/version/__init__.py
+-rw-rw-rw-   0        0        0      258 2023-04-08 01:38:27.000000 agstoolbox-0.3.7/src/agstoolbox/core/version/version.py
+-rw-rw-rw-   0        0        0     3313 2023-04-08 01:43:53.000000 agstoolbox-0.3.7/src/agstoolbox/core/version/version_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.544510 agstoolbox-0.3.7/src/agstoolbox/data/
+-rw-rw-rw-   0        0        0     6036 2022-02-06 18:38:23.000000 agstoolbox-0.3.7/src/agstoolbox/data/at_ags_editor_icon.png
+-rw-rw-rw-   0        0        0    53039 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/src/agstoolbox/data/at_ags_engine_icon.png
+-rw-rw-rw-   0        0        0     4571 2022-02-06 18:46:17.000000 agstoolbox-0.3.7/src/agstoolbox/data/at_icon.png
+-rw-rw-rw-   0        0        0    74585 2022-02-06 18:32:22.000000 agstoolbox-0.3.7/src/agstoolbox/data/at_icon_big.png
+-rw-rw-rw-   0        0        0     4036 2022-01-25 11:12:32.000000 agstoolbox-0.3.7/src/agstoolbox/data/exit_icon.png
+-rw-rw-rw-   0        0        0     2449 2022-01-25 11:11:19.000000 agstoolbox-0.3.7/src/agstoolbox/data/refresh_icon.png
+-rw-rw-rw-   0        0        0     6912 2022-01-25 11:17:17.000000 agstoolbox-0.3.7/src/agstoolbox/data/settings_icon.png
+-rw-rw-rw-   0        0        0      538 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/src/agstoolbox/getdata.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.544510 agstoolbox-0.3.7/src/agstoolbox/panels/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/src/agstoolbox/panels/__init__.py
+-rw-rw-rw-   0        0        0     5446 2023-04-07 02:51:49.000000 agstoolbox-0.3.7/src/agstoolbox/panels/at_mainpanel.py
+-rw-rw-rw-   0        0        0     7533 2023-04-09 03:39:22.000000 agstoolbox-0.3.7/src/agstoolbox/panels/at_settings_dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.554512 agstoolbox-0.3.7/src/agstoolbox/system/
+-rw-rw-rw-   0        0        0        0 2023-04-02 19:34:00.000000 agstoolbox-0.3.7/src/agstoolbox/system/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-02 20:12:53.000000 agstoolbox-0.3.7/src/agstoolbox/system/at_runguard.py
+-rw-rw-rw-   0        0        0     1210 2023-04-03 00:55:58.000000 agstoolbox-0.3.7/src/agstoolbox/system/at_unique_application.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.554512 agstoolbox-0.3.7/src/agstoolbox/wdgts/
+-rw-rw-rw-   0        0        0        0 2022-01-27 21:21:40.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts/__init__.py
+-rw-rw-rw-   0        0        0     7381 2023-04-09 03:39:13.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts/at_dirlist_wdgt.py
+-rw-rw-rw-   0        0        0     2510 2023-04-09 03:40:47.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts/at_single_dir_wdgt.py
+-rw-rw-rw-   0        0        0     6290 2023-04-09 16:00:52.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts/at_tree_item_project.py
+-rw-rw-rw-   0        0        0     8291 2023-04-05 02:14:45.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts/at_tree_item_tool.py
+-rw-rw-rw-   0        0        0     1428 2023-04-04 01:42:57.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts/at_tree_projects_wdgt.py
+-rw-rw-rw-   0        0        0     7062 2023-04-09 15:59:58.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts/at_tree_tools_wdgt.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.565719 agstoolbox-0.3.7/src/agstoolbox/wdgts_utils/
+-rw-rw-rw-   0        0        0        0 2022-04-27 23:21:51.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts_utils/__init__.py
+-rw-rw-rw-   0        0        0      358 2022-04-27 23:30:17.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts_utils/action_utils.py
+-rw-rw-rw-   0        0        0      467 2022-04-27 23:52:03.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts_utils/ags_local_extra.py
+-rw-rw-rw-   0        0        0      899 2022-04-27 23:49:42.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts_utils/file_explorer.py
+-rw-rw-rw-   0        0        0      149 2023-04-02 23:02:36.000000 agstoolbox-0.3.7/src/agstoolbox/wdgts_utils/get_self_path.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:46.514433 agstoolbox-0.3.7/src/agstoolbox.egg-info/
+-rw-rw-rw-   0        0        0     1189 2023-04-09 16:23:46.000000 agstoolbox-0.3.7/src/agstoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2942 2023-04-09 16:23:46.000000 agstoolbox-0.3.7/src/agstoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 16:23:46.000000 agstoolbox-0.3.7/src/agstoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-09 16:23:46.000000 agstoolbox-0.3.7/src/agstoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 16:23:46.000000 agstoolbox-0.3.7/src/agstoolbox.egg-info/top_level.txt
```

### Comparing `agstoolbox-0.3.6/COPYING` & `agstoolbox-0.3.7/COPYING`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/LICENSE` & `agstoolbox-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/PKG-INFO` & `agstoolbox-0.3.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.6
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.7
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `agstoolbox-0.3.6/README.rst` & `agstoolbox-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/pyproject.toml` & `agstoolbox-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/setup.py` & `agstoolbox-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/__main__.py` & `agstoolbox-0.3.7/src/agstoolbox/__main__.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/at_icons.py` & `agstoolbox-0.3.7/src/agstoolbox/at_icons.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/at_tasks.py` & `agstoolbox-0.3.7/src/agstoolbox/at_tasks.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/at_trayindicator.py` & `agstoolbox-0.3.7/src/agstoolbox/at_trayindicator.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_editor_validation_data.py` & `agstoolbox-0.3.7/src/agstoolbox/core/ags/ags_editor_validation_data.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/ags/ags_local_run.py` & `agstoolbox-0.3.7/src/agstoolbox/core/ags/ags_local_run.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/ags/get_game_projects.py` & `agstoolbox-0.3.7/src/agstoolbox/core/ags/get_game_projects.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/ags/get_local_ags_editors.py` & `agstoolbox-0.3.7/src/agstoolbox/core/ags/get_local_ags_editors.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/ags/validate_ags_editor.py` & `agstoolbox-0.3.7/src/agstoolbox/core/ags/validate_ags_editor.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/cmdline/cmdline.py` & `agstoolbox-0.3.7/src/agstoolbox/core/cmdline/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     editors = list_ags_editors_in_dir_list(unmanaged_dirs)
 
     for editor in editors:
         if editor.version.as_int == project_version.as_int:
             ags_editor_proj_command(editor, game_project)
             return
 
-    print("ERROR: Failed to find exact match of AGS Editor")
+    print("ERROR: Failed to find exact match of AGS Editor, wanted " + project_version.as_str)
 
 
 def at_cmd_list_projects(args):
     a_path: str | None = args.path
 
     if a_path is None:
         Settings().load()
@@ -183,29 +183,30 @@
     un_editors = list_ags_editors_in_dir_list(unmanaged_dirs)
 
     for editor in un_editors:
         if editor.version.as_int == editor_version.as_int:
             start_ags_editor(editor)
             return
 
-    print("WARN: Failed to find exact match of AGS Editor, will try to find a compatible one")
+    print("WARN: Failed to find exact match of AGS Editor( " + editor_version.as_str +
+          " ), will try to find a compatible one")
 
     filtered_editors = [ae for ae in editors if ae.version.family == editor_version.family]
     filtered_editors.sort(key=attrgetter("version.as_int"), reverse=True)
     if len(filtered_editors) >= 1:
         start_ags_editor(filtered_editors[0])
         return
 
     filtered_un_editors = [ae for ae in un_editors if ae.version.family == editor_version.family]
     filtered_un_editors.sort(key=attrgetter("version.as_int"), reverse=True)
     if len(filtered_un_editors) >= 1:
         start_ags_editor(filtered_un_editors[0])
         return
 
-    print("ERROR: No compatible AGS Editor available")
+    print("ERROR: No compatible AGS Editor available, wanted " + editor_version.family)
 
 
 def at_cmd_open_project(args):
     meta_cmd_project(args, ags_editor_load_project)
     return
```

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/cmdline/cmdline_download.py` & `agstoolbox-0.3.7/src/agstoolbox/core/cmdline/cmdline_download.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/cmdline/progress.py` & `agstoolbox-0.3.7/src/agstoolbox/core/cmdline/progress.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/gh/download_release.py` & `agstoolbox-0.3.7/src/agstoolbox/core/gh/download_release.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/gh/install_release.py` & `agstoolbox-0.3.7/src/agstoolbox/core/gh/install_release.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/gh/list_releases.py` & `agstoolbox-0.3.7/src/agstoolbox/core/gh/list_releases.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/settings/settings.py` & `agstoolbox-0.3.7/src/agstoolbox/core/settings/settings.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/settings/settings_utils.py` & `agstoolbox-0.3.7/src/agstoolbox/core/settings/settings_utils.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/utils/basics.py` & `agstoolbox-0.3.7/src/agstoolbox/core/utils/basics.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/utils/downloader.py` & `agstoolbox-0.3.7/src/agstoolbox/core/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/utils/file.py` & `agstoolbox-0.3.7/src/agstoolbox/core/utils/file.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/utils/pe.py` & `agstoolbox-0.3.7/src/agstoolbox/core/utils/pe.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/utils/startup.py` & `agstoolbox-0.3.7/src/agstoolbox/core/utils/startup.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/utils/systemdirs.py` & `agstoolbox-0.3.7/src/agstoolbox/core/utils/systemdirs.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/utils/time.py` & `agstoolbox-0.3.7/src/agstoolbox/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/utils/win_registry.py` & `agstoolbox-0.3.7/src/agstoolbox/core/utils/win_registry.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/core/version/version_utils.py` & `agstoolbox-0.3.7/src/agstoolbox/core/version/version_utils.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/data/at_ags_editor_icon.png` & `agstoolbox-0.3.7/src/agstoolbox/data/at_ags_editor_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/data/at_ags_engine_icon.png` & `agstoolbox-0.3.7/src/agstoolbox/data/at_ags_engine_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/data/at_icon.png` & `agstoolbox-0.3.7/src/agstoolbox/data/at_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/data/at_icon_big.png` & `agstoolbox-0.3.7/src/agstoolbox/data/at_icon_big.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/data/exit_icon.png` & `agstoolbox-0.3.7/src/agstoolbox/data/exit_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/data/refresh_icon.png` & `agstoolbox-0.3.7/src/agstoolbox/data/refresh_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/data/settings_icon.png` & `agstoolbox-0.3.7/src/agstoolbox/data/settings_icon.png`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/getdata.py` & `agstoolbox-0.3.7/src/agstoolbox/getdata.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/panels/at_mainpanel.py` & `agstoolbox-0.3.7/src/agstoolbox/panels/at_mainpanel.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/panels/at_settings_dialog.py` & `agstoolbox-0.3.7/src/agstoolbox/panels/at_settings_dialog.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/system/at_unique_application.py` & `agstoolbox-0.3.7/src/agstoolbox/system/at_unique_application.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_dirlist_wdgt.py` & `agstoolbox-0.3.7/src/agstoolbox/wdgts/at_dirlist_wdgt.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_single_dir_wdgt.py` & `agstoolbox-0.3.7/src/agstoolbox/wdgts/at_single_dir_wdgt.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_item_project.py` & `agstoolbox-0.3.7/src/agstoolbox/wdgts/at_tree_item_project.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_item_tool.py` & `agstoolbox-0.3.7/src/agstoolbox/wdgts/at_tree_item_tool.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_projects_wdgt.py` & `agstoolbox-0.3.7/src/agstoolbox/wdgts/at_tree_projects_wdgt.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/wdgts/at_tree_tools_wdgt.py` & `agstoolbox-0.3.7/src/agstoolbox/wdgts/at_tree_tools_wdgt.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox/wdgts_utils/file_explorer.py` & `agstoolbox-0.3.7/src/agstoolbox/wdgts_utils/file_explorer.py`

 * *Files identical despite different names*

### Comparing `agstoolbox-0.3.6/src/agstoolbox.egg-info/PKG-INFO` & `agstoolbox-0.3.7/src/agstoolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agstoolbox
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utility to help manage Adventure Game Studio Projects and Editors.
 Home-page: https://github.com/ericoporto/agstoolbox
-Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.6
+Download-URL: https://github.com/ericoporto/agstoolbox/tarball/0.3.7
 Author: erico
 Author-email: eri0onpm@gmail.com
 License: MIT
 Keywords: AGS Toolbox,Adventure Game Studio,development,ags,Game Development,gamedev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
```

### Comparing `agstoolbox-0.3.6/src/agstoolbox.egg-info/SOURCES.txt` & `agstoolbox-0.3.7/src/agstoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

