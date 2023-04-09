# Comparing `tmp/pynecone-0.1.21a0.tar.gz` & `tmp/pynecone-0.1.22a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.21a0.tar", max compression
+gzip compressed data, was "pynecone-0.1.22a0.tar", max compression
```

## Comparing `pynecone-0.1.21a0.tar` & `pynecone-0.1.22a0.tar`

### file list

```diff
@@ -1,141 +1,149 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.21a0/LICENSE
--rw-r--r--   0        0        0     8364 2023-03-16 23:51:05.127293 pynecone-0.1.21a0/README.md
--rw-r--r--   0        0        0        0 2022-11-18 20:43:33.738202 pynecone-0.1.21a0/pynecone/.templates/app/__init__.py
--rw-r--r--   0        0        0     1036 2023-03-10 00:25:42.687001 pynecone-0.1.21a0/pynecone/.templates/app/tutorial.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.21a0/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.21a0/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   261125 2023-03-10 00:25:42.688288 pynecone-0.1.21a0/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.21a0/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0     1017 2023-04-02 23:51:14.630623 pynecone-0.1.21a0/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.21a0/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.21a0/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       28 2023-04-03 00:00:47.639618 pynecone-0.1.21a0/pynecone/.templates/web/pynecone.json
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.21a0/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     6456 2023-04-02 23:51:28.426792 pynecone-0.1.21a0/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0      786 2023-03-10 00:25:42.690134 pynecone-0.1.21a0/pynecone/__init__.py
--rw-r--r--   0        0        0    19161 2023-04-02 23:51:28.426995 pynecone-0.1.21a0/pynecone/app.py
--rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.21a0/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.21a0/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     5737 2023-03-16 23:52:12.744038 pynecone-0.1.21a0/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     5334 2023-04-02 23:51:14.631307 pynecone-0.1.21a0/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     9084 2023-03-16 23:52:12.744496 pynecone-0.1.21a0/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     6371 2023-04-02 23:51:14.631475 pynecone-0.1.21a0/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.21a0/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      726 2022-11-18 20:43:33.735684 pynecone-0.1.21a0/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.21a0/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.21a0/pynecone/components/base/document.py
--rw-r--r--   0        0        0      242 2022-11-18 20:43:33.735533 pynecone-0.1.21a0/pynecone/components/base/head.py
--rw-r--r--   0        0        0      929 2023-03-13 04:10:28.761099 pynecone-0.1.21a0/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1399 2023-03-10 00:25:42.693576 pynecone-0.1.21a0/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    19351 2023-04-02 23:51:14.631702 pynecone-0.1.21a0/pynecone/components/component.py
--rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.21a0/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      333 2022-11-18 20:43:33.720898 pynecone-0.1.21a0/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2486 2023-03-16 23:52:12.744773 pynecone-0.1.21a0/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4067 2023-04-02 23:51:28.427690 pynecone-0.1.21a0/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      536 2022-11-18 20:43:33.720383 pynecone-0.1.21a0/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.21a0/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1429 2023-03-13 04:10:28.547828 pynecone-0.1.21a0/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2156 2023-03-09 23:41:57.135449 pynecone-0.1.21a0/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5156 2023-03-10 00:25:42.695438 pynecone-0.1.21a0/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.21a0/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2940 2023-03-09 23:41:57.135814 pynecone-0.1.21a0/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2776 2023-03-09 23:41:57.135961 pynecone-0.1.21a0/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.21a0/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.21a0/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1570 2023-03-10 00:25:42.695849 pynecone-0.1.21a0/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1904 2023-03-10 00:25:42.696112 pynecone-0.1.21a0/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      878 2023-03-10 00:25:42.696451 pynecone-0.1.21a0/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1784 2022-11-18 20:43:33.722941 pynecone-0.1.21a0/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      677 2022-11-18 20:43:33.724636 pynecone-0.1.21a0/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1103 2023-03-10 00:25:42.696881 pynecone-0.1.21a0/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1534 2022-11-18 20:43:33.708227 pynecone-0.1.21a0/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2240 2023-03-10 00:25:42.697372 pynecone-0.1.21a0/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      593 2023-01-30 21:50:18.211339 pynecone-0.1.21a0/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0     1964 2023-03-10 00:25:42.697696 pynecone-0.1.21a0/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0     2323 2023-03-09 23:41:57.137070 pynecone-0.1.21a0/pynecone/components/forms/formcontrol.py
--rw-r--r--   0        0        0      801 2022-12-07 23:08:48.791901 pynecone-0.1.21a0/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2660 2023-03-10 00:25:42.698121 pynecone-0.1.21a0/pynecone/components/forms/input.py
--rw-r--r--   0        0        0     3916 2023-03-10 00:25:42.698330 pynecone-0.1.21a0/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      252 2023-03-10 00:25:42.698673 pynecone-0.1.21a0/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2685 2023-03-10 00:25:42.698849 pynecone-0.1.21a0/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3004 2023-03-16 23:52:12.745021 pynecone-0.1.21a0/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2868 2023-03-10 00:25:42.699342 pynecone-0.1.21a0/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3475 2023-03-16 23:52:12.745104 pynecone-0.1.21a0/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     2782 2023-03-10 00:25:42.699714 pynecone-0.1.21a0/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1466 2023-03-10 00:25:42.699988 pynecone-0.1.21a0/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1550 2023-03-10 00:25:42.700204 pynecone-0.1.21a0/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2691 2023-04-02 23:51:14.632480 pynecone-0.1.21a0/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.21a0/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1256 2023-03-09 23:41:57.137618 pynecone-0.1.21a0/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17359 2023-04-02 23:51:28.428293 pynecone-0.1.21a0/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.21a0/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      323 2023-04-02 23:51:14.632894 pynecone-0.1.21a0/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      768 2022-12-15 19:19:57.795670 pynecone-0.1.21a0/pynecone/components/layout/box.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.21a0/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3136 2023-03-16 23:52:12.745203 pynecone-0.1.21a0/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      362 2022-12-07 23:08:48.792884 pynecone-0.1.21a0/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      655 2022-12-07 23:08:48.793078 pynecone-0.1.21a0/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     1781 2023-03-10 00:25:42.701858 pynecone-0.1.21a0/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.21a0/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2417 2023-01-28 19:09:51.493446 pynecone-0.1.21a0/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0     1015 2023-03-09 22:58:06.084286 pynecone-0.1.21a0/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.21a0/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.21a0/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      994 2022-12-07 23:08:48.793762 pynecone-0.1.21a0/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1470 2023-03-09 23:41:57.138212 pynecone-0.1.21a0/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.21a0/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.21a0/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.21a0/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0     1539 2022-11-28 06:46:25.092156 pynecone-0.1.21a0/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.21a0/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1415 2022-12-07 23:08:48.794371 pynecone-0.1.21a0/pynecone/components/media/image.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.21a0/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2022 2023-03-09 23:41:57.138732 pynecone-0.1.21a0/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1005 2023-01-24 01:31:44.831545 pynecone-0.1.21a0/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      529 2022-12-07 23:08:48.794948 pynecone-0.1.21a0/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      483 2022-12-07 23:08:48.795126 pynecone-0.1.21a0/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.21a0/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5042 2023-03-10 00:25:42.703076 pynecone-0.1.21a0/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     4696 2023-03-10 00:25:42.703402 pynecone-0.1.21a0/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5545 2023-03-10 00:25:42.703834 pynecone-0.1.21a0/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4932 2023-03-10 00:25:42.704095 pynecone-0.1.21a0/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5703 2023-03-09 23:41:57.139627 pynecone-0.1.21a0/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1964 2023-01-28 19:09:51.496014 pynecone-0.1.21a0/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.21a0/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      840 2023-03-16 23:52:12.745828 pynecone-0.1.21a0/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3000 2023-03-16 23:52:12.746048 pynecone-0.1.21a0/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     6288 2023-04-02 23:51:14.633181 pynecone-0.1.21a0/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.21a0/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.21a0/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      281 2022-12-07 23:08:48.796090 pynecone-0.1.21a0/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      357 2023-03-09 23:41:57.139928 pynecone-0.1.21a0/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     2974 2023-03-16 23:52:12.746696 pynecone-0.1.21a0/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      336 2022-12-08 04:28:39.380713 pynecone-0.1.21a0/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      305 2022-12-07 23:08:48.796735 pynecone-0.1.21a0/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     1969 2023-03-16 23:52:12.746899 pynecone-0.1.21a0/pynecone/config.py
--rw-r--r--   0        0        0     8788 2023-03-16 23:52:12.747156 pynecone-0.1.21a0/pynecone/constants.py
--rw-r--r--   0        0        0     9489 2023-04-02 23:51:14.633295 pynecone-0.1.21a0/pynecone/event.py
--rw-r--r--   0        0        0      163 2022-12-27 07:24:05.349499 pynecone-0.1.21a0/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1955 2023-03-16 23:52:12.747621 pynecone-0.1.21a0/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1010 2022-12-27 07:24:05.349743 pynecone-0.1.21a0/pynecone/middleware/logging_middleware.py
--rw-r--r--   0        0        0     1109 2023-01-28 19:09:51.497705 pynecone-0.1.21a0/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     1583 2023-04-02 23:51:28.428464 pynecone-0.1.21a0/pynecone/model.py
--rw-r--r--   0        0        0     7582 2023-04-02 23:51:14.633461 pynecone-0.1.21a0/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.21a0/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.21a0/pynecone/route.py
--rw-r--r--   0        0        0    22841 2023-03-17 21:55:20.767085 pynecone-0.1.21a0/pynecone/state.py
--rw-r--r--   0        0        0     1059 2023-03-16 23:52:12.748857 pynecone-0.1.21a0/pynecone/style.py
--rw-r--r--   0        0        0     2411 2023-03-10 00:25:42.708535 pynecone-0.1.21a0/pynecone/telemetry.py
--rw-r--r--   0        0        0     4054 2023-03-16 23:52:12.749028 pynecone-0.1.21a0/pynecone/utils/build.py
--rw-r--r--   0        0        0     1627 2023-03-16 23:52:12.749156 pynecone-0.1.21a0/pynecone/utils/console.py
--rw-r--r--   0        0        0     3795 2023-03-16 23:52:12.756812 pynecone-0.1.21a0/pynecone/utils/exec.py
--rw-r--r--   0        0        0     9766 2023-04-02 23:51:28.428628 pynecone-0.1.21a0/pynecone/utils/format.py
--rw-r--r--   0        0        0      544 2023-03-16 23:52:12.757094 pynecone-0.1.21a0/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.21a0/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0     7724 2023-03-16 23:52:12.757262 pynecone-0.1.21a0/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.21a0/pynecone/utils/processes.py
--rw-r--r--   0        0        0     4299 2023-03-16 23:52:12.757408 pynecone-0.1.21a0/pynecone/utils/types.py
--rw-r--r--   0        0        0    25132 2023-04-02 23:51:28.428813 pynecone-0.1.21a0/pynecone/var.py
--rw-r--r--   0        0        0     2634 2023-03-13 04:10:28.761553 pynecone-0.1.21a0/pynecone/watch.py
--rw-r--r--   0        0        0     1757 2023-04-03 00:02:40.555662 pynecone-0.1.21a0/pyproject.toml
--rw-r--r--   0        0        0     9856 1970-01-01 00:00:00.000000 pynecone-0.1.21a0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.22a0/LICENSE
+-rw-r--r--   0        0        0     8364 2023-03-16 23:51:05.127293 pynecone-0.1.22a0/README.md
+-rw-r--r--   0        0        0        0 2022-11-18 20:43:33.738202 pynecone-0.1.22a0/pynecone/.templates/app/__init__.py
+-rw-r--r--   0        0        0     1036 2023-03-10 00:25:42.687001 pynecone-0.1.22a0/pynecone/.templates/app/tutorial.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.22a0/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.22a0/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   261125 2023-03-10 00:25:42.688288 pynecone-0.1.22a0/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.22a0/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1017 2023-04-02 23:51:14.630623 pynecone-0.1.22a0/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.22a0/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.22a0/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       28 2023-04-03 00:00:47.639618 pynecone-0.1.22a0/pynecone/.templates/web/pynecone.json
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.22a0/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     6456 2023-04-02 23:51:28.426792 pynecone-0.1.22a0/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0      808 2023-04-08 16:05:43.351479 pynecone-0.1.22a0/pynecone/__init__.py
+-rw-r--r--   0        0        0    19946 2023-04-09 05:48:16.467591 pynecone-0.1.22a0/pynecone/app.py
+-rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.22a0/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.22a0/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     5737 2023-04-03 21:50:34.663262 pynecone-0.1.22a0/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     5334 2023-04-02 23:51:14.631307 pynecone-0.1.22a0/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     9084 2023-03-16 23:52:12.744496 pynecone-0.1.22a0/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     6371 2023-04-02 23:51:14.631475 pynecone-0.1.22a0/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.22a0/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      726 2022-11-18 20:43:33.735684 pynecone-0.1.22a0/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.22a0/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.22a0/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      242 2022-11-18 20:43:33.735533 pynecone-0.1.22a0/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-03-13 04:10:28.761099 pynecone-0.1.22a0/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1399 2023-03-10 00:25:42.693576 pynecone-0.1.22a0/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    19436 2023-04-04 01:35:33.200080 pynecone-0.1.22a0/pynecone/components/component.py
+-rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.22a0/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      333 2022-11-18 20:43:33.720898 pynecone-0.1.22a0/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2486 2023-03-16 23:52:12.744773 pynecone-0.1.22a0/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4067 2023-04-02 23:51:28.427690 pynecone-0.1.22a0/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      536 2022-11-18 20:43:33.720383 pynecone-0.1.22a0/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.22a0/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1429 2023-03-13 04:10:28.547828 pynecone-0.1.22a0/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2156 2023-03-09 23:41:57.135449 pynecone-0.1.22a0/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5156 2023-03-10 00:25:42.695438 pynecone-0.1.22a0/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.22a0/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2940 2023-03-09 23:41:57.135814 pynecone-0.1.22a0/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2776 2023-03-09 23:41:57.135961 pynecone-0.1.22a0/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.22a0/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.22a0/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1570 2023-03-10 00:25:42.695849 pynecone-0.1.22a0/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1904 2023-03-10 00:25:42.696112 pynecone-0.1.22a0/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      878 2023-03-10 00:25:42.696451 pynecone-0.1.22a0/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1784 2022-11-18 20:43:33.722941 pynecone-0.1.22a0/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      677 2022-11-18 20:43:33.724636 pynecone-0.1.22a0/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1103 2023-03-10 00:25:42.696881 pynecone-0.1.22a0/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1534 2022-11-18 20:43:33.708227 pynecone-0.1.22a0/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2240 2023-03-10 00:25:42.697372 pynecone-0.1.22a0/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      593 2023-01-30 21:50:18.211339 pynecone-0.1.22a0/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0     1964 2023-03-10 00:25:42.697696 pynecone-0.1.22a0/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0     2323 2023-03-09 23:41:57.137070 pynecone-0.1.22a0/pynecone/components/forms/formcontrol.py
+-rw-r--r--   0        0        0      801 2022-12-07 23:08:48.791901 pynecone-0.1.22a0/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2660 2023-03-10 00:25:42.698121 pynecone-0.1.22a0/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0     3916 2023-03-10 00:25:42.698330 pynecone-0.1.22a0/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      252 2023-03-10 00:25:42.698673 pynecone-0.1.22a0/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2685 2023-03-10 00:25:42.698849 pynecone-0.1.22a0/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3004 2023-03-16 23:52:12.745021 pynecone-0.1.22a0/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2868 2023-03-10 00:25:42.699342 pynecone-0.1.22a0/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3475 2023-03-16 23:52:12.745104 pynecone-0.1.22a0/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     2782 2023-03-10 00:25:42.699714 pynecone-0.1.22a0/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1466 2023-03-10 00:25:42.699988 pynecone-0.1.22a0/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1550 2023-03-10 00:25:42.700204 pynecone-0.1.22a0/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2691 2023-04-02 23:51:14.632480 pynecone-0.1.22a0/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.22a0/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-04 00:07:26.680060 pynecone-0.1.22a0/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17359 2023-04-02 23:51:28.428293 pynecone-0.1.22a0/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.22a0/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      323 2023-04-02 23:51:14.632894 pynecone-0.1.22a0/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      768 2022-12-15 19:19:57.795670 pynecone-0.1.22a0/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.22a0/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3136 2023-03-16 23:52:12.745203 pynecone-0.1.22a0/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      362 2022-12-07 23:08:48.792884 pynecone-0.1.22a0/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      655 2022-12-07 23:08:48.793078 pynecone-0.1.22a0/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     1781 2023-03-10 00:25:42.701858 pynecone-0.1.22a0/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.22a0/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2417 2023-01-28 19:09:51.493446 pynecone-0.1.22a0/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-04-08 16:05:43.352661 pynecone-0.1.22a0/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.22a0/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.22a0/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      994 2022-12-07 23:08:48.793762 pynecone-0.1.22a0/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1470 2023-03-09 23:41:57.138212 pynecone-0.1.22a0/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.22a0/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.22a0/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.22a0/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0     1539 2022-11-28 06:46:25.092156 pynecone-0.1.22a0/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.22a0/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1415 2022-12-07 23:08:48.794371 pynecone-0.1.22a0/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.22a0/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2022 2023-03-09 23:41:57.138732 pynecone-0.1.22a0/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1005 2023-01-24 01:31:44.831545 pynecone-0.1.22a0/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      529 2022-12-07 23:08:48.794948 pynecone-0.1.22a0/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      483 2022-12-07 23:08:48.795126 pynecone-0.1.22a0/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.22a0/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5042 2023-03-10 00:25:42.703076 pynecone-0.1.22a0/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     4696 2023-03-10 00:25:42.703402 pynecone-0.1.22a0/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5545 2023-03-10 00:25:42.703834 pynecone-0.1.22a0/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4932 2023-03-10 00:25:42.704095 pynecone-0.1.22a0/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5703 2023-03-09 23:41:57.139627 pynecone-0.1.22a0/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1964 2023-01-28 19:09:51.496014 pynecone-0.1.22a0/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.22a0/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      840 2023-03-16 23:52:12.745828 pynecone-0.1.22a0/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3000 2023-03-16 23:52:12.746048 pynecone-0.1.22a0/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     6288 2023-04-02 23:51:14.633181 pynecone-0.1.22a0/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.22a0/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.22a0/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      281 2022-12-07 23:08:48.796090 pynecone-0.1.22a0/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      357 2023-03-09 23:41:57.139928 pynecone-0.1.22a0/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     2973 2023-04-08 16:05:43.353266 pynecone-0.1.22a0/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      336 2022-12-08 04:28:39.380713 pynecone-0.1.22a0/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      305 2022-12-07 23:08:48.796735 pynecone-0.1.22a0/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     5296 2023-04-08 16:05:43.353608 pynecone-0.1.22a0/pynecone/config.py
+-rw-r--r--   0        0        0     8905 2023-04-04 00:07:26.681289 pynecone-0.1.22a0/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-03 21:29:22.111846 pynecone-0.1.22a0/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-03 21:29:22.112002 pynecone-0.1.22a0/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-03 21:29:22.112233 pynecone-0.1.22a0/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-04 00:00:54.955098 pynecone-0.1.22a0/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-03 21:29:22.112537 pynecone-0.1.22a0/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1289 2023-04-04 00:00:54.955401 pynecone-0.1.22a0/pynecone/el/element.py
+-rw-r--r--   0        0        0   108515 2023-04-03 21:29:22.113056 pynecone-0.1.22a0/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2666 2023-04-04 00:00:54.955649 pynecone-0.1.22a0/pynecone/el/precompile.py
+-rw-r--r--   0        0        0     9581 2023-04-08 19:55:02.842558 pynecone-0.1.22a0/pynecone/event.py
+-rw-r--r--   0        0        0      163 2022-12-27 07:24:05.349499 pynecone-0.1.22a0/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     2781 2023-04-08 17:02:14.865880 pynecone-0.1.22a0/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1022 2023-04-08 16:05:43.354548 pynecone-0.1.22a0/pynecone/middleware/logging_middleware.py
+-rw-r--r--   0        0        0     1193 2023-04-08 16:05:43.355024 pynecone-0.1.22a0/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     1583 2023-04-02 23:51:28.428464 pynecone-0.1.22a0/pynecone/model.py
+-rw-r--r--   0        0        0     7580 2023-04-08 16:05:43.355348 pynecone-0.1.22a0/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.22a0/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.22a0/pynecone/route.py
+-rw-r--r--   0        0        0    23620 2023-04-08 16:55:17.975051 pynecone-0.1.22a0/pynecone/state.py
+-rw-r--r--   0        0        0     1059 2023-03-16 23:52:12.748857 pynecone-0.1.22a0/pynecone/style.py
+-rw-r--r--   0        0        0     2411 2023-03-10 00:25:42.708535 pynecone-0.1.22a0/pynecone/telemetry.py
+-rw-r--r--   0        0        0     4054 2023-03-16 23:52:12.749028 pynecone-0.1.22a0/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1627 2023-03-16 23:52:12.749156 pynecone-0.1.22a0/pynecone/utils/console.py
+-rw-r--r--   0        0        0     3795 2023-03-16 23:52:12.756812 pynecone-0.1.22a0/pynecone/utils/exec.py
+-rw-r--r--   0        0        0     9766 2023-04-02 23:51:28.428628 pynecone-0.1.22a0/pynecone/utils/format.py
+-rw-r--r--   0        0        0      544 2023-03-16 23:52:12.757094 pynecone-0.1.22a0/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.22a0/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0     8615 2023-04-04 00:07:26.681689 pynecone-0.1.22a0/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.22a0/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     4299 2023-03-16 23:52:12.757408 pynecone-0.1.22a0/pynecone/utils/types.py
+-rw-r--r--   0        0        0    25132 2023-04-02 23:51:28.428813 pynecone-0.1.22a0/pynecone/var.py
+-rw-r--r--   0        0        0     2634 2023-03-13 04:10:28.761553 pynecone-0.1.22a0/pynecone/watch.py
+-rw-r--r--   0        0        0     1757 2023-04-09 05:55:04.077494 pynecone-0.1.22a0/pyproject.toml
+-rw-r--r--   0        0        0     9856 1970-01-01 00:00:00.000000 pynecone-0.1.22a0/PKG-INFO
```

### Comparing `pynecone-0.1.21a0/LICENSE` & `pynecone-0.1.22a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/README.md` & `pynecone-0.1.22a0/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/.templates/app/tutorial.py` & `pynecone-0.1.22a0/pynecone/.templates/app/tutorial.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.22a0/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.22a0/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/.templates/web/package.json` & `pynecone-0.1.22a0/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.22a0/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.22a0/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.22a0/pynecone/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/__init__.py` & `pynecone-0.1.22a0/pynecone/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Import all classes and functions the end user will need to make an app.
 
 Anything imported here will be available in the default Pynecone import as `pc.*`.
 """
 
+from . import el
 from .app import App, UploadFile
 from .base import Base
 from .components import *
-from .components.component import custom_component as component
+from .components.component import custom_component as memo
 from .components.graphing.victory import data
-from .config import Config
+from .config import Config, DBConfig
 from .constants import Env, Transports
 from .event import (
     EVENT_ARG,
     EventChain,
     console_log,
     redirect,
     window_alert,
```

### Comparing `pynecone-0.1.21a0/pynecone/app.py` & `pynecone-0.1.22a0/pynecone/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """The main Pynecone app."""
 
+import asyncio
 import inspect
 from typing import Any, Callable, Coroutine, Dict, List, Optional, Tuple, Type, Union
 
 from fastapi import FastAPI, UploadFile
 from fastapi.middleware import cors
 from socketio import ASGIApp, AsyncNamespace, AsyncServer
 
@@ -144,15 +145,17 @@
             cors.CORSMiddleware,
             allow_credentials=True,
             allow_methods=["*"],
             allow_headers=["*"],
             allow_origins=["*"],
         )
 
-    def preprocess(self, state: State, event: Event) -> Optional[Delta]:
+    async def preprocess(
+        self, state: State, event: Event
+    ) -> Optional[Union[StateUpdate, List[StateUpdate]]]:
         """Preprocess the event.
 
         This is where middleware can modify the event before it is processed.
         Each middleware is called in the order it was added to the app.
 
         If a middleware returns a delta, the event is not processed and the
         delta is returned.
