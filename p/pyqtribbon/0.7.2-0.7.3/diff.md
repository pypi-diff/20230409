# Comparing `tmp/pyqtribbon-0.7.2.tar.gz` & `tmp/pyqtribbon-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqtribbon-0.7.2.tar", last modified: Sat Apr  8 03:45:55 2023, max compression
+gzip compressed data, was "pyqtribbon-0.7.3.tar", last modified: Sun Apr  9 16:25:55 2023, max compression
```

## Comparing `pyqtribbon-0.7.2.tar` & `pyqtribbon-0.7.3.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.093880 pyqtribbon-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.077880 pyqtribbon-0.7.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.081880 pyqtribbon-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/CHANGE_LOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-08 03:45:55.093880 pyqtribbon-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.081880 pyqtribbon-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.081880 pyqtribbon-0.7.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.081880 pyqtribbon-0.7.2/docs/source/_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/category.png
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/category.py
--rw-r--r--   0 runner    (1001) docker     (123)    25735 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/panel.png
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/python.png
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/ribbonbar-customize.png
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/ribbonbar-customize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/ribbonbar.png
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/ribbonbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    26937 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/tutorial-ribbonbar.png
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_examples/tutorial-ribbonbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.081880 pyqtribbon-0.7.2/docs/source/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    44571 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_images/example.png
--rw-r--r--   0 runner    (1001) docker     (123)    57874 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_images/main-interface.png
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_images/ribbon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/_images/ribbon_no_callouts.png
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/ribbon.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/docs/source/user.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.085880 pyqtribbon-0.7.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/bold.png
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/copy-to-clipboard.png
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/copy.png
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/cut.png
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/decrease-font.png
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/increase-font.png
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/italic.png
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/lowercase.png
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/painter.png
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/paste-as-text.png
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/paste-shortcut.png
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/paste-special.png
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/paste.png
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/redo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/save.png
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/strikethrough.png
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/subscript.png
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/superscript.png
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/text-color.png
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/underline.png
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/undo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/word.png
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/examples/word.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.089880 pyqtribbon-0.7.2/pyqtribbon/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-08 03:45:54.000000 pyqtribbon-0.7.2/pyqtribbon/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.089880 pyqtribbon-0.7.2/pyqtribbon/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/backward.png
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/close.png
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/down.png
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/forward.png
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/help.png
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/linking.png
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/max.png
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/min.png
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/more.png
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/python.png
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/redo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/save.png
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/undo.png
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/icons/up.png
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    24026 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/panel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/ribbonbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/screenshotwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/separator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.089880 pyqtribbon-0.7.2/pyqtribbon/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/styles/base.qss
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/styles/debug.qss
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/styles/default.qss
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/tabbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/titlewidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/toolbutton.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/pyqtribbon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.089880 pyqtribbon-0.7.2/pyqtribbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-08 03:45:55.000000 pyqtribbon-0.7.2/pyqtribbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-08 03:45:55.000000 pyqtribbon-0.7.2/pyqtribbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 03:45:55.000000 pyqtribbon-0.7.2/pyqtribbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-08 03:45:55.000000 pyqtribbon-0.7.2/pyqtribbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 03:45:55.000000 pyqtribbon-0.7.2/pyqtribbon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.089880 pyqtribbon-0.7.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/requirements/PyQt5.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/requirements/PyQt6.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/requirements/PySide2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/requirements/PySide6.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/requirements/deps.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/requirements/dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.089880 pyqtribbon-0.7.2/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)    44120 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/screenshots/main.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 03:45:55.093880 pyqtribbon-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:55.093880 pyqtribbon-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/test_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/test_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/test_filemenu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/test_gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/test_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/test_ribbonbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/test_titlewidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tests/test_use_dictionary_to_create_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-08 03:45:44.000000 pyqtribbon-0.7.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.086497 pyqtribbon-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.058497 pyqtribbon-0.7.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.062497 pyqtribbon-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/CHANGE_LOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-09 16:25:55.086497 pyqtribbon-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.062497 pyqtribbon-0.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.062497 pyqtribbon-0.7.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.066497 pyqtribbon-0.7.3/docs/source/_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/category.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25735 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/panel.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/ribbonbar-customize.png
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/ribbonbar-customize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/ribbonbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/ribbonbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26937 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/tutorial-ribbonbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_examples/tutorial-ribbonbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.066497 pyqtribbon-0.7.3/docs/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    44571 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_images/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57874 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_images/main-interface.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_images/ribbon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/_images/ribbon_no_callouts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/ribbon.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/docs/source/user.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.074497 pyqtribbon-0.7.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/bold.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/copy-to-clipboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/copy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/cut.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/decrease-font.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/increase-font.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/italic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/lowercase.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/painter.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/paste-as-text.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/paste-shortcut.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/paste-special.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/paste.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/redo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/strikethrough.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/subscript.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/superscript.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/text-color.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/underline.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/word.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/examples/word.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.078498 pyqtribbon-0.7.3/pyqtribbon/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 16:25:54.000000 pyqtribbon-0.7.3/pyqtribbon/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.082497 pyqtribbon-0.7.3/pyqtribbon/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/backward.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/close.png
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/forward.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/linking.png
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/max.png
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/min.png
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/more.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/redo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/icons/up.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24026 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16461 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/panel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/ribbonbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/screenshotwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/separator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.082497 pyqtribbon-0.7.3/pyqtribbon/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/styles/base.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/styles/debug.qss
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/styles/default.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/tabbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/titlewidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/toolbutton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/pyqtribbon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.078498 pyqtribbon-0.7.3/pyqtribbon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-09 16:25:55.000000 pyqtribbon-0.7.3/pyqtribbon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-09 16:25:55.000000 pyqtribbon-0.7.3/pyqtribbon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:25:55.000000 pyqtribbon-0.7.3/pyqtribbon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-09 16:25:55.000000 pyqtribbon-0.7.3/pyqtribbon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 16:25:55.000000 pyqtribbon-0.7.3/pyqtribbon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.082497 pyqtribbon-0.7.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/requirements/PyQt5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/requirements/PyQt6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/requirements/PySide2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/requirements/PySide6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/requirements/deps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/requirements/dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.082497 pyqtribbon-0.7.3/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)    44120 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/screenshots/main.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 16:25:55.086497 pyqtribbon-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:55.086497 pyqtribbon-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_filemenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_ribbonbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_titlewidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tests/test_use_dictionary_to_create_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-09 16:25:43.000000 pyqtribbon-0.7.3/tox.ini
```

### Comparing `pyqtribbon-0.7.2/.github/release-drafter.yml` & `pyqtribbon-0.7.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/.github/release.yml` & `pyqtribbon-0.7.3/.github/release.yml`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/.github/workflows/publish.yml` & `pyqtribbon-0.7.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/.github/workflows/release-drafter.yml` & `pyqtribbon-0.7.3/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/.github/workflows/tests.yml` & `pyqtribbon-0.7.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/.gitignore` & `pyqtribbon-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/CHANGE_LOG.md` & `pyqtribbon-0.7.3/CHANGE_LOG.md`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/LICENSE` & `pyqtribbon-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/PKG-INFO` & `pyqtribbon-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtribbon
-Version: 0.7.2
+Version: 0.7.3
 Summary: Ribbon Bar for PyQt or PySide applications
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: GitHub, https://github.com/haiiliin/pyqtribbon
 Project-URL: Documentation, https://pyqtribbon.haiiliin.com/en/stable/
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyqtribbon-0.7.2/README.md` & `pyqtribbon-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/Makefile` & `pyqtribbon-0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/make.bat` & `pyqtribbon-0.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/category.png` & `pyqtribbon-0.7.3/docs/source/_examples/category.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/category.py` & `pyqtribbon-0.7.3/docs/source/_examples/category.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/panel.png` & `pyqtribbon-0.7.3/docs/source/_examples/panel.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/panel.py` & `pyqtribbon-0.7.3/docs/source/_examples/panel.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/python.png` & `pyqtribbon-0.7.3/docs/source/_examples/python.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/ribbonbar-customize.png` & `pyqtribbon-0.7.3/docs/source/_examples/ribbonbar-customize.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/ribbonbar-customize.py` & `pyqtribbon-0.7.3/docs/source/_examples/ribbonbar-customize.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/ribbonbar.png` & `pyqtribbon-0.7.3/docs/source/_examples/ribbonbar.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/tutorial-ribbonbar.png` & `pyqtribbon-0.7.3/docs/source/_examples/tutorial-ribbonbar.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_examples/tutorial-ribbonbar.py` & `pyqtribbon-0.7.3/docs/source/_examples/tutorial-ribbonbar.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_images/example.png` & `pyqtribbon-0.7.3/docs/source/_images/example.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_images/main-interface.png` & `pyqtribbon-0.7.3/docs/source/_images/main-interface.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_images/ribbon.png` & `pyqtribbon-0.7.3/docs/source/_images/ribbon.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/_images/ribbon_no_callouts.png` & `pyqtribbon-0.7.3/docs/source/_images/ribbon_no_callouts.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/conf.py` & `pyqtribbon-0.7.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/index.rst` & `pyqtribbon-0.7.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/ribbon.rst` & `pyqtribbon-0.7.3/docs/source/ribbon.rst`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/docs/source/user.rst` & `pyqtribbon-0.7.3/docs/source/user.rst`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/bold.png` & `pyqtribbon-0.7.3/examples/bold.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/copy-to-clipboard.png` & `pyqtribbon-0.7.3/examples/copy-to-clipboard.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/copy.png` & `pyqtribbon-0.7.3/examples/copy.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/cut.png` & `pyqtribbon-0.7.3/examples/cut.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/decrease-font.png` & `pyqtribbon-0.7.3/examples/decrease-font.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/increase-font.png` & `pyqtribbon-0.7.3/examples/increase-font.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/italic.png` & `pyqtribbon-0.7.3/examples/italic.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/lowercase.png` & `pyqtribbon-0.7.3/examples/lowercase.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/painter.png` & `pyqtribbon-0.7.3/examples/painter.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/paste-as-text.png` & `pyqtribbon-0.7.3/examples/paste-as-text.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/paste-shortcut.png` & `pyqtribbon-0.7.3/examples/paste-shortcut.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/paste-special.png` & `pyqtribbon-0.7.3/examples/paste-special.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/paste.png` & `pyqtribbon-0.7.3/examples/paste.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/redo.png` & `pyqtribbon-0.7.3/examples/redo.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/save.png` & `pyqtribbon-0.7.3/examples/save.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/strikethrough.png` & `pyqtribbon-0.7.3/examples/strikethrough.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/subscript.png` & `pyqtribbon-0.7.3/examples/subscript.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/superscript.png` & `pyqtribbon-0.7.3/examples/superscript.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/text-color.png` & `pyqtribbon-0.7.3/examples/text-color.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/underline.png` & `pyqtribbon-0.7.3/examples/underline.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/undo.png` & `pyqtribbon-0.7.3/examples/undo.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/word.png` & `pyqtribbon-0.7.3/examples/word.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/examples/word.py` & `pyqtribbon-0.7.3/examples/word.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/main.py` & `pyqtribbon-0.7.3/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     popupMenu.addAction(QtGui.QIcon("pyqtribbon/icons/close.png"), "Action 2")
     popupMenu.addSeparator()
     popupMenu.addWidget(QtWidgets.QLabel("This is a custom widget"))
     formLayout = popupMenu.addFormLayoutWidget()
     formLayout.addRow(QtWidgets.QLabel("Row 1"), QtWidgets.QLineEdit())
 
     categories = ribbon.addContextCategories('name', ['Context 4', 'Context 5'])
