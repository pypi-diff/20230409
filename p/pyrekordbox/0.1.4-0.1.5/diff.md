# Comparing `tmp/pyrekordbox-0.1.4.tar.gz` & `tmp/pyrekordbox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrekordbox-0.1.4.tar", last modified: Sun Oct 30 21:31:15 2022, max compression
+gzip compressed data, was "pyrekordbox-0.1.5.tar", last modified: Sun Apr  9 09:08:18 2023, max compression
```

## Comparing `pyrekordbox-0.1.4.tar` & `pyrekordbox-0.1.5.tar`

### file list

```diff
@@ -1,607 +1,608 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.721064 pyrekordbox-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5221 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/export/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.testdata/export/PIONEER/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/DEVSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/DJMMYSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/MYSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P016/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P016/0000875E/
--rw-r--r--   0 runner    (1001) docker     (121)    81410 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     5324 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    86386 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P017/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P017/00009B77/
--rw-r--r--   0 runner    (1001) docker     (121)     7105 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10801 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P019/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/
--rw-r--r--   0 runner    (1001) docker     (121)     6154 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     9850 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P021/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/
--rw-r--r--   0 runner    (1001) docker     (121)     7220 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10916 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P043/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P043/00011517/
--rw-r--r--   0 runner    (1001) docker     (121)     6385 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10081 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P053/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.681063 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/
--rw-r--r--   0 runner    (1001) docker     (121)    61436 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    65998 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/export/PIONEER/rekordbox/
--rw-r--r--   0 runner    (1001) docker     (121)   184320 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/rekordbox/export.pdb
--rw-r--r--   0 runner    (1001) docker     (121)    81920 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/export/PIONEER/rekordbox/exportExt.pdb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/DEVSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/DJMMYSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/MYSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/beat_fx_quantize/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/beat_fx_quantize/off/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/beat_fx_quantize/off/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/beat_fx_quantize/on/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/beat_fx_quantize/on/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.665063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve/linear/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve/linear/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve/steep_bottom/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve/steep_bottom/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve/steep_top/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve/steep_top/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve_long/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve_long/exponential/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve_long/exponential/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve_long/linear/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve_long/linear/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve_long/smooth/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/channel_fader_curve_long/smooth/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/cross_fader_curve/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/cross_fader_curve/constant/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/cross_fader_curve/constant/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/cross_fader_curve/fast_cut/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/cross_fader_curve/fast_cut/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/cross_fader_curve/slow_cut/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/cross_fader_curve/slow_cut/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/five/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/five/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/four/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/four/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/one/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/one/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/three/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/three/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/two/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/two/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/white/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/display_brightness/white/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_mono_split/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_mono_split/mono_split/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_mono_split/mono_split/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_mono_split/stereo/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_mono_split/stereo/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_pre_eq/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_pre_eq/post_eq/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_pre_eq/post_eq/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_pre_eq/pre_eq/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/headphones_pre_eq/pre_eq/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/indicator_brightness/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/indicator_brightness/one/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/indicator_brightness/one/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/indicator_brightness/three/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/indicator_brightness/three/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/indicator_brightness/two/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/indicator_brightness/two/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/mic_low_cut/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/mic_low_cut/off/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/mic_low_cut/off/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/mic_low_cut/on/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/mic_low_cut/on/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_button_type/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_button_type/toggle/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_button_type/toggle/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_button_type/trigger/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_button_type/trigger/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/eight/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/eight/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/eleven/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/eleven/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/fifteen/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/fifteen/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/five/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/five/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/four/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/four/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/fourteen/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/fourteen/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/nine/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/nine/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/one/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/one/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/seven/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/seven/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/six/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/six/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/sixteen/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/sixteen/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.685063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/ten/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/ten/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/thirteen/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/thirteen/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/three/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/three/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/twelve/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/twelve/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/two/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/midi_channel/two/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/minus_12db/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/minus_12db/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/minus_18db/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/minus_18db/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/minus_24db/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/minus_24db/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/minus_6db/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_level/minus_6db/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_mode/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_mode/advanced/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_mode/advanced/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_mode/normal/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/djmmysetting/talk_over_mode/normal/DJMMYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/memory/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/memory/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_36db/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_36db/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_42db/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_42db/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_48db/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_48db/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_54db/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_54db/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_60db/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_60db/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_66db/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_66db/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_72db/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_72db/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_78db/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/auto_cue_level/minus_78db/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/disc_slot_illumination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/disc_slot_illumination/bright/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/disc_slot_illumination/bright/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/disc_slot_illumination/dark/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/disc_slot_illumination/dark/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/disc_slot_illumination/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/disc_slot_illumination/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.669063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/eject_lock/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/eject_lock/lock/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/eject_lock/lock/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/eject_lock/unlock/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/eject_lock/unlock/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_autoload/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_autoload/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_autoload/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_autoload/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_autoload/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_autoload/rekordbox/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_autoload/rekordbox/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_color/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_color/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_color/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_color/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/hotcue_color/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_mode/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_mode/cdj/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_mode/cdj/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_mode/vinyl/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_mode/vinyl/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_brightness/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_brightness/bright/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_brightness/bright/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_brightness/dark/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_brightness/dark/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_brightness/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_brightness/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_indicator/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_indicator/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_indicator/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_indicator/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/jog_ring_indicator/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/chinese_simplified/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/chinese_simplified/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/chinese_traditional/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/chinese_traditional/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/czech/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/czech/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/danish/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/danish/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/dutch/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/dutch/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.689063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/english/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/english/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/french/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/french/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/german/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/german/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/greek/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/greek/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/hungarian/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/hungarian/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/italian/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/italian/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/japanese/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/japanese/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/korean/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/korean/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/portuguese/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/portuguese/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/russian/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/russian/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/spanish/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/spanish/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/swedish/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/swedish/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/turkish/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/language/turkish/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/five/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/five/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/four/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/four/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/one/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/one/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/three/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/three/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/two/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/lcd_brightness/two/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/master_tempo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/master_tempo/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/master_tempo/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/master_tempo/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/master_tempo/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/needle_lock/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/needle_lock/lock/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/needle_lock/lock/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/needle_lock/unlock/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/needle_lock/unlock/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/on_air_display/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/on_air_display/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/on_air_display/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/on_air_display/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/on_air_display/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/phase_meter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/phase_meter/type1/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/phase_meter/type1/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/phase_meter/type2/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/phase_meter/type2/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/play_mode/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/play_mode/continue_/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/play_mode/continue_/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/play_mode/single/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/play_mode/single/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/eighth/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/eighth/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/half/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/half/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/one/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/one/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/quarter/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/quantize_beat_value/quarter/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/slip_flashing/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/slip_flashing/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/slip_flashing/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/slip_flashing/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/slip_flashing/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/sync/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/sync/off/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/sync/off/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/sync/on/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/sync/on/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/six/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/six/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/sixteen/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/sixteen/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/ten/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/ten/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/wide/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/tempo_range/wide/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.673063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/time_mode/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/time_mode/elapsed/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/time_mode/elapsed/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/time_mode/remain/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting/time_mode/remain/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.693064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/eight/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/eight/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/four/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/four/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/half/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/half/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/one/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/one/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/sixteen/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/sixteen/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/sixtyfour/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/sixtyfour/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/thirtytwo/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/thirtytwo/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/two/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/beat_jump_beat_value/two/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/artwork/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/artwork/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/auto/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/auto/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/info/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/info/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/simple/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_display_mode/simple/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/five/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/five/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/four/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/four/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/one/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/one/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/three/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/three/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/two/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/jog_lcd_brightness/two/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/four/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/four/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/one/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/one/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/three/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/three/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/two/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/pad_button_brightness/two/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/vinyl_speed_adjust/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/vinyl_speed_adjust/release/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/vinyl_speed_adjust/release/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/vinyl_speed_adjust/touch/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/vinyl_speed_adjust/touch/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/vinyl_speed_adjust/touch_release/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/vinyl_speed_adjust/touch_release/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform/phase_meter/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform/phase_meter/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform/waveform/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform/waveform/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform_divisions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform_divisions/phrase/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform_divisions/phrase/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform_divisions/time_scale/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/mysettings/mysetting2/waveform_divisions/time_scale/MYSETTING2.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/rekordbox 5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/DEVSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     9480 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/ExtData.edb
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/MYSETTING.DAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10950 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10115 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/
--rw-r--r--   0 runner    (1001) docker     (121)     4428 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    65694 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.697064 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     9884 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.701063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/
--rw-r--r--   0 runner    (1001) docker     (121)     5316 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    85890 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.701063 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/
--rw-r--r--   0 runner    (1001) docker     (121)     2404 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10835 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/ANLZ0000.EXT
--rw-r--r--   0 runner    (1001) docker     (121)    19936 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/datafile.edb
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/masterPlaylists3.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4837 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/database.xml
--rw-r--r--   0 runner    (1001) docker     (121)    19936 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 5/datafile.edb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.701063 pyrekordbox-0.1.4/.testdata/rekordbox 6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.705064 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/DEVSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/DJMMYSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/MYSETTING.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/MYSETTING2.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/masterPlaylists3.xml
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/masterPlaylists6.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.705064 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/
--rw-r--r--   0 runner    (1001) docker     (121)     6315 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10011 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.705064 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/
--rw-r--r--   0 runner    (1001) docker     (121)     7150 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10846 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.705064 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/
--rw-r--r--   0 runner    (1001) docker     (121)    61370 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    65932 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.705064 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/
--rw-r--r--   0 runner    (1001) docker     (121)     7035 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    10731 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.705064 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/
--rw-r--r--   0 runner    (1001) docker     (121)     6084 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)     9780 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.EXT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.705064 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/
--rw-r--r--   0 runner    (1001) docker     (121)    81344 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.2EX
--rw-r--r--   0 runner    (1001) docker     (121)     5258 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.DAT
--rw-r--r--   0 runner    (1001) docker     (121)    86320 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.EXT
--rw-r--r--   0 runner    (1001) docker     (121)     4164 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/database.xml
--rw-r--r--   0 runner    (1001) docker     (121)  1470464 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/master_locked.db
--rw-r--r--   0 runner    (1001) docker     (121)  1470464 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/.testdata/rekordbox 6/master_unlocked.db
--rw-r--r--   0 runner    (1001) docker     (121)     8652 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3276 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     7570 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.705064 pyrekordbox-0.1.4/Libs/
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/Libs/LICENSE_SQLCipher
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.709064 pyrekordbox-0.1.4/Libs/sqlcipher_py38/
--rw-r--r--   0 runner    (1001) docker     (121)  2523136 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/Libs/sqlcipher_py38/libcrypto-1_1.dll
--rw-r--r--   0 runner    (1001) docker     (121)   531456 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/Libs/sqlcipher_py38/libssl-1_1.dll
--rw-r--r--   0 runner    (1001) docker     (121)  1825792 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/Libs/sqlcipher_py38/sqlcipher.dll
--rw-r--r--   0 runner    (1001) docker     (121)    15455 2022-10-30 21:31:15.721064 pyrekordbox-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14099 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.713064 pyrekordbox-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.713064 pyrekordbox-0.1.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.713064 pyrekordbox-0.1.4/docs/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_beat.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12320 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_file.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8155 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pco2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8682 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pcob.svg
--rw-r--r--   0 runner    (1001) docker     (121)    24904 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pcp2.svg
--rw-r--r--   0 runner    (1001) docker     (121)    16473 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pcpt.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7124 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_ppth.svg
--rw-r--r--   0 runner    (1001) docker     (121)    18386 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pqt2.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13774 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pqt2_2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8141 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pqtz.svg
--rw-r--r--   0 runner    (1001) docker     (121)    11684 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pssi.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12095 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pssi_entry.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7284 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pvbr.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7566 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwav.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8389 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv3.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8173 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv4.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8173 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv5.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5648 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv5_entry.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7577 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv6.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8173 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv7.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7128 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwvc.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6188 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/images/anlz_tag.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/docs/source/_static/logos/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/docs/source/_static/logos/dark/
--rw-r--r--   0 runner    (1001) docker     (121)     3079 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/logos/dark/logo_primary.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/docs/source/_static/logos/light/
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/logos/light/logo_primary.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/docs/source/_static/logos/mid/
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_static/logos/mid/logo_primary.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.677063 pyrekordbox-0.1.4/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/docs/source/_templates/apidoc/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_templates/apidoc/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_templates/apidoc/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_templates/apidoc/toc.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6199 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/development/changes.md
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/development/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/docs/source/formats/
--rw-r--r--   0 runner    (1001) docker     (121)    18440 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/formats/anlz.rst
--rw-r--r--   0 runner    (1001) docker     (121)    27707 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/formats/db6.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9935 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/formats/mysetting.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/formats/xml.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7565 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/installation.md
--rw-r--r--   0 runner    (1001) docker     (121)     5489 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/tutorial/anlz.md
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/tutorial/configuration.md
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/tutorial/db6.md
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/tutorial/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/tutorial/mysetting.md
--rw-r--r--   0 runner    (1001) docker     (121)     6414 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/docs/source/tutorial/xml.md
--rw-r--r--   0 runner    (1001) docker     (121)     4813 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/install_pysqlcipher.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/pyrekordbox/
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-30 21:31:15.000000 pyrekordbox-0.1.4/pyrekordbox/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/pyrekordbox/anlz/
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/anlz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5143 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/anlz/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     8010 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/anlz/structs.py
--rw-r--r--   0 runner    (1001) docker     (121)    14117 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/anlz/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     8291 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.721064 pyrekordbox-0.1.4/pyrekordbox/db6/
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/db6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29467 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/db6/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     3137 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/db6/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    28290 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/db6/tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.721064 pyrekordbox-0.1.4/pyrekordbox/mysettings/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/mysettings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13285 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/mysettings/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     8495 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/mysettings/structs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11138 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    37476 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/pyrekordbox/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.717064 pyrekordbox-0.1.4/pyrekordbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15455 2022-10-30 21:31:15.000000 pyrekordbox-0.1.4/pyrekordbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18688 2022-10-30 21:31:15.000000 pyrekordbox-0.1.4/pyrekordbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 21:31:15.000000 pyrekordbox-0.1.4/pyrekordbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 21:30:55.000000 pyrekordbox-0.1.4/pyrekordbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-10-30 21:31:15.000000 pyrekordbox-0.1.4/pyrekordbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-30 21:31:15.000000 pyrekordbox-0.1.4/pyrekordbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-10-30 21:31:15.721064 pyrekordbox-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 21:31:15.721064 pyrekordbox-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5805 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/tests/test_anlz.py
--rw-r--r--   0 runner    (1001) docker     (121)     7396 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/tests/test_db6.py
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/tests/test_mysetting.py
--rw-r--r--   0 runner    (1001) docker     (121)    15899 2022-10-30 21:30:45.000000 pyrekordbox-0.1.4/tests/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.232222 pyrekordbox-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.184222 pyrekordbox-0.1.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.184222 pyrekordbox-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/export/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.184222 pyrekordbox-0.1.5/.testdata/export/PIONEER/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/DEVSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/DJMMYSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/MYSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P016/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.184222 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P016/0000875E/
+-rw-r--r--   0 runner    (1001) docker     (123)    81410 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    86386 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P017/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P017/00009B77/
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P021/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P043/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P043/00011517/
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P053/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/
+-rw-r--r--   0 runner    (1001) docker     (123)    61436 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    65998 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/export/PIONEER/rekordbox/
+-rw-r--r--   0 runner    (1001) docker     (123)   184320 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/rekordbox/export.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/export/PIONEER/rekordbox/exportExt.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/mysettings/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/DEVSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/DJMMYSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/MYSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.160221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/beat_fx_quantize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/beat_fx_quantize/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/beat_fx_quantize/off/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/beat_fx_quantize/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/beat_fx_quantize/on/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve/linear/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve/steep_bottom/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve/steep_bottom/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve/steep_top/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve/steep_top/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve_long/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.188222 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve_long/exponential/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve_long/exponential/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve_long/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve_long/linear/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve_long/smooth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/channel_fader_curve_long/smooth/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/cross_fader_curve/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/cross_fader_curve/constant/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/cross_fader_curve/constant/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/cross_fader_curve/fast_cut/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/cross_fader_curve/fast_cut/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/cross_fader_curve/slow_cut/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/cross_fader_curve/slow_cut/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/five/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/five/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/four/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/four/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/one/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/one/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/three/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/three/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/two/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/two/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/white/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/display_brightness/white/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_mono_split/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_mono_split/mono_split/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_mono_split/mono_split/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_mono_split/stereo/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_mono_split/stereo/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_pre_eq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_pre_eq/post_eq/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_pre_eq/post_eq/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_pre_eq/pre_eq/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/headphones_pre_eq/pre_eq/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/indicator_brightness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/indicator_brightness/one/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/indicator_brightness/one/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/indicator_brightness/three/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/indicator_brightness/three/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/indicator_brightness/two/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/indicator_brightness/two/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/mic_low_cut/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/mic_low_cut/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/mic_low_cut/off/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/mic_low_cut/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/mic_low_cut/on/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.164221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_button_type/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_button_type/toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_button_type/toggle/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_button_type/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_button_type/trigger/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/eight/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/eight/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/eleven/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/eleven/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/fifteen/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/fifteen/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/five/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/five/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/four/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/four/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/fourteen/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/fourteen/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/nine/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/nine/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/one/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/one/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/seven/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/seven/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/six/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/six/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.192221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/sixteen/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/sixteen/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/ten/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/ten/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/thirteen/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/thirteen/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/three/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/three/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/twelve/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/twelve/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/two/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/midi_channel/two/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/minus_12db/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/minus_12db/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/minus_18db/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/minus_18db/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/minus_24db/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/minus_24db/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/minus_6db/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_level/minus_6db/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_mode/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_mode/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_mode/advanced/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_mode/normal/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/djmmysetting/talk_over_mode/normal/DJMMYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/memory/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_36db/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_36db/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_42db/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_42db/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_48db/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_48db/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_54db/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_54db/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_60db/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_60db/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_66db/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_66db/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_72db/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_72db/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_78db/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/auto_cue_level/minus_78db/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/disc_slot_illumination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/disc_slot_illumination/bright/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/disc_slot_illumination/bright/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/disc_slot_illumination/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/disc_slot_illumination/dark/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/disc_slot_illumination/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/disc_slot_illumination/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/eject_lock/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/eject_lock/lock/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/eject_lock/lock/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/eject_lock/unlock/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/eject_lock/unlock/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_autoload/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_autoload/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_autoload/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_autoload/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_autoload/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_autoload/rekordbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_autoload/rekordbox/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_color/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_color/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_color/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.196221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_color/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/hotcue_color/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_mode/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_mode/cdj/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_mode/cdj/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_mode/vinyl/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_mode/vinyl/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_brightness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_brightness/bright/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_brightness/bright/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_brightness/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_brightness/dark/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_brightness/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_brightness/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.168221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_indicator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_indicator/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_indicator/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_indicator/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/jog_ring_indicator/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.172222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/chinese_simplified/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/chinese_simplified/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/chinese_traditional/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/chinese_traditional/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/czech/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/czech/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/danish/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/danish/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/dutch/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/dutch/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/english/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/english/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/french/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/french/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/german/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/german/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/greek/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/greek/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/hungarian/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/hungarian/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/italian/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/italian/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/japanese/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/japanese/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/korean/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/korean/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/portuguese/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/portuguese/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/russian/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/russian/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/spanish/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/spanish/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/swedish/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/swedish/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/turkish/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/language/turkish/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.172222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/five/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/five/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/four/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/four/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/one/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/one/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/three/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/three/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/two/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/lcd_brightness/two/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.172222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/master_tempo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/master_tempo/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/master_tempo/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/master_tempo/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/master_tempo/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.172222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/needle_lock/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.200222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/needle_lock/lock/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/needle_lock/lock/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/needle_lock/unlock/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/needle_lock/unlock/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.172222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/on_air_display/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/on_air_display/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/on_air_display/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/on_air_display/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/on_air_display/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.172222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/phase_meter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/phase_meter/type1/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/phase_meter/type1/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/phase_meter/type2/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/phase_meter/type2/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.172222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/play_mode/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/play_mode/continue_/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/play_mode/continue_/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/play_mode/single/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/play_mode/single/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.172222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/eighth/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/eighth/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/half/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/half/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/one/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/one/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/quarter/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/quantize_beat_value/quarter/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/slip_flashing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/slip_flashing/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/slip_flashing/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/slip_flashing/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/slip_flashing/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/sync/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/sync/off/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/sync/off/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/sync/on/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/sync/on/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/six/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/six/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/sixteen/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/sixteen/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/ten/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/ten/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/wide/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/tempo_range/wide/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/time_mode/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/time_mode/elapsed/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/time_mode/elapsed/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/time_mode/remain/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting/time_mode/remain/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/eight/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/eight/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/four/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/four/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/half/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/half/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/one/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/one/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/sixteen/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/sixteen/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/sixtyfour/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/sixtyfour/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/thirtytwo/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/thirtytwo/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/two/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/beat_jump_beat_value/two/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/artwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/artwork/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.204222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/auto/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/info/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_display_mode/simple/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/five/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/five/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/four/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/four/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/one/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/one/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/three/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/three/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/two/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/jog_lcd_brightness/two/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/four/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/four/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/one/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/one/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/three/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/three/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/two/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/pad_button_brightness/two/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/vinyl_speed_adjust/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/vinyl_speed_adjust/release/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/vinyl_speed_adjust/release/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/vinyl_speed_adjust/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/vinyl_speed_adjust/touch/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/vinyl_speed_adjust/touch_release/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/vinyl_speed_adjust/touch_release/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.176221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform/phase_meter/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform/phase_meter/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform/waveform/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform/waveform/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform_divisions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform_divisions/phrase/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform_divisions/phrase/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform_divisions/time_scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/mysettings/mysetting2/waveform_divisions/time_scale/MYSETTING2.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/rekordbox 5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/DEVSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/ExtData.edb
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/MYSETTING.DAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.208222 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    65694 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.212222 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.212222 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    85890 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.212222 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/ANLZ0000.EXT
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/datafile.edb
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/masterPlaylists3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/database.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 5/datafile.edb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.212222 pyrekordbox-0.1.5/.testdata/rekordbox 6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.216222 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/DEVSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/DJMMYSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/MYSETTING.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/MYSETTING2.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/masterPlaylists3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/masterPlaylists6.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.216222 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.216222 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.216222 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/
+-rw-r--r--   0 runner    (1001) docker     (123)    61370 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    65932 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.216222 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.216222 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.EXT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.216222 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/
+-rw-r--r--   0 runner    (1001) docker     (123)    81344 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.2EX
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)    86320 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.EXT
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/database.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  1470464 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/master_locked.db
+-rw-r--r--   0 runner    (1001) docker     (123)  1470464 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/.testdata/rekordbox 6/master_unlocked.db
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.216222 pyrekordbox-0.1.5/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/Libs/LICENSE_SQLCipher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.220222 pyrekordbox-0.1.5/Libs/sqlcipher_py38/
+-rw-r--r--   0 runner    (1001) docker     (123)  2523136 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/Libs/sqlcipher_py38/libcrypto-1_1.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   531456 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/Libs/sqlcipher_py38/libssl-1_1.dll
+-rw-r--r--   0 runner    (1001) docker     (123)  1825792 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/Libs/sqlcipher_py38/sqlcipher.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-04-09 09:08:18.232222 pyrekordbox-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.224222 pyrekordbox-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.224222 pyrekordbox-0.1.5/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.224222 pyrekordbox-0.1.5/docs/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_beat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pco2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pcob.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pcp2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pcpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_ppth.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pqt2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pqt2_2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pqtz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pssi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pssi_entry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pvbr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwav.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv5_entry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwvc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/images/anlz_tag.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/docs/source/_static/logos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.224222 pyrekordbox-0.1.5/docs/source/_static/logos/dark/
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/logos/dark/logo_primary.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/docs/source/_static/logos/light/
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/logos/light/logo_primary.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/docs/source/_static/logos/mid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_static/logos/mid/logo_primary.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.180221 pyrekordbox-0.1.5/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/docs/source/_templates/apidoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_templates/apidoc/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_templates/apidoc/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_templates/apidoc/toc.rst_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/development/changes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/development/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/docs/source/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)    18440 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/formats/anlz.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    27707 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/formats/db6.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/formats/mysetting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/formats/xml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/tutorial/anlz.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/tutorial/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/tutorial/db6.md
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/tutorial/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/tutorial/mysetting.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/docs/source/tutorial/xml.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/install_pysqlcipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/pyrekordbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 09:08:17.000000 pyrekordbox-0.1.5/pyrekordbox/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/pyrekordbox/anlz/
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/anlz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/anlz/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/anlz/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/anlz/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.232222 pyrekordbox-0.1.5/pyrekordbox/db6/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/db6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30010 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/db6/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/db6/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28290 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/db6/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.232222 pyrekordbox-0.1.5/pyrekordbox/mysettings/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/mysettings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/mysettings/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/mysettings/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37473 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/pyrekordbox/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.228222 pyrekordbox-0.1.5/pyrekordbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-04-09 09:08:17.000000 pyrekordbox-0.1.5/pyrekordbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-04-09 09:08:18.000000 pyrekordbox-0.1.5/pyrekordbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:08:17.000000 pyrekordbox-0.1.5/pyrekordbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:07:57.000000 pyrekordbox-0.1.5/pyrekordbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-09 09:08:17.000000 pyrekordbox-0.1.5/pyrekordbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 09:08:17.000000 pyrekordbox-0.1.5/pyrekordbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-09 09:08:18.232222 pyrekordbox-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:08:18.232222 pyrekordbox-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/tests/test_anlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/tests/test_db6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/tests/test_mysetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-09 09:07:46.000000 pyrekordbox-0.1.5/tests/test_xml.py
```

### Comparing `pyrekordbox-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md` & `pyrekordbox-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.github/workflows/pypi-publish.yml` & `pyrekordbox-0.1.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.github/workflows/tests.yml` & `pyrekordbox-0.1.5/.github/workflows/tests.yml`

 * *Files 16% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     needs: code-change
     if: ${{ needs.code-change.outputs.should_skip != 'true'}}
 
     strategy:
       matrix:
         os: [windows-latest, macos-latest]
         python-version: ["3.7", "3.11"]  # check oldest and latest supported version
-        other-os: [false]
+        other-os: [true]
 
     runs-on: ${{ matrix.os }}
-    continue-on-error: ${{ matrix.other-os }}  # don't cancel due to OS specific failures
+    continue-on-error: true  # don't cancel due to OS specific failures
     env:
       OS: ${{ matrix.os }}
       PYTHON: ${{ matrix.python-version }}
 
     steps:
     - uses: actions/checkout@v3
       with:
```