@@ -161,19 +164,24 @@
             state: The state to preprocess.
             event: The event to preprocess.
 
         Returns:
             An optional state to return.
         """
         for middleware in self.middleware:
-            out = middleware.preprocess(app=self, state=state, event=event)
+            if asyncio.iscoroutinefunction(middleware.preprocess):
+                out = await middleware.preprocess(app=self, state=state, event=event)
+            else:
+                out = middleware.preprocess(app=self, state=state, event=event)
             if out is not None:
-                return out
+                return out  # type: ignore
 
-    def postprocess(self, state: State, event: Event, delta: Delta) -> Optional[Delta]:
+    async def postprocess(
+        self, state: State, event: Event, delta: Delta
+    ) -> Optional[Delta]:
         """Postprocess the event.
 
         This is where middleware can modify the delta after it is processed.
         Each middleware is called in the order it was added to the app.
 
         If a middleware returns a delta, the delta is not processed and the
         delta is returned.
@@ -183,19 +191,24 @@
             event: The event to postprocess.
             delta: The delta to postprocess.
 
         Returns:
             An optional state to return.
         """
         for middleware in self.middleware:
-            out = middleware.postprocess(
-                app=self, state=state, event=event, delta=delta
-            )
+            if asyncio.iscoroutinefunction(middleware.postprocess):
+                out = await middleware.postprocess(
+                    app=self, state=state, event=event, delta=delta
+                )
+            else:
+                out = middleware.postprocess(
+                    app=self, state=state, event=event, delta=delta
+                )
             if out is not None:
-                return out
+                return out  # type: ignore
 
     def add_middleware(self, middleware: Middleware, index: Optional[int] = None):
         """Add middleware to the app.
 
         Args:
             middleware: The middleware to add.
             index: The index to add the middleware at.