-    showCategoryButton45.clicked.connect(categories.setCategoriesVisible)  # type: ignore
+    showCategoryButton45.clicked.connect(lambda v: categories.setCategoriesVisible(v))  # PySide2 Bug: use lambda
 
     panel1 = categories['Context 4'].addPanel('Context 4 Panel 1')
     panel1.addLargeButton('Button 1', icon=QIcon('pyqtribbon/icons/close.png'))
     panel1.addLargeButton('Button 2', icon=QIcon('pyqtribbon/icons/close.png'))
     panel1.addLargeButton('Button 3', icon=QIcon('pyqtribbon/icons/close.png'))
 
     panel2 = categories['Context 5'].addPanel('Context 5 Panel 1')
```

### Comparing `pyqtribbon-0.7.2/pyproject.toml` & `pyqtribbon-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/category.py` & `pyqtribbon-0.7.3/pyqtribbon/category.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/constants.py` & `pyqtribbon-0.7.3/pyqtribbon/constants.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/gallery.py` & `pyqtribbon-0.7.3/pyqtribbon/gallery.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/close.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/close.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/help.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/help.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/linking.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/linking.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/max.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/max.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/min.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/min.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/more.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/more.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/python.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/python.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/redo.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/redo.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/save.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/save.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/icons/undo.png` & `pyqtribbon-0.7.3/pyqtribbon/icons/undo.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/logger.py` & `pyqtribbon-0.7.3/pyqtribbon/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 log = logging.getLogger(__name__)
 log.addHandler(logging.StreamHandler(stream=sys.stdout))
 
 
 class UncaughtHook(QtCore.QObject):