### Comparing `pyrekordbox-0.1.4/.gitignore` & `pyrekordbox-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.pre-commit-config.yaml` & `pyrekordbox-0.1.5/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.3.0
+      rev: v4.4.0
       hooks:
           - id: end-of-file-fixer
           - id: trailing-whitespace
             exclude: CHANGELOG.md
           - id: mixed-line-ending
           - id: check-toml
           - id: check-yaml
 
     - repo: https://github.com/psf/black
-      rev: 22.10.0
+      rev: 22.12.0
       hooks:
         - id: black
           args: [ --safe ]
 
     - repo: https://github.com/PyCQA/flake8
-      rev: 5.0.4
+      rev: 6.0.0
       hooks:
           - id: flake8
             args: [--config, setup.cfg]
```

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P017/00009B77/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P019/00020AA9/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P021/00006D2B/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P043/00011517/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/USBANLZ/P053/0001D21F/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/rekordbox/export.pdb` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/rekordbox/export.pdb`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/export/PIONEER/rekordbox/exportExt.pdb` & `pyrekordbox-0.1.5/.testdata/export/PIONEER/rekordbox/exportExt.pdb`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/ExtData.edb` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/ExtData.edb`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P002/00009C2E/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P02B/00023587/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P035/00027763/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P038/0002AAA0/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P068/00012CA2/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/PIONEER/USBANLZ/P076/00013B6E/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/backup/datafile.edb` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/backup/datafile.edb`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/database.xml` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/database.xml`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 5/datafile.edb` & `pyrekordbox-0.1.5/.testdata/rekordbox 5/datafile.edb`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/003/c9538-33bc-4ca7-b6c7-e63ebf9a96f8/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/104/c82cc-661c-4f30-ab60-51ce1effeeed/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/36d/ad2b4-5d4e-4b94-9a5d-a5bb241aee4b/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/731/0104f-53cb-453e-8b83-e0dfd5cff825/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/c8b/ac74a-bbfc-4fce-8fb8-50aa4e974273/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.2EX` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.2EX`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.DAT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.DAT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.EXT` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/backup/share/PIONEER/USBANLZ/e35/fa187-3f34-47e2-9880-2b33cb8d1304/ANLZ0000.EXT`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/database.xml` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/database.xml`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/master_locked.db` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/master_locked.db`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/.testdata/rekordbox 6/master_unlocked.db` & `pyrekordbox-0.1.5/.testdata/rekordbox 6/master_unlocked.db`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/CHANGELOG.md` & `pyrekordbox-0.1.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # What's New
 