@@ -396,59 +409,68 @@
         compiler.compile_components(custom_components)
 
         self.state.convert_handlers_to_fns()
 
 
 async def process(
     app: App, event: Event, sid: str, headers: Dict, client_ip: str
-) -> StateUpdate:
+) -> List[StateUpdate]:
     """Process an event.
 
     Args:
         app: The app to process the event for.
         event: The event to process.
         sid: The Socket.IO session id.
         headers: The client headers.
         client_ip: The client_ip.
 
     Returns:
-        The state update after processing the event.
+        The state updates after processing the event.
     """
     # Get the state for the session.
     state = app.state_manager.get_state(event.token)
 
-    formatted_params = format.format_query_params(event.router_data)
-
-    # Pass router_data to the state of the App.
+    # Add request data to the state.
     state.router_data = event.router_data
-    # also pass router_data to all substates
+    state.router_data.update(
+        {
+            constants.RouteVar.QUERY: format.format_query_params(event.router_data),
+            constants.RouteVar.CLIENT_TOKEN: event.token,
+            constants.RouteVar.SESSION_ID: sid,
+            constants.RouteVar.HEADERS: headers,
+            constants.RouteVar.CLIENT_IP: client_ip,
+        }
+    )
+
+    # Also pass router_data to all substates. (TODO: this isn't recursive currently)
     for _, substate in state.substates.items():