-
     def __init__(self, *args, **kwargs):
         super(UncaughtHook, self).__init__(*args, **kwargs)
 
         # this registers the exception_hook() function as hook with the Python interpreter
         sys.excepthook = self.exception_hook
 
     @staticmethod
```

### Comparing `pyqtribbon-0.7.2/pyqtribbon/menu.py` & `pyqtribbon-0.7.3/pyqtribbon/menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         :param spacing: The spacing.
         """
         spacer = QtWidgets.QLabel()
         spacer.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
         spacer.setFixedHeight(spacing)
         self.addWidget(spacer)
 
-    def addLabel(self, text: str = "", alignment = QtCore.Qt.AlignLeft):
+    def addLabel(self, text: str = "", alignment=QtCore.Qt.AlignLeft):
         """Add a label to the menu.
 
         :param text: The text of the label.
         :param alignment: The alignment of the label.
         """
         label = QtWidgets.QLabel(text)
         label.setAlignment(alignment)
@@ -107,11 +107,11 @@
     """
 
     actionAdded = QtCore.Signal(QtWidgets.QAction)
 
     def hideEvent(self, a0: QtGui.QHideEvent) -> None:
         self.show()
 
-    def actionEvent(self, a0: QtGui.QActionEvent) -> None:
-        if a0.type() == QtGui.QActionEvent.ActionAdded:
-            self.actionAdded.emit(a0.action())  # type: ignore
-        super().actionEvent(a0)
+    def addAction(self, *args, **kwargs) -> QtWidgets.QAction:
+        action = super().addAction(*args, **kwargs)
+        self.actionAdded.emit(action)
+        return action
```

### Comparing `pyqtribbon-0.7.2/pyqtribbon/panel.py` & `pyqtribbon-0.7.3/pyqtribbon/panel.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/panel.pyi` & `pyqtribbon-0.7.3/pyqtribbon/panel.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from qtpy import QtWidgets, QtGui, QtCore
 
 from .constants import ColumnWise, RibbonButtonStyle, Large, Small
 from .gallery import RibbonGallery
 from .separator import RibbonSeparator
 from .toolbutton import RibbonToolButton
 