+<a name="0.1.5"></a>
+## [0.1.5] - 2023-09-04
+
+This release contains bug fixes and improves error handling.
+
+### Improvements/Bug Fixes
+
+- **Improve RBv6 configuration handling**  
+  Don't warn if no Rekordbox installation was found instead raise an error if no config exists when opening the `Rekordbox6Database`.
+- **improve error handling for incompatible RB versions ([#64](https://github.com/dylanljones/pyrekordbox/issues/64))**
+- **fix sqlalchemy iso-format error**  
+  Using SQLAlchemy v2 results in ValueError's.
+- **don't fail on incompatible Rekordbox database**  
+  This allows the library to be used with reduced functionality, for example, RekordboxXML still works.
+
 <a name="0.1.4"></a>
 ## [0.1.4] - 2022-30-10
 
 This release improves the Rekordbox v6 database handling and fixes bugs in the 
 USN tracking.
 
 ### New Features
@@ -265,16 +280,15 @@
 - **fix Python version**  
 
 
 <a name="0.0.0"></a>
 ## 0.0.0 - 2022-10-04
 
 
-
-[Unreleased]: https://github.com/dylanljones/pyrekordbox/compare/0.1.4...HEAD
+[0.1.5]: https://github.com/dylanljones/pyrekordbox/compare/0.1.4...0.1.5
 [0.1.4]: https://github.com/dylanljones/pyrekordbox/compare/0.1.3...0.1.4
 [0.1.3]: https://github.com/dylanljones/pyrekordbox/compare/0.1.2...0.1.3
 [0.1.2]: https://github.com/dylanljones/pyrekordbox/compare/0.1.1...0.1.2
 [0.1.1]: https://github.com/dylanljones/pyrekordbox/compare/0.1.0...0.1.1
 [0.1.0]: https://github.com/dylanljones/pyrekordbox/compare/0.0.8...0.1.0
 [0.0.8]: https://github.com/dylanljones/pyrekordbox/compare/0.0.7...0.0.8
 [0.0.7]: https://github.com/dylanljones/pyrekordbox/compare/0.0.6...0.0.7
```

### Comparing `pyrekordbox-0.1.4/CONTRIBUTING.md` & `pyrekordbox-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/INSTALLATION.md` & `pyrekordbox-0.1.5/INSTALLATION.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/LICENSE` & `pyrekordbox-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/Libs/LICENSE_SQLCipher` & `pyrekordbox-0.1.5/Libs/LICENSE_SQLCipher`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/Libs/sqlcipher_py38/libcrypto-1_1.dll` & `pyrekordbox-0.1.5/Libs/sqlcipher_py38/libcrypto-1_1.dll`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/Libs/sqlcipher_py38/libssl-1_1.dll` & `pyrekordbox-0.1.5/Libs/sqlcipher_py38/libssl-1_1.dll`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/Libs/sqlcipher_py38/sqlcipher.dll` & `pyrekordbox-0.1.5/Libs/sqlcipher_py38/sqlcipher.dll`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/PKG-INFO` & `pyrekordbox-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrekordbox
-Version: 0.1.4
+Version: 0.1.5
 Summary: Inofficial Python package for interacting with the library of Pioneer's Rekordbox DJ software.
 Home-page: https://github.com/dylanljones/pyrekordbox
 Author: Dylan Jones
 Author-email: dylanljones94@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/dylanljones/pyrekordbox
 Project-URL: Documentation, https://pyrekordbox.readthedocs.io/en/stable/
@@ -294,39 +294,33 @@
 - [ ] Planned: Add RekordboxAgent client
 - [ ] Planned: Add USB export database support (`.pdb`).
 - [x] Improve Rekordbox 6 `master.db` database parsing.
 - [x] Add MySettings support.
 
 
 
-## 🔗 Related Projects
+## 🔗 Related Projects and References
 
 - [crate-digger]: Java library for fetching and parsing rekordbox exports and track analysis files.
 - [rekordcrate]: Library for parsing Pioneer Rekordbox device exports
 - [supbox]: Get the currently playing track from Rekordbox v6 as Audio Hijack Shoutcast/Icecast metadata, display in your OBS video broadcast or export as JSON.
-
-
-
-## 🙏 Thank Yous
-
-- [phil-bergmann](https://github.com/phil-bergmann) for helping with MacOS support!
 - Deep Symmetry has an extensive analysis of Rekordbox's ANLZ and .edb export file formats
   https://djl-analysis.deepsymmetry.org/djl-analysis
 - rekordcrate reverse engineered the format of the Rekordbox MySetting files
   https://holzhaus.github.io/rekordcrate/rekordcrate/setting/index.html
 - rekordcloud went into detail about the internals of Rekordbox 6
   https://rekord.cloud/blog/technical-inspection-of-rekordbox-6-and-its-new-internals.
 - supbox has a nice implementation on finding the Rekordbox 6 database key
   https://github.com/gabek/supbox
 
 
 
 
-[tests-badge]: https://img.shields.io/github/workflow/status/dylanljones/pyrekordbox/Test/master?label=tests&logo=github&style=flat
-[tests-dev-badge]: https://img.shields.io/github/workflow/status/dylanljones/pyrekordbox/Test/dev?label=tests&logo=github&style=flat
+[tests-badge]: https://img.shields.io/github/actions/workflow/status/dylanljones/pyrekordbox/tests.yml?branch=master&label=tests&logo=github&style=flat
+[tests-dev-badge]: https://img.shields.io/github/actions/workflow/status/dylanljones/pyrekordbox/tests.yml?branch=dev&label=tests&logo=github&style=flat
 [docs-badge]: https://img.shields.io/readthedocs/pyrekordbox/stable?style=flat
 [python-badge]: https://img.shields.io/pypi/pyversions/pyrekordbox?style=flat
 [python-badge+]: https://img.shields.io/badge/python-3.7+-blue.svg
 [platform-badge]: https://img.shields.io/badge/platform-win%20%7C%20osx-blue?style=flat
 [pypi-badge]: https://img.shields.io/pypi/v/pyrekordbox?style=flat
 [license-badge]: https://img.shields.io/pypi/l/pyrekordbox?color=lightgrey
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000?style=flat
```

### Comparing `pyrekordbox-0.1.4/README.md` & `pyrekordbox-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -262,39 +262,33 @@
 - [ ] Planned: Add RekordboxAgent client
 - [ ] Planned: Add USB export database support (`.pdb`).
 - [x] Improve Rekordbox 6 `master.db` database parsing.
 - [x] Add MySettings support.
 
 
 
-## 🔗 Related Projects
+## 🔗 Related Projects and References
 
 - [crate-digger]: Java library for fetching and parsing rekordbox exports and track analysis files.
 - [rekordcrate]: Library for parsing Pioneer Rekordbox device exports
 - [supbox]: Get the currently playing track from Rekordbox v6 as Audio Hijack Shoutcast/Icecast metadata, display in your OBS video broadcast or export as JSON.
-
-
-
-## 🙏 Thank Yous
-
-- [phil-bergmann](https://github.com/phil-bergmann) for helping with MacOS support!
 - Deep Symmetry has an extensive analysis of Rekordbox's ANLZ and .edb export file formats
   https://djl-analysis.deepsymmetry.org/djl-analysis
 - rekordcrate reverse engineered the format of the Rekordbox MySetting files
   https://holzhaus.github.io/rekordcrate/rekordcrate/setting/index.html
 - rekordcloud went into detail about the internals of Rekordbox 6
   https://rekord.cloud/blog/technical-inspection-of-rekordbox-6-and-its-new-internals.
 - supbox has a nice implementation on finding the Rekordbox 6 database key
   https://github.com/gabek/supbox
 
 
 
 
-[tests-badge]: https://img.shields.io/github/workflow/status/dylanljones/pyrekordbox/Test/master?label=tests&logo=github&style=flat
-[tests-dev-badge]: https://img.shields.io/github/workflow/status/dylanljones/pyrekordbox/Test/dev?label=tests&logo=github&style=flat
+[tests-badge]: https://img.shields.io/github/actions/workflow/status/dylanljones/pyrekordbox/tests.yml?branch=master&label=tests&logo=github&style=flat
+[tests-dev-badge]: https://img.shields.io/github/actions/workflow/status/dylanljones/pyrekordbox/tests.yml?branch=dev&label=tests&logo=github&style=flat
 [docs-badge]: https://img.shields.io/readthedocs/pyrekordbox/stable?style=flat
 [python-badge]: https://img.shields.io/pypi/pyversions/pyrekordbox?style=flat
 [python-badge+]: https://img.shields.io/badge/python-3.7+-blue.svg
 [platform-badge]: https://img.shields.io/badge/platform-win%20%7C%20osx-blue?style=flat
 [pypi-badge]: https://img.shields.io/pypi/v/pyrekordbox?style=flat
 [license-badge]: https://img.shields.io/pypi/l/pyrekordbox?color=lightgrey
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000?style=flat
```

### Comparing `pyrekordbox-0.1.4/docs/Makefile` & `pyrekordbox-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/make.bat` & `pyrekordbox-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_beat.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_beat.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_file.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_file.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pco2.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pco2.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pcob.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pcob.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pcp2.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pcp2.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pcpt.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pcpt.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_ppth.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_ppth.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pqt2.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pqt2.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pqt2_2.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pqt2_2.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pqtz.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pqtz.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pssi.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pssi.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pssi_entry.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pssi_entry.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pvbr.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pvbr.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwav.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwav.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv3.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv3.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv4.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv4.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv5.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv5.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv5_entry.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv5_entry.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv6.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv6.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwv7.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwv7.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_pwvc.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_pwvc.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/images/anlz_tag.svg` & `pyrekordbox-0.1.5/docs/source/_static/images/anlz_tag.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/logos/dark/logo_primary.svg` & `pyrekordbox-0.1.5/docs/source/_static/logos/dark/logo_primary.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/logos/light/logo_primary.svg` & `pyrekordbox-0.1.5/docs/source/_static/logos/light/logo_primary.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_static/logos/mid/logo_primary.svg` & `pyrekordbox-0.1.5/docs/source/_static/logos/mid/logo_primary.svg`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_templates/apidoc/package.rst_t` & `pyrekordbox-0.1.5/docs/source/_templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_templates/autosummary/class.rst` & `pyrekordbox-0.1.5/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/_templates/autosummary/module.rst` & `pyrekordbox-0.1.5/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/conf.py` & `pyrekordbox-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/formats/anlz.rst` & `pyrekordbox-0.1.5/docs/source/formats/anlz.rst`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/formats/db6.rst` & `pyrekordbox-0.1.5/docs/source/formats/db6.rst`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/formats/mysetting.rst` & `pyrekordbox-0.1.5/docs/source/formats/mysetting.rst`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/formats/xml.rst` & `pyrekordbox-0.1.5/docs/source/formats/xml.rst`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/index.rst` & `pyrekordbox-0.1.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/installation.md` & `pyrekordbox-0.1.5/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/quickstart.md` & `pyrekordbox-0.1.5/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/tutorial/configuration.md` & `pyrekordbox-0.1.5/docs/source/tutorial/configuration.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/tutorial/db6.md` & `pyrekordbox-0.1.5/docs/source/tutorial/db6.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/tutorial/mysetting.md` & `pyrekordbox-0.1.5/docs/source/tutorial/mysetting.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/docs/source/tutorial/xml.md` & `pyrekordbox-0.1.5/docs/source/tutorial/xml.md`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/install_pysqlcipher.py` & `pyrekordbox-0.1.5/install_pysqlcipher.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyproject.toml` & `pyrekordbox-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/__init__.py` & `pyrekordbox-0.1.5/pyrekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/anlz/__init__.py` & `pyrekordbox-0.1.5/pyrekordbox/anlz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/anlz/file.py` & `pyrekordbox-0.1.5/pyrekordbox/anlz/file.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/anlz/structs.py` & `pyrekordbox-0.1.5/pyrekordbox/anlz/structs.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/anlz/tags.py` & `pyrekordbox-0.1.5/pyrekordbox/anlz/tags.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/config.py` & `pyrekordbox-0.1.5/pyrekordbox/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,28 +24,16 @@
 
 # Define empty pyrekordbox configuration
 __config__ = {
     "pioneer": {
         "app_dir": "",
         "install_dir": "",
     },
-    "rekordbox5": {
-        "version": "",
-        "db_path": "",
-        "db_dir": "",
-        "app_dir": "",
-        "install_dir": "",
-    },
-    "rekordbox6": {
-        "version": "",
-        "db_path": "",
-        "db_dir": "",
-        "app_dir": "",
-        "install_dir": "",
-    },
+    "rekordbox5": {},
+    "rekordbox6": {},
 }
 
 
 def _get_rb_config(pioneer_prog_dir: str, pioneer_app_dir: str, version: int):
     # Get latest Rekordbox installation directory for major release `version`
     # -----------------------------------------------------------------------
 
@@ -124,25 +112,29 @@
     db_path = os.path.normpath(opts["db-path"])
     db_dir = os.path.dirname(db_path)
     assert conf["db_dir"] == db_dir
 
     if not os.path.exists(db_path):
         raise FileNotFoundError(f"The Rekordbox database '{db_path}' doesn't exist!")
 
+    conf["db_path"] = db_path
     # Read password from app.asar, see
     # https://www.reddit.com/r/Rekordbox/comments/qou6nm/key_to_open_masterdb_file/
     asar_data = read_rekordbox6_asar(conf["install_dir"])
-    match = re.search('pass: ".(.*?)"', asar_data).group(0)
-    pw = match.replace("pass: ", "").strip('"')
-
-    cipher = blowfish.Cipher(pw.encode())
-    dp = base64.standard_b64decode(opts["dp"])
-    dp = b"".join(cipher.decrypt_ecb(dp)).decode()
+    match_result = re.search('pass: ".(.*?)"', asar_data)
+    if match_result is None:
+        logging.warning("Incompatible rekordbox 6 database: Could not retrieve db-key.")
+    else:
+        match = match_result.group(0)
+        pw = match.replace("pass: ", "").strip('"')
+        cipher = blowfish.Cipher(pw.encode())
+        dp = base64.standard_b64decode(opts["dp"])
+        dp = b"".join(cipher.decrypt_ecb(dp)).decode()
+        conf["dp"] = dp
 
-    conf.update({"db_path": db_path, "dp": dp})
     return conf
 
 
 def update_config(pioneer_install_dir="", pioneer_app_dir=""):
     """Update the pyrekordbox configuration.
 
     This method scans the system for the Rekordbox installation and application data
@@ -186,22 +178,22 @@
         return
 
     # Update Rekordbox 5 config
     try:
         conf = _get_rb5_config(pioneer_install_dir, pioneer_app_dir)
         __config__["rekordbox5"].update(conf)
     except FileNotFoundError as e:
-        logging.warning(e)
+        logger.info(e)
 
     # Update Rekordbox 6 config
     try:
         conf = _get_rb6_config(pioneer_install_dir, pioneer_app_dir)
         __config__["rekordbox6"].update(conf)
     except FileNotFoundError as e:
-        logging.warning(e)
+        logger.info(e)
 
 
 # Fill the pyrekordbox-configuration
 update_config()
 
 
 def get_config(section, key=None):
@@ -231,17 +223,19 @@
     pioneer = __config__["pioneer"]
     rb5 = __config__["rekordbox5"]
     rb6 = __config__["rekordbox6"]
 
     lines = ["Pioneer:"]
     lines += [f"{indent}{k + delim:<{hw}} {pioneer[k]}" for k in sorted(pioneer.keys())]
     lines.append("Rekordbox 5:")
-    lines += [f"{indent}{k + delim:<{hw}} {rb5[k]}" for k in sorted(rb5.keys())]
+    if rb5:
+        lines += [f"{indent}{k + delim:<{hw}} {rb5[k]}" for k in sorted(rb5.keys())]
     lines.append("Rekordbox 6:")
-    rb6_keys = [k for k in rb6.keys() if k not in ("dp", "p")]
-    lines += [f"{indent}{k + delim:<{hw}} {rb6[k]}" for k in sorted(rb6_keys)]
+    if rb6:
+        rb6_keys = [k for k in rb6.keys() if k not in ("dp", "p")]
+        lines += [f"{indent}{k + delim:<{hw}} {rb6[k]}" for k in sorted(rb6_keys)]
     return "\n".join(lines)
 
 
 def show_config():
     """Prints a formatted string of the pyrekordbox configurations."""
     print(pformat_config())
```

### Comparing `pyrekordbox-0.1.4/pyrekordbox/db6/__init__.py` & `pyrekordbox-0.1.5/pyrekordbox/db6/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/db6/database.py` & `pyrekordbox-0.1.5/pyrekordbox/db6/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,18 @@
         # Use default sqlite3 package
         # This requires that the 'sqlite3.dll' was replaced by the 'sqlcipher.dll'
         sql_driver = sqlite3
     con = sql_driver.connect(path)
 
     if unlock:
         # Read and decode master.db key
-        key = rb6_config["dp"]
+        try:
+            key = rb6_config["dp"]
+        except KeyError:
+            raise ValueError("Incompatible rekordbox 6 database: No key found")
         logger.info("Key: %s", key)
         # Unlock database
         con.execute(f"PRAGMA key='{key}'")
 
     # Check connection
     try:
         con.execute("SELECT name FROM sqlite_master WHERE type='table';")
@@ -149,35 +152,44 @@
 
     Use the included getters for querying the database:
 
     >>> db.get_content()[0]
     <DjmdContent(40110712   Title=NOISE)>
     """
 
-    def __init__(self, path="", unlock=True):
+    def __init__(self, path="", key="", unlock=True):
         if not path:
-            path = rb6_config["db_path"]
+            # Get path from the RB config
+            path = rb6_config.get("db_path", "")
+            if not path:
+                pdir = get_config("pioneer", "install_dir")
+                raise FileNotFoundError(f"No Rekordbox v6 directory found in '{pdir}'")
+        # make sure file exists
         if not os.path.exists(path):
             raise FileNotFoundError(f"File '{path}' does not exist!")
         # Open database
         if unlock:
-            key = rb6_config["dp"]
+            if not key:
+                try:
+                    key = rb6_config["dp"]
+                except KeyError:
+                    raise ValueError("Incompatible rekordbox 6 database: No key found")
             url = f"sqlite+pysqlcipher://:{key}@/{path}?"
             engine = create_engine(url, module=sqlite3)
         else:
             engine = create_engine(f"sqlite:///{path}")
 
         self.engine = engine
         self._Session = sessionmaker(bind=self.engine)
         self.session: Optional[Session] = None
 
         self.registry = RekordboxAgentRegistry(self)
         self._events = dict()
 
-        self._db_dir = os.path.normpath(rb6_config["db_dir"])
+        self._db_dir = os.path.normpath(path)
         self._anlz_root = os.path.join(self._db_dir, "share")
 
         self.open()
 
     @property
     def no_autoflush(self):
         """Creates a no-autoflush context."""
```

### Comparing `pyrekordbox-0.1.4/pyrekordbox/db6/registry.py` & `pyrekordbox-0.1.5/pyrekordbox/db6/registry.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/db6/tables.py` & `pyrekordbox-0.1.5/pyrekordbox/db6/tables.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/logger.py` & `pyrekordbox-0.1.5/pyrekordbox/logger.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/mysettings/__init__.py` & `pyrekordbox-0.1.5/pyrekordbox/mysettings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/mysettings/file.py` & `pyrekordbox-0.1.5/pyrekordbox/mysettings/file.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/mysettings/structs.py` & `pyrekordbox-0.1.5/pyrekordbox/mysettings/structs.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/utils.py` & `pyrekordbox-0.1.5/pyrekordbox/utils.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/pyrekordbox/xml.py` & `pyrekordbox-0.1.5/pyrekordbox/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
             raise XmlAttributeKeyError(self.__class__, key, self.ATTRIBS)
         try:
             # Apply callback
             value = self.SETTERS[key](value)
         except KeyError:
             # Convert to str just in case
             value = str(value)
-        self._element.attrib.set(key, value)
+        self._element.attrib[key] = value
 
     def __len__(self):
         """int: The number of attributes of the XML element."""
         return len(self._element.attrib)
 
     def __iter__(self):
         """Iterable: An iterator of the attribute keys of the XML element."""
```

### Comparing `pyrekordbox-0.1.4/pyrekordbox.egg-info/PKG-INFO` & `pyrekordbox-0.1.5/pyrekordbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrekordbox
-Version: 0.1.4
+Version: 0.1.5
 Summary: Inofficial Python package for interacting with the library of Pioneer's Rekordbox DJ software.
 Home-page: https://github.com/dylanljones/pyrekordbox
 Author: Dylan Jones
 Author-email: dylanljones94@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/dylanljones/pyrekordbox
 Project-URL: Documentation, https://pyrekordbox.readthedocs.io/en/stable/
@@ -294,39 +294,33 @@
 - [ ] Planned: Add RekordboxAgent client
 - [ ] Planned: Add USB export database support (`.pdb`).
 - [x] Improve Rekordbox 6 `master.db` database parsing.
 - [x] Add MySettings support.
 
 
 
-## 🔗 Related Projects
+## 🔗 Related Projects and References
 
 - [crate-digger]: Java library for fetching and parsing rekordbox exports and track analysis files.
 - [rekordcrate]: Library for parsing Pioneer Rekordbox device exports
 - [supbox]: Get the currently playing track from Rekordbox v6 as Audio Hijack Shoutcast/Icecast metadata, display in your OBS video broadcast or export as JSON.
-
-
-
-## 🙏 Thank Yous
-
-- [phil-bergmann](https://github.com/phil-bergmann) for helping with MacOS support!
 - Deep Symmetry has an extensive analysis of Rekordbox's ANLZ and .edb export file formats
   https://djl-analysis.deepsymmetry.org/djl-analysis
 - rekordcrate reverse engineered the format of the Rekordbox MySetting files
   https://holzhaus.github.io/rekordcrate/rekordcrate/setting/index.html
 - rekordcloud went into detail about the internals of Rekordbox 6
   https://rekord.cloud/blog/technical-inspection-of-rekordbox-6-and-its-new-internals.
 - supbox has a nice implementation on finding the Rekordbox 6 database key
   https://github.com/gabek/supbox
 
 
 
 
-[tests-badge]: https://img.shields.io/github/workflow/status/dylanljones/pyrekordbox/Test/master?label=tests&logo=github&style=flat
-[tests-dev-badge]: https://img.shields.io/github/workflow/status/dylanljones/pyrekordbox/Test/dev?label=tests&logo=github&style=flat
+[tests-badge]: https://img.shields.io/github/actions/workflow/status/dylanljones/pyrekordbox/tests.yml?branch=master&label=tests&logo=github&style=flat
+[tests-dev-badge]: https://img.shields.io/github/actions/workflow/status/dylanljones/pyrekordbox/tests.yml?branch=dev&label=tests&logo=github&style=flat
 [docs-badge]: https://img.shields.io/readthedocs/pyrekordbox/stable?style=flat
 [python-badge]: https://img.shields.io/pypi/pyversions/pyrekordbox?style=flat
 [python-badge+]: https://img.shields.io/badge/python-3.7+-blue.svg
 [platform-badge]: https://img.shields.io/badge/platform-win%20%7C%20osx-blue?style=flat
 [pypi-badge]: https://img.shields.io/pypi/v/pyrekordbox?style=flat
 [license-badge]: https://img.shields.io/pypi/l/pyrekordbox?color=lightgrey
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000?style=flat
```

### Comparing `pyrekordbox-0.1.4/pyrekordbox.egg-info/SOURCES.txt` & `pyrekordbox-0.1.5/pyrekordbox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yaml
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/codeql.yml
 .github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
 .testdata/export/PIONEER/DEVSETTING.DAT
 .testdata/export/PIONEER/DJMMYSETTING.DAT
 .testdata/export/PIONEER/MYSETTING.DAT
 .testdata/export/PIONEER/MYSETTING2.DAT
 .testdata/export/PIONEER/USBANLZ/P016/0000875E/ANLZ0000.2EX
```

### Comparing `pyrekordbox-0.1.4/setup.cfg` & `pyrekordbox-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	construct>=2.10.0
 	hypothesis>=6.0.0
 	numpy>=1.19.0
 	pytest>=6.2.0
 	psutil>=5.9.0
 	setuptools>=60.0.0
 	setuptools-scm[toml]>=4
-	sqlalchemy>=1.4.0
+	sqlalchemy~=1.4.0
 python_requires = >=3.7
 include_package_data = True
 platforms = any
 zip_safe = False
 
 [options.extras_require]
 build =
```

### Comparing `pyrekordbox-0.1.4/tests/test_anlz.py` & `pyrekordbox-0.1.5/tests/test_anlz.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/tests/test_db6.py` & `pyrekordbox-0.1.5/tests/test_db6.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/tests/test_mysetting.py` & `pyrekordbox-0.1.5/tests/test_mysetting.py`

 * *Files identical despite different names*

### Comparing `pyrekordbox-0.1.4/tests/test_xml.py` & `pyrekordbox-0.1.5/tests/test_xml.py`

 * *Files identical despite different names*