-        substate.router_data = event.router_data
-    state.router_data[constants.RouteVar.QUERY] = formatted_params
-    state.router_data[constants.RouteVar.CLIENT_TOKEN] = event.token
-    state.router_data[constants.RouteVar.SESSION_ID] = sid
-    state.router_data[constants.RouteVar.HEADERS] = headers
-    state.router_data[constants.RouteVar.CLIENT_IP] = client_ip
+        substate.router_data = state.router_data
 
     # Preprocess the event.
-    pre = app.preprocess(state, event)
-    if pre is not None:
-        return StateUpdate(delta=pre)
+    pre = await app.preprocess(state, event)
+    if isinstance(pre, StateUpdate):
+        return [pre]
+    updates = pre
 
     # Apply the event to the state.
-    update = await state.process(event)
-    app.state_manager.set_state(event.token, state)
+    if updates is None:
+        updates = [await state.process(event)]
+        app.state_manager.set_state(event.token, state)
 
     # Postprocess the event.
-    post = app.postprocess(state, event, update.delta)
-    if post is not None:
-        return StateUpdate(delta=post)
+    post_list = []
+    for update in updates:
+        post = await app.postprocess(state, event, update.delta)  # type: ignore
+        post_list.append(post) if post else None
+
+    if len(post_list) > 0:
+        return [StateUpdate(delta=post) for post in post_list]
 