-
 class RibbonPanelTitle(QtWidgets.QLabel): ...
 
 class RibbonGridLayoutManager(object):
     rows: int
     cells: np.ndarray
 
     def __init__(self, rows: int): ...
```

### Comparing `pyqtribbon-0.7.2/pyqtribbon/ribbonbar.py` & `pyqtribbon-0.7.3/pyqtribbon/ribbonbar.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/screenshotwindow.py` & `pyqtribbon-0.7.3/pyqtribbon/screenshotwindow.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/separator.py` & `pyqtribbon-0.7.3/pyqtribbon/separator.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/styles/base.qss` & `pyqtribbon-0.7.3/pyqtribbon/styles/base.qss`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/styles/debug.qss` & `pyqtribbon-0.7.3/pyqtribbon/styles/debug.qss`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/tabbar.py` & `pyqtribbon-0.7.3/pyqtribbon/tabbar.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/titlewidget.py` & `pyqtribbon-0.7.3/pyqtribbon/titlewidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     _quickAccessButtonHeight = 30
     _rightButtonHeight = 24
 
     # Mouse move events
     _start_point = None
     _window_point = None
 
-
     @typing.overload
     def __init__(self, title="PyQtRibbon", parent=None):
         pass
 
     @typing.overload
     def __init__(self, parent=None):
         pass
@@ -285,19 +284,19 @@
 
     def topLevelWidget(self) -> QtWidgets.QWidget:
         widget = self
         while widget.parentWidget():
             widget = widget.parentWidget()
         return widget
 
-    def mousePressEvent(self, e):
-        self._start_point = e.globalPos()
+    def mousePressEvent(self, e: QtGui.QMouseEvent):
+        self._start_point = e.pos()
         self._window_point = self.topLevelWidget().frameGeometry().topLeft()
 
-    def mouseMoveEvent(self, e):
-        relpos = e.globalPos() - self._start_point if self._start_point else None
+    def mouseMoveEvent(self, e: QtGui.QMouseEvent):
+        relpos = e.pos() - self._start_point if self._start_point else None
         self.topLevelWidget().move(self._window_point + relpos) if self._window_point and relpos else None
         self.topLevelWidget().windowHandle().startSystemMove()
 
-    def mouseDoubleClickEvent(self, e):
+    def mouseDoubleClickEvent(self, e: QtGui.QMouseEvent):
         mainwindow = self.topLevelWidget()
         mainwindow.showNormal() if mainwindow.isMaximized() else mainwindow.showMaximized()
```

### Comparing `pyqtribbon-0.7.2/pyqtribbon/toolbutton.py` & `pyqtribbon-0.7.3/pyqtribbon/toolbutton.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon/version.py` & `pyqtribbon-0.7.3/pyqtribbon/version.py`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/pyqtribbon.egg-info/PKG-INFO` & `pyqtribbon-0.7.3/pyqtribbon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtribbon
-Version: 0.7.2
+Version: 0.7.3
 Summary: Ribbon Bar for PyQt or PySide applications
 Author-email: WANG Hailin <hailin.wang@connect.polyu.hk>
 Project-URL: GitHub, https://github.com/haiiliin/pyqtribbon
 Project-URL: Documentation, https://pyqtribbon.haiiliin.com/en/stable/
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyqtribbon-0.7.2/pyqtribbon.egg-info/SOURCES.txt` & `pyqtribbon-0.7.3/pyqtribbon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,11 +106,12 @@
 requirements/dev.txt
 screenshots/main.png
 tests/__init__.py
 tests/test_categories.py
 tests/test_category.py
 tests/test_filemenu.py
 tests/test_gallery.py
+tests/test_main.py
 tests/test_panel.py
 tests/test_ribbonbar.py
 tests/test_titlewidget.py
 tests/test_use_dictionary_to_create_widgets.py
```

### Comparing `pyqtribbon-0.7.2/screenshots/main.png` & `pyqtribbon-0.7.3/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `pyqtribbon-0.7.2/tests/test_categories.py` & `pyqtribbon-0.7.3/tests/test_categories.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-import sys
-
+from pytestqt.qtbot import QtBot
 from qtpy import QtWidgets
 
 from pyqtribbon import RibbonBar
 from pyqtribbon.panel import RibbonPanel
 from pyqtribbon.toolbutton import RibbonToolButton
 
 
-def test_categories():
-    if __name__ == "__main__":
-        app = QtWidgets.QApplication(sys.argv)
-        # Central widget
-        window = QtWidgets.QMainWindow()
-
-        # Ribbon bar
-        ribbonbar = RibbonBar()
-        window.setMenuBar(ribbonbar)
-
-        categories = ribbonbar.addContextCategories("name", ["Context 1", "Context 2"])
-        assert isinstance(categories, dict)
-        assert len(categories) == 2
-        assert categories["Context 1"].title() == "Context 1"
-        assert categories["Context 2"].title() == "Context 2"
-
-        panel1 = categories["Context 1"].addPanel("Context 1 Panel 1")
-        button1 = panel1.addLargeButton("Button 1")
-        assert isinstance(panel1, RibbonPanel)
-        assert panel1.title() == "Context 1 Panel 1"
-        assert isinstance(button1, RibbonToolButton)
-        assert button1.text() == "Button 1"
-
-        panel2 = categories["Context 2"].addPanel("Context 2 Panel 1")
-        button2 = panel2.addLargeButton("Button 2")
-        assert isinstance(panel2, RibbonPanel)
-        assert panel2.title() == "Context 2 Panel 1"
-        assert isinstance(button2, RibbonToolButton)
-        assert button2.text() == "Button 2"
-
-        # Show the window
-        window.resize(1800, 350)
-        window.show()
-        sys.exit(app.exec_())
+def test_categories(qtbot: QtBot):
+    # Central widget
+    window = QtWidgets.QMainWindow()
+    window.show()
+    qtbot.addWidget(window)
+
+    # Ribbon bar
+    ribbonbar = RibbonBar()
+    window.setMenuBar(ribbonbar)
+
+    categories = ribbonbar.addContextCategories("name", ["Context 1", "Context 2"])
+    assert isinstance(categories, dict)
+    assert len(categories) == 2
+    assert categories["Context 1"].title() == "Context 1"
+    assert categories["Context 2"].title() == "Context 2"
+
+    panel1 = categories["Context 1"].addPanel("Context 1 Panel 1")
+    button1 = panel1.addLargeButton("Button 1")
+    assert isinstance(panel1, RibbonPanel)
+    assert panel1.title() == "Context 1 Panel 1"
+    assert isinstance(button1, RibbonToolButton)
+    assert button1.text() == "Button 1"
+
+    panel2 = categories["Context 2"].addPanel("Context 2 Panel 1")
+    button2 = panel2.addLargeButton("Button 2")
+    assert isinstance(panel2, RibbonPanel)
+    assert panel2.title() == "Context 2 Panel 1"
+    assert isinstance(button2, RibbonToolButton)
+    assert button2.text() == "Button 2"
+
+    # Show the window
+    window.resize(1800, 350)
```

### Comparing `pyqtribbon-0.7.2/tests/test_category.py` & `pyqtribbon-0.7.3/tests/test_category.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-import sys
-
+from pytestqt.qtbot import QtBot
 from qtpy import QtWidgets
 
 from pyqtribbon import RibbonBar
 
 
-def test_category():
-    if __name__ == "__main__":
-        app = QtWidgets.QApplication(sys.argv)
-        # Central widget
-        window = QtWidgets.QMainWindow()
-
-        # Ribbon bar
-        ribbonbar = RibbonBar()
-        window.setMenuBar(ribbonbar)
-
-        # Add a category
-        category = ribbonbar.addCategory("Category 1")
-        assert category.title() == "Category 1"
-        assert category in ribbonbar.categories().values()
-
-        # Show the window
-        window.resize(1800, 350)
-        window.show()
-        sys.exit(app.exec_())
+def test_category(qtbot: QtBot):
+    # Central widget
+    window = QtWidgets.QMainWindow()
+    window.show()
+    qtbot.addWidget(window)
+
+    # Ribbon bar
+    ribbonbar = RibbonBar()
+    window.setMenuBar(ribbonbar)
+
+    # Add a category
+    category = ribbonbar.addCategory("Category 1")
+    assert category.title() == "Category 1"
+    assert category in ribbonbar.categories().values()
+
+    # Show the window
+    window.resize(1800, 350)
```

### Comparing `pyqtribbon-0.7.2/tests/test_filemenu.py` & `pyqtribbon-0.7.3/tests/test_filemenu.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-import sys
-
+from pytestqt.qtbot import QtBot
 from qtpy import QtWidgets
 
 from pyqtribbon import RibbonBar
 
 