-    # Return the update.
-    return update
+    # Return the updates.
+    return updates
 
 
 async def ping() -> str:
     """Test API endpoint.
 
     Returns:
         The response.
@@ -574,19 +596,20 @@
             k.decode("utf-8"): v.decode("utf-8")
             for (k, v) in environ["asgi.scope"]["headers"]
         }
 
         # Get the client IP
         client_ip = environ["REMOTE_ADDR"]
 
-        # Process the event.
-        update = await process(self.app, event, sid, headers, client_ip)
+        # Process the events.
+        updates = await process(self.app, event, sid, headers, client_ip)
 
         # Emit the event.
-        await self.emit(str(constants.SocketEvent.EVENT), update.json(), to=sid)
+        for update in updates:
+            await self.emit(str(constants.SocketEvent.EVENT), update.json(), to=sid)  # type: ignore
 
     async def on_ping(self, sid):
         """Event for testing the API endpoint.
 
         Args:
             sid: The Socket.IO session id.
         """
```

### Comparing `pynecone-0.1.21a0/pynecone/base.py` & `pynecone-0.1.22a0/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/compiler/compiler.py` & `pynecone-0.1.22a0/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/compiler/templates.py` & `pynecone-0.1.22a0/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/compiler/utils.py` & `pynecone-0.1.22a0/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/__init__.py` & `pynecone-0.1.22a0/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/base/bare.py` & `pynecone-0.1.22a0/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/base/document.py` & `pynecone-0.1.22a0/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/base/link.py` & `pynecone-0.1.22a0/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/base/meta.py` & `pynecone-0.1.22a0/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/component.py` & `pynecone-0.1.22a0/pynecone/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,14 +505,16 @@
             if key not in props:
                 continue
             type_ = props[key]
             if types._issubclass(type_, EventChain):
                 value = self._create_event_chain(key, value)
                 self.props[format.to_camel_case(key)] = value
                 continue
+            if not types._issubclass(type_, Var):
+                type_ = Var[type_]
             type_ = types.get_args(type_)[0]
             if types._issubclass(type_, Base):
                 try:
                     value = BaseVar(name=value.json(), type_=type_, is_local=True)
                 except Exception:
                     value = Var.create(value)
             else:
```

### Comparing `pynecone-0.1.21a0/pynecone/components/datadisplay/code.py` & `pynecone-0.1.22a0/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.22a0/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.22a0/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/datadisplay/list.py` & `pynecone-0.1.22a0/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.22a0/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/datadisplay/table.py` & `pynecone-0.1.22a0/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.22a0/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.22a0/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/feedback/alert.py` & `pynecone-0.1.22a0/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.22a0/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/feedback/progress.py` & `pynecone-0.1.22a0/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.22a0/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/feedback/spinner.py` & `pynecone-0.1.22a0/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/__init__.py` & `pynecone-0.1.22a0/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/button.py` & `pynecone-0.1.22a0/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/checkbox.py` & `pynecone-0.1.22a0/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.22a0/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/editable.py` & `pynecone-0.1.22a0/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/formcontrol.py` & `pynecone-0.1.22a0/pynecone/components/forms/formcontrol.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.22a0/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/input.py` & `pynecone-0.1.22a0/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/numberinput.py` & `pynecone-0.1.22a0/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/pininput.py` & `pynecone-0.1.22a0/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/radio.py` & `pynecone-0.1.22a0/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.22a0/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/select.py` & `pynecone-0.1.22a0/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/slider.py` & `pynecone-0.1.22a0/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/switch.py` & `pynecone-0.1.22a0/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/textarea.py` & `pynecone-0.1.22a0/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/forms/upload.py` & `pynecone-0.1.22a0/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/graphing/plotly.py` & `pynecone-0.1.22a0/pynecone/components/graphing/plotly.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
     # The width of the graph.
     width: Var[str]
 
     # The height of the graph.
     height: Var[str]
 
+    # If true, the graph will resize when the window is resized.
+    use_resize_handler: Var[bool]
+
     def _get_imports(self):
         return {}
 
     def _get_custom_code(self) -> str:
         return """import dynamic from 'next/dynamic'
 const Plot = dynamic(() => import('react-plotly.js'), { ssr: false });
 """
```

### Comparing `pynecone-0.1.21a0/pynecone/components/graphing/victory.py` & `pynecone-0.1.22a0/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/__init__.py` & `pynecone-0.1.22a0/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/box.py` & `pynecone-0.1.22a0/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/cond.py` & `pynecone-0.1.22a0/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/flex.py` & `pynecone-0.1.22a0/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/foreach.py` & `pynecone-0.1.22a0/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/grid.py` & `pynecone-0.1.22a0/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/html.py` & `pynecone-0.1.22a0/pynecone/components/layout/html.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """A html component."""
 
-from typing import Dict
+from typing import Any
 
 from pynecone.components.layout.box import Box
-from pynecone.var import Var
 
 
 class Html(Box):
     """Render the html.
 
     Returns:
         The code to render the  html component.
     """
 
     # The HTML to render.
-    dangerouslySetInnerHTML: Var[Dict]
+    dangerouslySetInnerHTML: Any
 
     @classmethod
     def create(cls, *children, **props):
         """Create a html component.
 
         Args:
             *children: The children of the component.
```

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/responsive.py` & `pynecone-0.1.22a0/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/stack.py` & `pynecone-0.1.22a0/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/layout/wrap.py` & `pynecone-0.1.22a0/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/media/avatar.py` & `pynecone-0.1.22a0/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/media/icon.py` & `pynecone-0.1.22a0/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/media/image.py` & `pynecone-0.1.22a0/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.22a0/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/navigation/link.py` & `pynecone-0.1.22a0/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.22a0/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/overlay/__init__.py` & `pynecone-0.1.22a0/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.22a0/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/overlay/drawer.py` & `pynecone-0.1.22a0/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/overlay/menu.py` & `pynecone-0.1.22a0/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/overlay/modal.py` & `pynecone-0.1.22a0/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/overlay/popover.py` & `pynecone-0.1.22a0/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.22a0/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/tags/cond_tag.py` & `pynecone-0.1.22a0/pynecone/components/tags/cond_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.22a0/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/tags/tag.py` & `pynecone-0.1.22a0/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/tags/tagless.py` & `pynecone-0.1.22a0/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/components/typography/markdown.py` & `pynecone-0.1.22a0/pynecone/components/typography/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                     "h2": "{({node, ...props}) => <Heading size='xl' {...props} />}",
                     "h3": "{({node, ...props}) => <Heading size='lg' {...props} />}",
                     "ul": "{UnorderedList}",
                     "ol": "{OrderedList}",
                     "li": "{ListItem}",
                     "p": "{Text}",
                     "a": "{Link}",
-                    "code": """{({node, inline, className, children, ...props}) => 
+                    "code": """{({node, inline, className, children, ...props}) =>
                     {
         const match = (className || '').match(/language-(?<lang>.*)/);
         return !inline ? (
           <Prism
             children={String(children).replace(/\n$/, '')}
             language={match ? match[1] : ''}
             {...props}
```