-def test_filemenu():
-    if __name__ == "__main__":
-        app = QtWidgets.QApplication(sys.argv)
-        # Central widget
-        window = QtWidgets.QMainWindow()
-
-        # Ribbon bar
-        ribbonbar = RibbonBar()
-        window.setMenuBar(ribbonbar)
-
-        fileMenu = ribbonbar.applicationOptionButton().addFileMenu()
-        submenu = fileMenu.addMenu("Submenu")
-        action1 = submenu.addAction("Action 1")
-        assert action1.text() == "Action 1"
-        assert action1 in submenu.actions()
-
-        fileMenu.addSeparator()
-
-        action2 = fileMenu.addAction("Action 2")
-        assert action2.text() == "Action 2"
-        assert action2 in fileMenu.actions()
-
-        # Show the window
-        window.resize(1800, 350)
-        window.show()
-        sys.exit(app.exec_())
+def test_filemenu(qtbot: QtBot):
+    window = QtWidgets.QMainWindow()
+    window.show()
+    qtbot.addWidget(window)
+
+    # Ribbon bar
+    ribbonbar = RibbonBar()
+    window.setMenuBar(ribbonbar)
+
+    fileMenu = ribbonbar.applicationOptionButton().addFileMenu()
+    submenu = fileMenu.addMenu("Submenu")
+    action1 = submenu.addAction("Action 1")
+    assert action1.text() == "Action 1"
+    assert action1 in submenu.actions()
+
+    fileMenu.addSeparator()
+
+    action2 = fileMenu.addAction("Action 2")
+    assert action2.text() == "Action 2"
+    assert action2 in fileMenu.actions()
+
+    # Show the window
+    window.resize(1800, 350)
```

### Comparing `pyqtribbon-0.7.2/tests/test_gallery.py` & `pyqtribbon-0.7.3/tests/test_gallery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-import sys
-
+from pytestqt.qtbot import QtBot
 from qtpy import QtWidgets
 
 from pyqtribbon import RibbonBar
 from pyqtribbon.gallery import RibbonGallery
 
 
-def test_ribbonbar():
-    if __name__ == "__main__":
-        app = QtWidgets.QApplication(sys.argv)
-        # Central widget
-        window = QtWidgets.QMainWindow()
-
-        # Ribbon bar
-        ribbonbar = RibbonBar()
-        window.setMenuBar(ribbonbar)
-
-        category = ribbonbar.addCategory("name")
-        panel = category.addPanel("Panel 1")
-
-        gallery = panel.addGallery(popupHideOnClick=True)
-        for i in range(100):
-            gallery.addToggleButton(f"item {i + 1}")
-        popupMenu = gallery.popupMenu()
-        submenu = popupMenu.addMenu("Submenu")
-        submenu.addAction("Action 1")
-        popupMenu.addAction("Action 2")
-        popupMenu.addSeparator()
-        popupMenu.addWidget(QtWidgets.QLabel("This is a custom widget"))
-        formLayout = popupMenu.addFormLayoutWidget()
-        formLayout.addRow(QtWidgets.QLabel("Row 1"), QtWidgets.QLineEdit("Line Edit"))
-
-        assert isinstance(gallery, RibbonGallery)
-        assert gallery.popupMenu() is not None
-        assert gallery.popupMenu().actions()[0].text() == "Submenu"
-        assert submenu.actions()[0].text() == "Action 1"
-        assert gallery.popupMenu().actions()[1].text() == "Action 2"
-        assert gallery.popupMenu().actions()[2].isSeparator()
-        assert gallery.popupMenu().actions()[3].defaultWidget().text() == "This is a custom widget"
-        assert isinstance(formLayout, QtWidgets.QFormLayout)
-        assert formLayout.itemAt(0, QtWidgets.QFormLayout.LabelRole).widget().text() == "Row 1"
-        assert formLayout.itemAt(0, QtWidgets.QFormLayout.FieldRole).widget().text() == "Line Edit"
-
-        # Show the window
-        window.resize(1800, 350)
-        window.show()
-        sys.exit(app.exec_())
+def test_ribbonbar(qtbot: QtBot):
+    # Central widget
+    window = QtWidgets.QMainWindow()
+    window.show()
+    qtbot.addWidget(window)
+
+    # Ribbon bar
+    ribbonbar = RibbonBar()
+    window.setMenuBar(ribbonbar)
+
+    category = ribbonbar.addCategory("name")
+    panel = category.addPanel("Panel 1")
+
+    gallery = panel.addGallery(popupHideOnClick=True)
+    for i in range(100):
+        gallery.addToggleButton(f"item {i + 1}")
+    popupMenu = gallery.popupMenu()
+    submenu = popupMenu.addMenu("Submenu")
+    submenu.addAction("Action 1")
+    popupMenu.addAction("Action 2")
+    popupMenu.addSeparator()
+    popupMenu.addWidget(QtWidgets.QLabel("This is a custom widget"))
+    formLayout = popupMenu.addFormLayoutWidget()
+    formLayout.addRow(QtWidgets.QLabel("Row 1"), QtWidgets.QLineEdit("Line Edit"))
+
+    assert isinstance(gallery, RibbonGallery)
+    assert gallery.popupMenu() is not None
+    assert gallery.popupMenu().actions()[0].text() == "Submenu"
+    assert submenu.actions()[0].text() == "Action 1"
+    assert gallery.popupMenu().actions()[1].text() == "Action 2"
+    assert gallery.popupMenu().actions()[2].isSeparator()
+    assert gallery.popupMenu().actions()[3].defaultWidget().text() == "This is a custom widget"
+    assert isinstance(formLayout, QtWidgets.QFormLayout)
+    assert formLayout.itemAt(0, QtWidgets.QFormLayout.LabelRole).widget().text() == "Row 1"
+    assert formLayout.itemAt(0, QtWidgets.QFormLayout.FieldRole).widget().text() == "Line Edit"
+
+    # Show the window
+    window.resize(1800, 350)
```

### Comparing `pyqtribbon-0.7.2/tests/test_panel.py` & `pyqtribbon-0.7.3/tests/test_panel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-import sys
-
+from pytestqt.qtbot import QtBot
 from qtpy import QtWidgets
 
 from pyqtribbon import RibbonBar
 
 
-def test_panel():
-    if __name__ == "__main__":
-        app = QtWidgets.QApplication(sys.argv)
-        # Central widget
-        window = QtWidgets.QMainWindow()
-
-        # Ribbon bar
-        ribbonbar = RibbonBar()
-        window.setMenuBar(ribbonbar)
-
-        # Add a category
-        category = ribbonbar.addCategory("Category 1")
-        assert category.title() == "Category 1"
-        assert category in ribbonbar.categories().values()
-
-        # Add a panel
-        panel = category.addPanel("Panel 1")
-        assert panel.title() == "Panel 1"
-        assert panel in category.panels().values()
-
-        button1 = panel.addButton("Button 1")
-        assert button1.text() == "Button 1"
-        assert button1 in panel.widgets()
-        button2 = panel.addButton("Button 2")
-        assert button2.text() == "Button 2"
-        assert button2 in panel.widgets()
-
-        # Show the window
-        window.resize(1800, 350)
-        window.show()
-        sys.exit(app.exec_())
+def test_panel(qtbot: QtBot):
+    # Central widget
+    window = QtWidgets.QMainWindow()
+    window.show()
+    qtbot.addWidget(window)
+
+    # Ribbon bar
+    ribbonbar = RibbonBar()
+    window.setMenuBar(ribbonbar)
+
+    # Add a category
+    category = ribbonbar.addCategory("Category 1")
+    assert category.title() == "Category 1"
+    assert category in ribbonbar.categories().values()
+
+    # Add a panel
+    panel = category.addPanel("Panel 1")
+    assert panel.title() == "Panel 1"
+    assert panel in category.panels().values()
+
+    button1 = panel.addButton("Button 1")
+    assert button1.text() == "Button 1"
+    assert button1 in panel.widgets()
+    button2 = panel.addButton("Button 2")
+    assert button2.text() == "Button 2"
+    assert button2 in panel.widgets()
+
+    # Show the window
+    window.resize(1800, 350)
```

### Comparing `pyqtribbon-0.7.2/tests/test_titlewidget.py` & `pyqtribbon-0.7.3/tests/test_titlewidget.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from pytestqt.qtbot import QtBot
 from qtpy import QtCore
 
 from pyqtribbon.titlewidget import RibbonTitleWidget
-from pytestqt.qtbot import QtBot
 
 
 def test_titlewidget(qtbot: QtBot):
     # Add the widget to the test
     titlewidget = RibbonTitleWidget()
     titlewidget.setMouseTracking(True)
     titlewidget.show()
```

### Comparing `pyqtribbon-0.7.2/tests/test_use_dictionary_to_create_widgets.py` & `pyqtribbon-0.7.3/tests/test_use_dictionary_to_create_widgets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,84 +1,81 @@
-import sys
-
+from pytestqt.qtbot import QtBot
 from qtpy import QtWidgets
 
 from pyqtribbon import RibbonBar, RibbonCategoryStyle
 
 