### Comparing `pynecone-0.1.21a0/pynecone/constants.py` & `pynecone-0.1.22a0/pynecone/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 # The name of the pip install package.
 PACKAGE_NAME = "pynecone"
 # The current version of Pynecone.
 VERSION = pkg_resources.get_distribution(PACKAGE_NAME).version
 # Minimum version of Node.js required to run Pynecone.
 MIN_NODE_VERSION = "12.22.0"
 
+# Valid bun versions.
+MIN_BUN_VERSION = "0.5.5"
+MAX_BUN_VERSION = "0.5.8"
+INVALID_BUN_VERSIONS = ["0.5.6", "0.5.7"]
+
 # Files and directories used to init a new project.
 # The root directory of the pynecone library.
 ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 # The name of the file used for pc init.
 APP_TEMPLATE_FILE = "tutorial.py"
 # The name of the assets directory.
 APP_ASSETS_DIR = "assets"
```

### Comparing `pynecone-0.1.21a0/pynecone/event.py` & `pynecone-0.1.22a0/pynecone/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,14 +342,16 @@
     # If the handler returns a single event, wrap it in a list.
     if not isinstance(events, List):
         events = [events]
 
     # Fix the events created by the handler.
     out = []
     for e in events:
+        if not isinstance(e, (EventHandler, EventSpec)):
+            e = EventHandler(fn=e)
         # Otherwise, create an event from the event spec.
         if isinstance(e, EventHandler):
             e = e()
         assert isinstance(e, EventSpec), f"Unexpected event type, {type(e)}."
         name = format.format_event_handler(e.handler)
         payload = dict(e.args)
```

### Comparing `pynecone-0.1.21a0/pynecone/middleware/logging_middleware.py` & `pynecone-0.1.22a0/pynecone/middleware/logging_middleware.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 if TYPE_CHECKING:
     from pynecone.app import App
 
 
 class LoggingMiddleware(Middleware):
     """Middleware to log requests and responses."""
 
-    def preprocess(self, app: App, state: State, event: Event):
+    async def preprocess(self, app: App, state: State, event: Event):
         """Preprocess the event.
 
         Args:
             app: The app to apply the middleware to.
             state: The client state.
             event: The event to preprocess.
         """
         print(f"Event {event}")
 
-    def postprocess(self, app: App, state: State, event: Event, delta: Delta):
+    async def postprocess(self, app: App, state: State, event: Event, delta: Delta):
         """Postprocess the event.
 
         Args:
             app: The app to apply the middleware to.
             state: The client state.
             event: The event to postprocess.
             delta: The delta to postprocess.
```

### Comparing `pynecone-0.1.21a0/pynecone/middleware/middleware.py` & `pynecone-0.1.22a0/pynecone/middleware/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Base Pynecone middleware."""
 from __future__ import annotations
 
 from abc import ABC
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, List, Optional, Union
 
 from pynecone.base import Base
 from pynecone.event import Event
-from pynecone.state import Delta, State
+from pynecone.state import Delta, State, StateUpdate
 
 if TYPE_CHECKING:
     from pynecone.app import App
 
 
 class Middleware(Base, ABC):
     """Middleware to preprocess and postprocess requests."""
 
-    def preprocess(self, app: App, state: State, event: Event) -> Optional[Delta]:
+    async def preprocess(
+        self, app: App, state: State, event: Event
+    ) -> Optional[Union[StateUpdate, List[StateUpdate]]]:
         """Preprocess the event.
 
         Args:
             app: The app.
             state: The client state.
             event: The event to preprocess.
 
         Returns:
             An optional state to return.
         """
         return None
 