-def test_filemenu():
-    if __name__ == "__main__":
-        app = QtWidgets.QApplication(sys.argv)
-        # Central widget
-        window = QtWidgets.QMainWindow()
-
-        # Ribbon bar
-        ribbonbar = RibbonBar()
-        window.setMenuBar(ribbonbar)
-
-        categories1 = ribbonbar.addCategoriesBy(
-            {
-                "Category 6": {
-                    "style": RibbonCategoryStyle.Normal,
-                    "panels": {
-                        "Panel 1": {
-                            "showPanelOptionButton": True,
-                            "widgets": {
-                                "Button 1": {
-                                    "type": "Button",
-                                    "arguments": {
-                                        "text": "Button",
-                                        "tooltip": "This is a tooltip",
-                                    },
+def test_filemenu(qtbot: QtBot):
+    # Central widget
+    window = QtWidgets.QMainWindow()
+    window.show()
+    qtbot.addWidget(window)
+
+    # Ribbon bar
+    ribbonbar = RibbonBar()
+    window.setMenuBar(ribbonbar)
+
+    categories1 = ribbonbar.addCategoriesBy(
+        {
+            "Category 6": {
+                "style": RibbonCategoryStyle.Normal,
+                "panels": {
+                    "Panel 1": {
+                        "showPanelOptionButton": True,
+                        "widgets": {
+                            "Button 1": {
+                                "type": "Button",
+                                "arguments": {
+                                    "text": "Button",
+                                    "tooltip": "This is a tooltip",
                                 },
-                                "Button 2": {
-                                    "type": "Button",
-                                    "arguments": {
-                                        "text": "Button 2",
-                                        "tooltip": "This is a tooltip",
-                                    },
+                            },
+                            "Button 2": {
+                                "type": "Button",
+                                "arguments": {
+                                    "text": "Button 2",
+                                    "tooltip": "This is a tooltip",
                                 },
                             },
                         },
-                        "Panel 2": {
-                            "showPanelOptionButton": False,
-                            "widgets": {
-                                "Button 3": {
-                                    "type": "Button",
-                                    "arguments": {
-                                        "text": "Button 3",
-                                        "tooltip": "This is a tooltip",
-                                    },
+                    },
+                    "Panel 2": {
+                        "showPanelOptionButton": False,
+                        "widgets": {
+                            "Button 3": {
+                                "type": "Button",
+                                "arguments": {
+                                    "text": "Button 3",
+                                    "tooltip": "This is a tooltip",
                                 },
-                                "Button 4": {
-                                    "type": "Button",
-                                    "arguments": {
-                                        "text": "Button 4",
-                                        "tooltip": "This is a tooltip",
-                                    },
+                            },
+                            "Button 4": {
+                                "type": "Button",
+                                "arguments": {
+                                    "text": "Button 4",
+                                    "tooltip": "This is a tooltip",
                                 },
                             },
                         },
                     },
-                }
+                },
             }
-        )
+        }
+    )
+
+    assert categories1["Category 6"].title() == "Category 6"
+    assert categories1["Category 6"].categoryStyle() == RibbonCategoryStyle.Normal
+    assert categories1["Category 6"].panels()["Panel 1"].title() == "Panel 1"
+    assert categories1["Category 6"].panels()["Panel 1"]._showPanelOptionButton
+    assert categories1["Category 6"].panels()["Panel 1"].widgets()[0].text() == "Button"
+    assert categories1["Category 6"].panels()["Panel 1"].widgets()[0].toolTip() == "This is a tooltip"
+    assert categories1["Category 6"].panels()["Panel 1"].widgets()[1].text() == "Button 2"
+    assert categories1["Category 6"].panels()["Panel 1"].widgets()[1].toolTip() == "This is a tooltip"
+    assert categories1["Category 6"].panels()["Panel 2"].title() == "Panel 2"
+    assert not categories1["Category 6"].panels()["Panel 2"]._showPanelOptionButton
+    assert categories1["Category 6"].panels()["Panel 2"].widgets()[0].text() == "Button 3"
+    assert categories1["Category 6"].panels()["Panel 2"].widgets()[0].toolTip() == "This is a tooltip"
+    assert categories1["Category 6"].panels()["Panel 2"].widgets()[1].text() == "Button 4"
+    assert categories1["Category 6"].panels()["Panel 2"].widgets()[1].toolTip() == "This is a tooltip"
 
-        assert categories1["Category 6"].title() == "Category 6"
-        assert categories1["Category 6"].categoryStyle() == RibbonCategoryStyle.Normal
-        assert categories1["Category 6"].panels()["Panel 1"].title() == "Panel 1"
-        assert categories1["Category 6"].panels()["Panel 1"]._showPanelOptionButton
-        assert categories1["Category 6"].panels()["Panel 1"].widgets()[0].text() == "Button"
-        assert categories1["Category 6"].panels()["Panel 1"].widgets()[0].toolTip() == "This is a tooltip"
-        assert categories1["Category 6"].panels()["Panel 1"].widgets()[1].text() == "Button 2"
-        assert categories1["Category 6"].panels()["Panel 1"].widgets()[1].toolTip() == "This is a tooltip"
-        assert categories1["Category 6"].panels()["Panel 2"].title() == "Panel 2"
-        assert not categories1["Category 6"].panels()["Panel 2"]._showPanelOptionButton
-        assert categories1["Category 6"].panels()["Panel 2"].widgets()[0].text() == "Button 3"
-        assert categories1["Category 6"].panels()["Panel 2"].widgets()[0].toolTip() == "This is a tooltip"
-        assert categories1["Category 6"].panels()["Panel 2"].widgets()[1].text() == "Button 4"
-        assert categories1["Category 6"].panels()["Panel 2"].widgets()[1].toolTip() == "This is a tooltip"
-
-        # Show the window
-        window.resize(1800, 350)
-        window.show()
-        sys.exit(app.exec_())
+    # Show the window
+    window.resize(1800, 350)
```