-    def postprocess(
+    async def postprocess(
         self, app: App, state: State, event: Event, delta
     ) -> Optional[Delta]:
         """Postprocess the event.
 
         Args:
             app: The app.
             state: The client state.
```

### Comparing `pynecone-0.1.21a0/pynecone/model.py` & `pynecone-0.1.22a0/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/pc.py` & `pynecone-0.1.22a0/pynecone/pc.py`

 * *Files identical despite different names*

```diff
@@ -199,20 +199,20 @@
     )
 
     # Post a telemetry event.
     pynecone_telemetry("export", get_config().telemetry_enabled)
 
     if zipping:
         console.rule(
-            """Backend & Frontend compiled. See [green bold]backend.zip[/green bold] 
+            """Backend & Frontend compiled. See [green bold]backend.zip[/green bold]
             and [green bold]frontend.zip[/green bold]."""
         )
     else:
         console.rule(
-            """Backend & Frontend compiled. See [green bold]app[/green bold] 
+            """Backend & Frontend compiled. See [green bold]app[/green bold]
             and [green bold].web/_static[/green bold] directories."""
         )
 
 
 main = cli
 
 if __name__ == "__main__":
```

### Comparing `pynecone-0.1.21a0/pynecone/route.py` & `pynecone-0.1.22a0/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/state.py` & `pynecone-0.1.22a0/pynecone/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,45 +542,73 @@
                 return self
             path = path[1:]
         if path[0] not in self.substates:
             raise ValueError(f"Invalid path: {path}")
         return self.substates[path[0]].get_substate(path[1:])
 
     async def process(self, event: Event) -> StateUpdate:
-        """Process an event.
+        """Obtain event info and process event.
 
         Args:
             event: The event to process.
 
         Returns:
             The state update after processing the event.
+
+        Raises:
+            ValueError: If the state value is None.
         """
         # Get the event handler.
         path = event.name.split(".")
         path, name = path[:-1], path[-1]
         substate = self.get_substate(path)
         handler = substate.event_handlers[name]  # type: ignore
 
-        # Process the event.
-        fn = functools.partial(handler.fn, substate)
+        if not substate:
+            raise ValueError(
+                "The value of state cannot be None when processing an event."
+            )
+
+        return await self.process_event(
+            handler=handler,
+            state=substate,
+            payload=event.payload,
+            token=event.token,
+        )
+
+    async def process_event(
+        self, handler: EventHandler, state: State, payload: Dict, token: str
+    ) -> StateUpdate:
+        """Process event.
+
+        Args:
+            handler: Eventhandler to process.
+            state: State to process the handler.
+            payload: The event payload.
+            token: Client token.
+
+        Returns:
+            The state update after processing the event.
+        """
+        fn = functools.partial(handler.fn, state)
         try:
             if asyncio.iscoroutinefunction(fn.func):
-                events = await fn(**event.payload)
+                events = await fn(**payload)
             else:
-                events = fn(**event.payload)
+                events = fn(**payload)
         except Exception:
             error = traceback.format_exc()
             print(error)
             events = fix_events(
-                [window_alert("An error occurred. See logs for details.")], event.token
+                [window_alert("An error occurred. See logs for details.")], token
             )
             return StateUpdate(events=events)
 
         # Fix the returned events.
-        events = fix_events(events, event.token)
+        events = fix_events(events, token)
 
         # Get the delta after processing the event.
         delta = self.get_delta()
 
         # Reset the dirty vars.
         self.clean()
```

### Comparing `pynecone-0.1.21a0/pynecone/style.py` & `pynecone-0.1.22a0/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/telemetry.py` & `pynecone-0.1.22a0/pynecone/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/utils/build.py` & `pynecone-0.1.22a0/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/utils/console.py` & `pynecone-0.1.22a0/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/utils/exec.py` & `pynecone-0.1.22a0/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/utils/format.py` & `pynecone-0.1.22a0/pynecone/utils/format.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/utils/imports.py` & `pynecone-0.1.22a0/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/utils/path_ops.py` & `pynecone-0.1.22a0/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/utils/prerequisites.py` & `pynecone-0.1.22a0/pynecone/utils/prerequisites.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,34 +37,56 @@
         version = result.stdout.decode().strip().split("v")[1]
         # Compare the version numbers
         return version.split(".") >= min_version.split(".")
     except Exception:
         return False
 
 
+def get_bun_version() -> str:
+    """Get the version of bun.
+
+    Returns:
+        The version of bun.
+
+    Raises:
+        FileNotFoundError: If bun is not installed.
+    """
+    try:
+        # Run the bun -v command and capture the output
+        result = subprocess.run(
+            ["bun", "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
+        )
+        version = result.stdout.decode().strip()
+        return version
+    except Exception:
+        raise FileNotFoundError("Pynecone requires bun to be installed.") from None
+
+
 def get_package_manager() -> str:
     """Get the package manager executable.
 
     Returns:
         The path to the package manager.
 
     Raises:
         FileNotFoundError: If bun or npm is not installed.
         Exit: If the app directory is invalid.
 
     """
+    config = get_config()
+
     # Check that the node version is valid.
     if not check_node_version(constants.MIN_NODE_VERSION):
         console.print(
             f"[red]Node.js version {constants.MIN_NODE_VERSION} or higher is required to run Pynecone."
         )
         raise typer.Exit()
 
     # On Windows, we use npm instead of bun.
-    if platform.system() == "Windows":
+    if platform.system() == "Windows" or config.disable_bun:
         npm_path = path_ops.which("npm")
         if npm_path is None:
             raise FileNotFoundError("Pynecone requires npm to be installed on Windows.")
         return npm_path
 
     # On other platforms, we use bun.
     return os.path.expandvars(get_config().bun_path)
@@ -188,14 +210,20 @@
 
 def install_bun():
     """Install bun onto the user's system.
 
     Raises:
         FileNotFoundError: If the required packages are not installed.
     """
+    if get_bun_version() in constants.INVALID_BUN_VERSIONS:
+        console.print(
+            f"[red]Bun version {get_bun_version()} is not supported by Pynecone. Please downgrade to bun version {constants.MIN_BUN_VERSION} or upgrade to {constants.MAX_BUN_VERSION} or higher."
+        )
+        return
+
     # Bun is not supported on Windows.
     if platform.system() == "Windows":
         console.log("Skipping bun installation on Windows.")
         return
 
     # Only install if bun is not already installed.
     if not os.path.exists(get_package_manager()):
```

### Comparing `pynecone-0.1.21a0/pynecone/utils/processes.py` & `pynecone-0.1.22a0/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/utils/types.py` & `pynecone-0.1.22a0/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/var.py` & `pynecone-0.1.22a0/pynecone/var.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pynecone/watch.py` & `pynecone-0.1.22a0/pynecone/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.21a0/pyproject.toml` & `pynecone-0.1.22a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.21a"
+version = "0.1.22a"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.21a0/PKG-INFO` & `pynecone-0.1.22a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.21a0
+Version: 0.1.22a0
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

