# Comparing `tmp/nod-1.8.1.tar.gz` & `tmp/nod-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nod-1.8.1.tar", last modified: Tue Aug  2 15:13:41 2022, max compression
+gzip compressed data, was "nod-1.9.0.tar", last modified: Sun Apr  9 13:35:12 2023, max compression
```

## Comparing `nod-1.8.1.tar` & `nod-1.9.0.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.154636 nod-1.8.1/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.013264 nod-1.8.1/.github/
--rw-r--r--   0 runner     (501) staff       (20)      610 2022-08-02 15:12:16.000000 nod-1.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.013778 nod-1.8.1/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     4589 2022-08-02 15:12:16.000000 nod-1.8.1/.github/workflows/python.yml
--rw-r--r--   0 runner     (501) staff       (20)     1246 2022-08-02 15:12:16.000000 nod-1.8.1/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)       89 2022-08-02 15:12:16.000000 nod-1.8.1/.gitmodules
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.016065 nod-1.8.1/.idea/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.016520 nod-1.8.1/.idea/markdown-navigator/
--rw-r--r--   0 runner     (501) staff       (20)      104 2022-08-02 15:12:16.000000 nod-1.8.1/.idea/markdown-navigator/profiles_settings.xml
--rw-r--r--   0 runner     (501) staff       (20)     4167 2022-08-02 15:12:16.000000 nod-1.8.1/.idea/markdown-navigator.xml
--rw-r--r--   0 runner     (501) staff       (20)      185 2022-08-02 15:12:16.000000 nod-1.8.1/.idea/misc.xml
--rw-r--r--   0 runner     (501) staff       (20)      264 2022-08-02 15:12:16.000000 nod-1.8.1/.idea/modules.xml
--rw-r--r--   0 runner     (501) staff       (20)      317 2022-08-02 15:12:16.000000 nod-1.8.1/.idea/py-nod.iml
--rw-r--r--   0 runner     (501) staff       (20)      397 2022-08-02 15:12:16.000000 nod-1.8.1/.idea/vcs.xml
--rw-r--r--   0 runner     (501) staff       (20)      668 2022-08-02 15:12:16.000000 nod-1.8.1/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1087 2022-08-02 15:12:16.000000 nod-1.8.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       84 2022-08-02 15:12:16.000000 nod-1.8.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2196 2022-08-02 15:13:41.154870 nod-1.8.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1421 2022-08-02 15:12:16.000000 nod-1.8.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)   637916 2022-08-02 15:13:39.000000 nod-1.8.1/_nod.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9382 2022-08-02 15:12:16.000000 nod-1.8.1/_nod.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.016973 nod-1.8.1/ci-scripts/
--rwxr-xr-x   0 runner     (501) staff       (20)      697 2022-08-02 15:12:16.000000 nod-1.8.1/ci-scripts/build.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:40.995149 nod-1.8.1/external/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.020397 nod-1.8.1/external/nod/
--rw-r--r--   0 runner     (501) staff       (20)       40 2022-08-02 15:12:17.000000 nod-1.8.1/external/nod/.git
--rw-r--r--   0 runner     (501) staff       (20)       88 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)       80 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/.gitmodules
--rw-r--r--   0 runner     (501) staff       (20)     3124 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      101 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/Config.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     1146 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     2465 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.021748 nod-1.8.1/external/nod/driver/
--rw-r--r--   0 runner     (501) staff       (20)      365 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/driver/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      390 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/driver/app.manifest
--rw-r--r--   0 runner     (501) staff       (20)     8833 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/driver/main.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:40.995720 nod-1.8.1/external/nod/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.026983 nod-1.8.1/external/nod/include/nod/
--rw-r--r--   0 runner     (501) staff       (20)     1585 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/DirectoryEnumerator.hpp
--rw-r--r--   0 runner     (501) staff       (20)    14939 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/DiscBase.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1054 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/DiscGCN.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1074 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/DiscWii.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1807 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/IDiscIO.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2320 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/IFileIO.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2778 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/OSUTF.h
--rw-r--r--   0 runner     (501) staff       (20)     5527 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/Util.hpp
--rw-r--r--   0 runner     (501) staff       (20)      437 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/aes.hpp
--rw-r--r--   0 runner     (501) staff       (20)      415 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/nod.hpp
--rw-r--r--   0 runner     (501) staff       (20)      782 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/include/nod/sha1.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.034963 nod-1.8.1/external/nod/lib/
--rw-r--r--   0 runner     (501) staff       (20)     1270 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     8070 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/DirectoryEnumerator.cpp
--rw-r--r--   0 runner     (501) staff       (20)    29883 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/DiscBase.cpp
--rw-r--r--   0 runner     (501) staff       (20)    14099 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/DiscGCN.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1759 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/DiscIOISO.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8939 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/DiscIONFS.cpp
--rw-r--r--   0 runner     (501) staff       (20)     9130 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/DiscIOWBFS.cpp
--rw-r--r--   0 runner     (501) staff       (20)    43036 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/DiscWii.cpp
--rw-r--r--   0 runner     (501) staff       (20)     4533 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/FileIOFILE.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6852 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/FileIOWin32.cpp
--rw-r--r--   0 runner     (501) staff       (20)   295791 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/OSUTF.c
--rw-r--r--   0 runner     (501) staff       (20)     1868 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/Util.cpp
--rw-r--r--   0 runner     (501) staff       (20)    15260 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/aes.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2398 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/nod.cpp
--rw-r--r--   0 runner     (501) staff       (20)     8616 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/lib/sha1.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.037163 nod-1.8.1/external/nod/logvisor/
--rw-r--r--   0 runner     (501) staff       (20)       60 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/.git
--rw-r--r--   0 runner     (501) staff       (20)       84 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/.gitmodules
--rw-r--r--   0 runner     (501) staff       (20)     3538 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      111 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/Config.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     1151 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.041252 nod-1.8.1/external/nod/logvisor/fmt/
--rw-r--r--   0 runner     (501) staff       (20)      231 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/.clang-format
--rw-r--r--   0 runner     (501) staff       (20)       75 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/.git
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.041740 nod-1.8.1/external/nod/logvisor/fmt/.github/
--rw-r--r--   0 runner     (501) staff       (20)      293 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/.github/pull_request_template.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.043606 nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)      591 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/doc.yml
--rw-r--r--   0 runner     (501) staff       (20)     2282 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/linux.yml
--rw-r--r--   0 runner     (501) staff       (20)     1051 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/macos.yml
--rw-r--r--   0 runner     (501) staff       (20)     1782 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/windows.yml
--rw-r--r--   0 runner     (501) staff       (20)      397 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)    14760 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      710 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/CONTRIBUTING.md
--rw-r--r--   0 runner     (501) staff       (20)   173916 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/ChangeLog.rst
--rw-r--r--   0 runner     (501) staff       (20)     1408 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/LICENSE.rst
--rw-r--r--   0 runner     (501) staff       (20)    19374 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.048167 nod-1.8.1/external/nod/logvisor/fmt/doc/
--rw-r--r--   0 runner     (501) staff       (20)      569 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.049336 nod-1.8.1/external/nod/logvisor/fmt/doc/_static/
--rw-r--r--   0 runner     (501) staff       (20)    35951 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/_static/bootstrap.min.js
--rw-r--r--   0 runner     (501) staff       (20)      540 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/_static/breathe.css
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.052732 nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/
--rw-r--r--   0 runner     (501) staff       (20)    20335 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner     (501) staff       (20)    62927 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner     (501) staff       (20)    41280 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner     (501) staff       (20)    23320 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.053772 nod-1.8.1/external/nod/logvisor/fmt/doc/_templates/
--rw-r--r--   0 runner     (501) staff       (20)     5155 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/_templates/layout.html
--rw-r--r--   0 runner     (501) staff       (20)     1938 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/_templates/search.html
--rw-r--r--   0 runner     (501) staff       (20)    17099 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/api.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.055214 nod-1.8.1/external/nod/logvisor/fmt/doc/basic-bootstrap/
--rw-r--r--   0 runner     (501) staff       (20)      141 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/basic-bootstrap/README
--rw-r--r--   0 runner     (501) staff       (20)     7570 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/basic-bootstrap/layout.html
--rw-r--r--   0 runner     (501) staff       (20)       24 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/basic-bootstrap/theme.conf
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.074880 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/
--rw-r--r--   0 runner     (501) staff       (20)     1518 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/alerts.less
--rw-r--r--   0 runner     (501) staff       (20)     1201 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/badges.less
--rw-r--r--   0 runner     (501) staff       (20)     1121 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/bootstrap.less
--rw-r--r--   0 runner     (501) staff       (20)      594 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/breadcrumbs.less
--rw-r--r--   0 runner     (501) staff       (20)     5659 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/button-groups.less
--rw-r--r--   0 runner     (501) staff       (20)     3565 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/buttons.less
--rw-r--r--   0 runner     (501) staff       (20)     5405 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/carousel.less
--rw-r--r--   0 runner     (501) staff       (20)      764 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/close.less
--rw-r--r--   0 runner     (501) staff       (20)     1401 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/code.less
--rw-r--r--   0 runner     (501) staff       (20)      666 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/component-animations.less
--rw-r--r--   0 runner     (501) staff       (20)     4764 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/dropdowns.less
--rw-r--r--   0 runner     (501) staff       (20)    14935 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/forms.less
--rw-r--r--   0 runner     (501) staff       (20)    19803 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/glyphicons.less
--rw-r--r--   0 runner     (501) staff       (20)     1390 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/grid.less
--rw-r--r--   0 runner     (501) staff       (20)     4215 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/input-groups.less
--rw-r--r--   0 runner     (501) staff       (20)      993 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/jumbotron.less
--rw-r--r--   0 runner     (501) staff       (20)     1079 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/labels.less
--rw-r--r--   0 runner     (501) staff       (20)     3022 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/list-group.less
--rw-r--r--   0 runner     (501) staff       (20)      780 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/media.less
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.088283 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/
--rw-r--r--   0 runner     (501) staff       (20)      257 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/alerts.less
--rw-r--r--   0 runner     (501) staff       (20)      139 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/background-variant.less
--rw-r--r--   0 runner     (501) staff       (20)      468 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/border-radius.less
--rw-r--r--   0 runner     (501) staff       (20)     1080 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/buttons.less
--rw-r--r--   0 runner     (501) staff       (20)      120 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/center-block.less
--rw-r--r--   0 runner     (501) staff       (20)      605 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/clearfix.less
--rw-r--r--   0 runner     (501) staff       (20)     2641 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/forms.less
--rw-r--r--   0 runner     (501) staff       (20)     4388 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/gradients.less
--rw-r--r--   0 runner     (501) staff       (20)     2784 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/grid-framework.less
--rw-r--r--   0 runner     (501) staff       (20)     3094 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/grid.less
--rw-r--r--   0 runner     (501) staff       (20)      579 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/hide-text.less
--rw-r--r--   0 runner     (501) staff       (20)     1062 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/image.less
--rw-r--r--   0 runner     (501) staff       (20)      161 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/labels.less
--rw-r--r--   0 runner     (501) staff       (20)      533 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/list-group.less
--rw-r--r--   0 runner     (501) staff       (20)      232 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/nav-divider.less
--rw-r--r--   0 runner     (501) staff       (20)      364 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/nav-vertical-align.less
--rw-r--r--   0 runner     (501) staff       (20)      148 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/opacity.less
--rw-r--r--   0 runner     (501) staff       (20)      438 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/pagination.less
--rw-r--r--   0 runner     (501) staff       (20)      537 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/panels.less
--rw-r--r--   0 runner     (501) staff       (20)      191 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/progress-bar.less
--rw-r--r--   0 runner     (501) staff       (20)      248 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/reset-filter.less
--rw-r--r--   0 runner     (501) staff       (20)      196 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/resize.less
--rw-r--r--   0 runner     (501) staff       (20)      343 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/responsive-visibility.less
--rw-r--r--   0 runner     (501) staff       (20)      127 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/size.less
--rw-r--r--   0 runner     (501) staff       (20)      159 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/tab-focus.less
--rw-r--r--   0 runner     (501) staff       (20)      700 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/table-row.less
--rw-r--r--   0 runner     (501) staff       (20)      116 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/text-emphasis.less
--rw-r--r--   0 runner     (501) staff       (20)      162 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/text-overflow.less
--rw-r--r--   0 runner     (501) staff       (20)     6650 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/vendor-prefixes.less
--rw-r--r--   0 runner     (501) staff       (20)     1102 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins.less
--rw-r--r--   0 runner     (501) staff       (20)     3565 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/modals.less
--rw-r--r--   0 runner     (501) staff       (20)    14634 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/navbar.less
--rw-r--r--   0 runner     (501) staff       (20)     4930 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/navs.less
--rw-r--r--   0 runner     (501) staff       (20)     7650 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/normalize.less
--rw-r--r--   0 runner     (501) staff       (20)      861 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/pager.less
--rw-r--r--   0 runner     (501) staff       (20)     2001 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/pagination.less
--rw-r--r--   0 runner     (501) staff       (20)     6151 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/panels.less
--rw-r--r--   0 runner     (501) staff       (20)     3509 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/popovers.less
--rw-r--r--   0 runner     (501) staff       (20)     2133 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/print.less
--rw-r--r--   0 runner     (501) staff       (20)     1925 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/progress-bars.less
--rw-r--r--   0 runner     (501) staff       (20)      546 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/responsive-embed.less
--rw-r--r--   0 runner     (501) staff       (20)     4262 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/responsive-utilities.less
--rw-r--r--   0 runner     (501) staff       (20)     3122 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/scaffolding.less
--rw-r--r--   0 runner     (501) staff       (20)     4612 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/tables.less
--rw-r--r--   0 runner     (501) staff       (20)     7812 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/theme.less
--rw-r--r--   0 runner     (501) staff       (20)      753 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/thumbnails.less
--rw-r--r--   0 runner     (501) staff       (20)     2937 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/tooltip.less
--rw-r--r--   0 runner     (501) staff       (20)     5951 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/type.less
--rw-r--r--   0 runner     (501) staff       (20)      747 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/utilities.less
--rw-r--r--   0 runner     (501) staff       (20)    27053 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/variables.less
--rw-r--r--   0 runner     (501) staff       (20)      527 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/wells.less
--rwxr-xr-x   0 runner     (501) staff       (20)     4596 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/build.py
--rw-r--r--   0 runner     (501) staff       (20)     8122 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/conf.py
--rw-r--r--   0 runner     (501) staff       (20)       84 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/contents.rst
--rw-r--r--   0 runner     (501) staff       (20)     1256 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/fmt.less
--rw-r--r--   0 runner     (501) staff       (20)     5441 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    14903 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/python-license.txt
--rw-r--r--   0 runner     (501) staff       (20)    23444 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/syntax.rst
--rw-r--r--   0 runner     (501) staff       (20)     6621 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/doc/usage.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:40.998901 nod-1.8.1/external/nod/logvisor/fmt/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.095635 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/
--rw-r--r--   0 runner     (501) staff       (20)     7467 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/args.h
--rw-r--r--   0 runner     (501) staff       (20)    42436 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)    24125 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/color.h
--rw-r--r--   0 runner     (501) staff       (20)    21510 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/compile.h
--rw-r--r--   0 runner     (501) staff       (20)    98359 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/core.h
--rw-r--r--   0 runner     (501) staff       (20)   103903 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/format-inl.h
--rw-r--r--   0 runner     (501) staff       (20)   103618 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/format.h
--rw-r--r--   0 runner     (501) staff       (20)      100 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/locale.h
--rw-r--r--   0 runner     (501) staff       (20)    15064 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/os.h
--rw-r--r--   0 runner     (501) staff       (20)     5971 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/ostream.h
--rw-r--r--   0 runner     (501) staff       (20)    20439 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/printf.h
--rw-r--r--   0 runner     (501) staff       (20)    14459 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/ranges.h
--rw-r--r--   0 runner     (501) staff       (20)     9231 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/include/fmt/xchar.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.096945 nod-1.8.1/external/nod/logvisor/fmt/src/
--rw-r--r--   0 runner     (501) staff       (20)     2265 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/src/fmt.cc
--rw-r--r--   0 runner     (501) staff       (20)     3008 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/src/format.cc
--rw-r--r--   0 runner     (501) staff       (20)    10842 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/src/os.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.103564 nod-1.8.1/external/nod/logvisor/fmt/support/
--rw-r--r--   0 runner     (501) staff       (20)      299 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/support/Android.mk
--rw-r--r--   0 runner     (501) staff       (20)       34 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/support/AndroidManifest.xml
--rw-r--r--   0 runner     (501) staff       (20)    72324 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/support/C++.sublime-syntax
--rw-r--r--   0 runner     (501) staff       (20)       85 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/support/README
--rw-r--r--   0 runner     (501) staff       (20)      602 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/support/Vagrantfile
--rw-r--r--   0 runner     (501) staff       (20)     1632 2022-08-02 15:12:20.000000 nod-1.8.1/external/nod/logvisor/fmt/support/appveyor-build.py
--rw-r--r--   0 runner     (501) staff       (20)      593 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/appveyor.yml
--rwxr-xr-x   0 runner     (501) staff       (20)     2064 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/build-docs.py
--rw-r--r--   0 runner     (501) staff       (20)     3977 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/build.gradle
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.106248 nod-1.8.1/external/nod/logvisor/fmt/support/cmake/
--rw-r--r--   0 runner     (501) staff       (20)      299 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/cmake/FindSetEnv.cmake
--rw-r--r--   0 runner     (501) staff       (20)      959 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/cmake/JoinPaths.cmake
--rw-r--r--   0 runner     (501) staff       (20)     1908 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/cmake/cxx14.cmake
--rw-r--r--   0 runner     (501) staff       (20)      110 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/cmake/fmt-config.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)      264 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/cmake/fmt.pc.in
--rwxr-xr-x   0 runner     (501) staff       (20)     1590 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/compute-powers.py
--rw-r--r--   0 runner     (501) staff       (20)    19784 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/docopt.py
--rwxr-xr-x   0 runner     (501) staff       (20)    11181 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/manage.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3958 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/rst2md.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.107207 nod-1.8.1/external/nod/logvisor/fmt/support/rtd/
--rw-r--r--   0 runner     (501) staff       (20)      123 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/rtd/conf.py
--rw-r--r--   0 runner     (501) staff       (20)      112 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/rtd/index.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.108160 nod-1.8.1/external/nod/logvisor/fmt/support/rtd/theme/
--rw-r--r--   0 runner     (501) staff       (20)      483 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/rtd/theme/layout.html
--rw-r--r--   0 runner     (501) staff       (20)       24 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/support/rtd/theme/theme.conf
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.123999 nod-1.8.1/external/nod/logvisor/fmt/test/
--rw-r--r--   0 runner     (501) staff       (20)     8888 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.125078 nod-1.8.1/external/nod/logvisor/fmt/test/add-subdirectory-test/
--rw-r--r--   0 runner     (501) staff       (20)      595 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/add-subdirectory-test/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      128 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/add-subdirectory-test/main.cc
--rw-r--r--   0 runner     (501) staff       (20)     4870 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/args-test.cc
--rw-r--r--   0 runner     (501) staff       (20)      852 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/assert-test.cc
--rw-r--r--   0 runner     (501) staff       (20)    15233 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/chrono-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2506 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/color-test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.125536 nod-1.8.1/external/nod/logvisor/fmt/test/compile-error-test/
--rw-r--r--   0 runner     (501) staff       (20)     2382 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/compile-error-test/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    13165 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/compile-test.cc
--rw-r--r--   0 runner     (501) staff       (20)    27324 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/core-test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.126962 nod-1.8.1/external/nod/logvisor/fmt/test/cuda-test/
--rw-r--r--   0 runner     (501) staff       (20)     3364 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/cuda-test/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      418 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/cuda-test/cpp14.cc
--rw-r--r--   0 runner     (501) staff       (20)      905 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/cuda-test/cuda-cpp14.cu
--rw-r--r--   0 runner     (501) staff       (20)     1587 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/enforce-checks-test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.127862 nod-1.8.1/external/nod/logvisor/fmt/test/find-package-test/
--rw-r--r--   0 runner     (501) staff       (20)      590 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/find-package-test/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      133 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/find-package-test/main.cc
--rw-r--r--   0 runner     (501) staff       (20)    33227 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/format
--rw-r--r--   0 runner     (501) staff       (20)    12498 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/format-impl-test.cc
--rw-r--r--   0 runner     (501) staff       (20)    86675 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/format-test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.133032 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/
--rw-r--r--   0 runner     (501) staff       (20)       54 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     1214 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      789 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/README.md
--rwxr-xr-x   0 runner     (501) staff       (20)     2104 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/build.sh
--rw-r--r--   0 runner     (501) staff       (20)     3275 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/chrono-duration.cc
--rw-r--r--   0 runner     (501) staff       (20)     1202 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/float.cc
--rw-r--r--   0 runner     (501) staff       (20)     2403 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/fuzzer-common.h
--rw-r--r--   0 runner     (501) staff       (20)      592 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/main.cc
--rw-r--r--   0 runner     (501) staff       (20)     2224 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/named-arg.cc
--rw-r--r--   0 runner     (501) staff       (20)     2024 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/one-arg.cc
--rw-r--r--   0 runner     (501) staff       (20)     2321 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/two-args.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.134342 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/
--rw-r--r--   0 runner     (501) staff       (20)       68 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/.clang-format
--rw-r--r--   0 runner     (501) staff       (20)     1242 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.136227 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gmock/
--rw-r--r--   0 runner     (501) staff       (20)   454528 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gmock/gmock.h
--rw-r--r--   0 runner     (501) staff       (20)   532560 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gmock-gtest-all.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.138322 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gtest/
--rw-r--r--   0 runner     (501) staff       (20)    10112 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gtest/gtest-spi.h
--rw-r--r--   0 runner     (501) staff       (20)   474089 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gtest/gtest.h
--rw-r--r--   0 runner     (501) staff       (20)    13892 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest-extra-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2037 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest-extra.cc
--rw-r--r--   0 runner     (501) staff       (20)     7599 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/gtest-extra.h
--rw-r--r--   0 runner     (501) staff       (20)      129 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/header-only-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1554 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/mock-allocator.h
--rw-r--r--   0 runner     (501) staff       (20)    17611 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/module-test.cc
--rw-r--r--   0 runner     (501) staff       (20)    15232 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/os-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     8803 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/ostream-test.cc
--rw-r--r--   0 runner     (501) staff       (20)    14738 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/posix-mock-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1655 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/posix-mock.h
--rw-r--r--   0 runner     (501) staff       (20)    20963 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/printf-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     7655 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/ranges-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2796 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/scan-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     6795 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/scan.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.140941 nod-1.8.1/external/nod/logvisor/fmt/test/static-export-test/
--rw-r--r--   0 runner     (501) staff       (20)      813 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/static-export-test/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      142 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/static-export-test/library.cc
--rw-r--r--   0 runner     (501) staff       (20)      114 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/static-export-test/main.cc
--rw-r--r--   0 runner     (501) staff       (20)     5431 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/std-format-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1113 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/test-assert.h
--rw-r--r--   0 runner     (501) staff       (20)     1203 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/test-main.cc
--rw-r--r--   0 runner     (501) staff       (20)     1301 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/unicode-test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1152 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/util.cc
--rw-r--r--   0 runner     (501) staff       (20)     2040 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/util.h
--rw-r--r--   0 runner     (501) staff       (20)    15053 2022-08-02 15:12:21.000000 nod-1.8.1/external/nod/logvisor/fmt/test/xchar-test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.003032 nod-1.8.1/external/nod/logvisor/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.141499 nod-1.8.1/external/nod/logvisor/include/logvisor/
--rw-r--r--   0 runner     (501) staff       (20)     9216 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/logvisor/logvisor.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.144434 nod-1.8.1/external/nod/logvisor/include/nowide/
--rw-r--r--   0 runner     (501) staff       (20)     5663 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/args.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1962 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/config.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5483 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/convert.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.144882 nod-1.8.1/external/nod/logvisor/include/nowide/detail/
--rw-r--r--   0 runner     (501) staff       (20)     3584 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/detail/is_string_container.hpp
--rw-r--r--   0 runner     (501) staff       (20)      533 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/replacement.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7384 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/stackstring.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.145883 nod-1.8.1/external/nod/logvisor/include/nowide/utf/
--rw-r--r--   0 runner     (501) staff       (20)     3543 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/utf/convert.hpp
--rw-r--r--   0 runner     (501) staff       (20)    14598 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/utf/utf.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1058 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/include/nowide/windows.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.146336 nod-1.8.1/external/nod/logvisor/lib/
--rw-r--r--   0 runner     (501) staff       (20)    23497 2022-08-02 15:12:18.000000 nod-1.8.1/external/nod/logvisor/lib/logvisor.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.147811 nod-1.8.1/nod/
--rw-r--r--   0 runner     (501) staff       (20)      225 2022-08-02 15:12:16.000000 nod-1.8.1/nod/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3164 2022-08-02 15:12:16.000000 nod-1.8.1/nod/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)      176 2022-08-02 15:13:40.000000 nod-1.8.1/nod/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.150114 nod-1.8.1/nod.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2196 2022-08-02 15:13:40.000000 nod-1.8.1/nod.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    13197 2022-08-02 15:13:40.000000 nod-1.8.1/nod.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-02 15:13:40.000000 nod-1.8.1/nod.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2022-08-02 15:13:40.000000 nod-1.8.1/nod.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-08-02 15:12:43.000000 nod-1.8.1/nod.egg-info/zip-safe
--rw-r--r--   0 runner     (501) staff       (20)     4236 2022-08-02 15:12:16.000000 nod-1.8.1/nod_wrap.pxd
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.151049 nod-1.8.1/py-nod/
--rw-r--r--   0 runner     (501) staff       (20)     4059 2022-08-02 15:12:16.000000 nod-1.8.1/py-nod/nod_wrap_util.cxx
--rw-r--r--   0 runner     (501) staff       (20)      620 2022-08-02 15:12:16.000000 nod-1.8.1/py-nod/nod_wrap_util.hpp
--rw-r--r--   0 runner     (501) staff       (20)      274 2022-08-02 15:12:16.000000 nod-1.8.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      770 2022-08-02 15:13:41.155767 nod-1.8.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     5191 2022-08-02 15:12:16.000000 nod-1.8.1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.151521 nod-1.8.1/test/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.005527 nod-1.8.1/test/sample_game/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.152298 nod-1.8.1/test/sample_game/files/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-08-02 15:12:16.000000 nod-1.8.1/test/sample_game/files/a.txt
--rw-r--r--   0 runner     (501) staff       (20)        4 2022-08-02 15:12:16.000000 nod-1.8.1/test/sample_game/files/b.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.152753 nod-1.8.1/test/sample_game/files/d/
--rw-r--r--   0 runner     (501) staff       (20)        3 2022-08-02 15:12:16.000000 nod-1.8.1/test/sample_game/files/d/nested.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-08-02 15:13:41.154372 nod-1.8.1/test/sample_game/sys/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-08-02 15:12:16.000000 nod-1.8.1/test/sample_game/sys/apploader.img
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-08-02 15:12:16.000000 nod-1.8.1/test/sample_game/sys/bi2.bin
--rw-r--r--   0 runner     (501) staff       (20)     1088 2022-08-02 15:12:16.000000 nod-1.8.1/test/sample_game/sys/boot.bin
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-08-02 15:12:16.000000 nod-1.8.1/test/sample_game/sys/main.dol
--rw-r--r--   0 runner     (501) staff       (20)     1569 2022-08-02 15:12:16.000000 nod-1.8.1/test/test_packunpack.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.061607 nod-1.9.0/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.866653 nod-1.9.0/.github/
+-rw-r--r--   0 runner     (501) staff       (20)      610 2023-04-09 13:33:36.000000 nod-1.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.867217 nod-1.9.0/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     4556 2023-04-09 13:33:36.000000 nod-1.9.0/.github/workflows/python.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1246 2023-04-09 13:33:36.000000 nod-1.9.0/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-04-09 13:33:36.000000 nod-1.9.0/.gitmodules
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.870050 nod-1.9.0/.idea/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.870587 nod-1.9.0/.idea/markdown-navigator/
+-rw-r--r--   0 runner     (501) staff       (20)      104 2023-04-09 13:33:36.000000 nod-1.9.0/.idea/markdown-navigator/profiles_settings.xml
+-rw-r--r--   0 runner     (501) staff       (20)     4167 2023-04-09 13:33:36.000000 nod-1.9.0/.idea/markdown-navigator.xml
+-rw-r--r--   0 runner     (501) staff       (20)      185 2023-04-09 13:33:36.000000 nod-1.9.0/.idea/misc.xml
+-rw-r--r--   0 runner     (501) staff       (20)      264 2023-04-09 13:33:36.000000 nod-1.9.0/.idea/modules.xml
+-rw-r--r--   0 runner     (501) staff       (20)      317 2023-04-09 13:33:36.000000 nod-1.9.0/.idea/py-nod.iml
+-rw-r--r--   0 runner     (501) staff       (20)      397 2023-04-09 13:33:36.000000 nod-1.9.0/.idea/vcs.xml
+-rw-r--r--   0 runner     (501) staff       (20)      668 2023-04-09 13:33:36.000000 nod-1.9.0/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1087 2023-04-09 13:33:36.000000 nod-1.9.0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-09 13:33:36.000000 nod-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     2177 2023-04-09 13:35:12.061899 nod-1.9.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1421 2023-04-09 13:33:36.000000 nod-1.9.0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     8935 2023-04-09 13:33:36.000000 nod-1.9.0/_nod.pyx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.871455 nod-1.9.0/ci-scripts/
+-rwxr-xr-x   0 runner     (501) staff       (20)      697 2023-04-09 13:33:36.000000 nod-1.9.0/ci-scripts/build.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.847410 nod-1.9.0/external/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.875499 nod-1.9.0/external/nod/
+-rw-r--r--   0 runner     (501) staff       (20)       40 2023-04-09 13:33:40.000000 nod-1.9.0/external/nod/.git
+-rw-r--r--   0 runner     (501) staff       (20)       88 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)       80 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/.gitmodules
+-rw-r--r--   0 runner     (501) staff       (20)     3124 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      101 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/Config.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)     1146 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     2465 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.877183 nod-1.9.0/external/nod/driver/
+-rw-r--r--   0 runner     (501) staff       (20)      365 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/driver/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      390 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/driver/app.manifest
+-rw-r--r--   0 runner     (501) staff       (20)     8833 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/driver/main.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.848126 nod-1.9.0/external/nod/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.883762 nod-1.9.0/external/nod/include/nod/
+-rw-r--r--   0 runner     (501) staff       (20)     1585 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/DirectoryEnumerator.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    14939 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/DiscBase.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1054 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/DiscGCN.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1074 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/DiscWii.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1807 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/IDiscIO.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2320 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/IFileIO.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2778 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/OSUTF.h
+-rw-r--r--   0 runner     (501) staff       (20)     5527 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/Util.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      437 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/aes.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      415 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/nod.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      782 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/include/nod/sha1.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.893445 nod-1.9.0/external/nod/lib/
+-rw-r--r--   0 runner     (501) staff       (20)     1270 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     8070 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/DirectoryEnumerator.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    29883 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/DiscBase.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/DiscGCN.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1759 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/DiscIOISO.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     8939 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/DiscIONFS.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     9130 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/DiscIOWBFS.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    43036 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/DiscWii.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     4533 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/FileIOFILE.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     6852 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/FileIOWin32.cpp
+-rw-r--r--   0 runner     (501) staff       (20)   295791 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/OSUTF.c
+-rw-r--r--   0 runner     (501) staff       (20)     1868 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/Util.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    15260 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/aes.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2398 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/nod.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     8616 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/lib/sha1.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.896316 nod-1.9.0/external/nod/logvisor/
+-rw-r--r--   0 runner     (501) staff       (20)       60 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/.git
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/.gitmodules
+-rw-r--r--   0 runner     (501) staff       (20)     3538 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      111 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/Config.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)     1151 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.901218 nod-1.9.0/external/nod/logvisor/fmt/
+-rw-r--r--   0 runner     (501) staff       (20)      231 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/.clang-format
+-rw-r--r--   0 runner     (501) staff       (20)       75 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/.git
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.901882 nod-1.9.0/external/nod/logvisor/fmt/.github/
+-rw-r--r--   0 runner     (501) staff       (20)      293 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/.github/pull_request_template.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.904049 nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)      591 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/doc.yml
+-rw-r--r--   0 runner     (501) staff       (20)     2282 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/linux.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1051 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/macos.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1782 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/windows.yml
+-rw-r--r--   0 runner     (501) staff       (20)      397 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)    14760 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      710 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/CONTRIBUTING.md
+-rw-r--r--   0 runner     (501) staff       (20)   173916 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/ChangeLog.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1408 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/LICENSE.rst
+-rw-r--r--   0 runner     (501) staff       (20)    19374 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.909890 nod-1.9.0/external/nod/logvisor/fmt/doc/
+-rw-r--r--   0 runner     (501) staff       (20)      569 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.911076 nod-1.9.0/external/nod/logvisor/fmt/doc/_static/
+-rw-r--r--   0 runner     (501) staff       (20)    35951 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/_static/bootstrap.min.js
+-rw-r--r--   0 runner     (501) staff       (20)      540 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/_static/breathe.css
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.913640 nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/
+-rw-r--r--   0 runner     (501) staff       (20)    20335 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner     (501) staff       (20)    62927 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner     (501) staff       (20)    41280 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner     (501) staff       (20)    23320 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.914875 nod-1.9.0/external/nod/logvisor/fmt/doc/_templates/
+-rw-r--r--   0 runner     (501) staff       (20)     5155 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/_templates/layout.html
+-rw-r--r--   0 runner     (501) staff       (20)     1938 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/_templates/search.html
+-rw-r--r--   0 runner     (501) staff       (20)    17099 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/api.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.916570 nod-1.9.0/external/nod/logvisor/fmt/doc/basic-bootstrap/
+-rw-r--r--   0 runner     (501) staff       (20)      141 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/basic-bootstrap/README
+-rw-r--r--   0 runner     (501) staff       (20)     7570 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/basic-bootstrap/layout.html
+-rw-r--r--   0 runner     (501) staff       (20)       24 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/basic-bootstrap/theme.conf
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.941700 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/
+-rw-r--r--   0 runner     (501) staff       (20)     1518 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/alerts.less
+-rw-r--r--   0 runner     (501) staff       (20)     1201 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/badges.less
+-rw-r--r--   0 runner     (501) staff       (20)     1121 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/bootstrap.less
+-rw-r--r--   0 runner     (501) staff       (20)      594 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/breadcrumbs.less
+-rw-r--r--   0 runner     (501) staff       (20)     5659 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/button-groups.less
+-rw-r--r--   0 runner     (501) staff       (20)     3565 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/buttons.less
+-rw-r--r--   0 runner     (501) staff       (20)     5405 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/carousel.less
+-rw-r--r--   0 runner     (501) staff       (20)      764 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/close.less
+-rw-r--r--   0 runner     (501) staff       (20)     1401 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/code.less
+-rw-r--r--   0 runner     (501) staff       (20)      666 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/component-animations.less
+-rw-r--r--   0 runner     (501) staff       (20)     4764 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/dropdowns.less
+-rw-r--r--   0 runner     (501) staff       (20)    14935 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/forms.less
+-rw-r--r--   0 runner     (501) staff       (20)    19803 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/glyphicons.less
+-rw-r--r--   0 runner     (501) staff       (20)     1390 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/grid.less
+-rw-r--r--   0 runner     (501) staff       (20)     4215 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/input-groups.less
+-rw-r--r--   0 runner     (501) staff       (20)      993 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/jumbotron.less
+-rw-r--r--   0 runner     (501) staff       (20)     1079 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/labels.less
+-rw-r--r--   0 runner     (501) staff       (20)     3022 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/list-group.less
+-rw-r--r--   0 runner     (501) staff       (20)      780 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/media.less
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.961964 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/
+-rw-r--r--   0 runner     (501) staff       (20)      257 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/alerts.less
+-rw-r--r--   0 runner     (501) staff       (20)      139 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/background-variant.less
+-rw-r--r--   0 runner     (501) staff       (20)      468 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/border-radius.less
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/buttons.less
+-rw-r--r--   0 runner     (501) staff       (20)      120 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/center-block.less
+-rw-r--r--   0 runner     (501) staff       (20)      605 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/clearfix.less
+-rw-r--r--   0 runner     (501) staff       (20)     2641 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/forms.less
+-rw-r--r--   0 runner     (501) staff       (20)     4388 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/gradients.less
+-rw-r--r--   0 runner     (501) staff       (20)     2784 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/grid-framework.less
+-rw-r--r--   0 runner     (501) staff       (20)     3094 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/grid.less
+-rw-r--r--   0 runner     (501) staff       (20)      579 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/hide-text.less
+-rw-r--r--   0 runner     (501) staff       (20)     1062 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/image.less
+-rw-r--r--   0 runner     (501) staff       (20)      161 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/labels.less
+-rw-r--r--   0 runner     (501) staff       (20)      533 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/list-group.less
+-rw-r--r--   0 runner     (501) staff       (20)      232 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/nav-divider.less
+-rw-r--r--   0 runner     (501) staff       (20)      364 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/nav-vertical-align.less
+-rw-r--r--   0 runner     (501) staff       (20)      148 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/opacity.less
+-rw-r--r--   0 runner     (501) staff       (20)      438 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/pagination.less
+-rw-r--r--   0 runner     (501) staff       (20)      537 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/panels.less
+-rw-r--r--   0 runner     (501) staff       (20)      191 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/progress-bar.less
+-rw-r--r--   0 runner     (501) staff       (20)      248 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/reset-filter.less
+-rw-r--r--   0 runner     (501) staff       (20)      196 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/resize.less
+-rw-r--r--   0 runner     (501) staff       (20)      343 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/responsive-visibility.less
+-rw-r--r--   0 runner     (501) staff       (20)      127 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/size.less
+-rw-r--r--   0 runner     (501) staff       (20)      159 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/tab-focus.less
+-rw-r--r--   0 runner     (501) staff       (20)      700 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/table-row.less
+-rw-r--r--   0 runner     (501) staff       (20)      116 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/text-emphasis.less
+-rw-r--r--   0 runner     (501) staff       (20)      162 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/text-overflow.less
+-rw-r--r--   0 runner     (501) staff       (20)     6650 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/vendor-prefixes.less
+-rw-r--r--   0 runner     (501) staff       (20)     1102 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins.less
+-rw-r--r--   0 runner     (501) staff       (20)     3565 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/modals.less
+-rw-r--r--   0 runner     (501) staff       (20)    14634 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/navbar.less
+-rw-r--r--   0 runner     (501) staff       (20)     4930 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/navs.less
+-rw-r--r--   0 runner     (501) staff       (20)     7650 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/normalize.less
+-rw-r--r--   0 runner     (501) staff       (20)      861 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/pager.less
+-rw-r--r--   0 runner     (501) staff       (20)     2001 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/pagination.less
+-rw-r--r--   0 runner     (501) staff       (20)     6151 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/panels.less
+-rw-r--r--   0 runner     (501) staff       (20)     3509 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/popovers.less
+-rw-r--r--   0 runner     (501) staff       (20)     2133 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/print.less
+-rw-r--r--   0 runner     (501) staff       (20)     1925 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/progress-bars.less
+-rw-r--r--   0 runner     (501) staff       (20)      546 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/responsive-embed.less
+-rw-r--r--   0 runner     (501) staff       (20)     4262 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/responsive-utilities.less
+-rw-r--r--   0 runner     (501) staff       (20)     3122 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/scaffolding.less
+-rw-r--r--   0 runner     (501) staff       (20)     4612 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/tables.less
+-rw-r--r--   0 runner     (501) staff       (20)     7812 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/theme.less
+-rw-r--r--   0 runner     (501) staff       (20)      753 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/thumbnails.less
+-rw-r--r--   0 runner     (501) staff       (20)     2937 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/tooltip.less
+-rw-r--r--   0 runner     (501) staff       (20)     5951 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/type.less
+-rw-r--r--   0 runner     (501) staff       (20)      747 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/utilities.less
+-rw-r--r--   0 runner     (501) staff       (20)    27053 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/variables.less
+-rw-r--r--   0 runner     (501) staff       (20)      527 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/wells.less
+-rwxr-xr-x   0 runner     (501) staff       (20)     4596 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/build.py
+-rw-r--r--   0 runner     (501) staff       (20)     8122 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/conf.py
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/contents.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1256 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/fmt.less
+-rw-r--r--   0 runner     (501) staff       (20)     5441 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)    14903 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/python-license.txt
+-rw-r--r--   0 runner     (501) staff       (20)    23444 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/syntax.rst
+-rw-r--r--   0 runner     (501) staff       (20)     6621 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/doc/usage.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.852104 nod-1.9.0/external/nod/logvisor/fmt/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.972164 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/
+-rw-r--r--   0 runner     (501) staff       (20)     7467 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/args.h
+-rw-r--r--   0 runner     (501) staff       (20)    42436 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/chrono.h
+-rw-r--r--   0 runner     (501) staff       (20)    24125 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/color.h
+-rw-r--r--   0 runner     (501) staff       (20)    21510 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/compile.h
+-rw-r--r--   0 runner     (501) staff       (20)    98359 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/core.h
+-rw-r--r--   0 runner     (501) staff       (20)   103903 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/format-inl.h
+-rw-r--r--   0 runner     (501) staff       (20)   103618 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/format.h
+-rw-r--r--   0 runner     (501) staff       (20)      100 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/locale.h
+-rw-r--r--   0 runner     (501) staff       (20)    15064 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/os.h
+-rw-r--r--   0 runner     (501) staff       (20)     5971 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/ostream.h
+-rw-r--r--   0 runner     (501) staff       (20)    20439 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/printf.h
+-rw-r--r--   0 runner     (501) staff       (20)    14459 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/ranges.h
+-rw-r--r--   0 runner     (501) staff       (20)     9231 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/include/fmt/xchar.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.974083 nod-1.9.0/external/nod/logvisor/fmt/src/
+-rw-r--r--   0 runner     (501) staff       (20)     2265 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/src/fmt.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3008 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/src/format.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10842 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/src/os.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.982832 nod-1.9.0/external/nod/logvisor/fmt/support/
+-rw-r--r--   0 runner     (501) staff       (20)      299 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/Android.mk
+-rw-r--r--   0 runner     (501) staff       (20)       34 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/AndroidManifest.xml
+-rw-r--r--   0 runner     (501) staff       (20)    72324 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/C++.sublime-syntax
+-rw-r--r--   0 runner     (501) staff       (20)       85 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/README
+-rw-r--r--   0 runner     (501) staff       (20)      602 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/Vagrantfile
+-rw-r--r--   0 runner     (501) staff       (20)     1632 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/appveyor-build.py
+-rw-r--r--   0 runner     (501) staff       (20)      593 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/appveyor.yml
+-rwxr-xr-x   0 runner     (501) staff       (20)     2064 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/build-docs.py
+-rw-r--r--   0 runner     (501) staff       (20)     3977 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/build.gradle
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.986343 nod-1.9.0/external/nod/logvisor/fmt/support/cmake/
+-rw-r--r--   0 runner     (501) staff       (20)      299 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/cmake/FindSetEnv.cmake
+-rw-r--r--   0 runner     (501) staff       (20)      959 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/cmake/JoinPaths.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/cmake/cxx14.cmake
+-rw-r--r--   0 runner     (501) staff       (20)      110 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/cmake/fmt-config.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)      264 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/cmake/fmt.pc.in
+-rwxr-xr-x   0 runner     (501) staff       (20)     1590 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/compute-powers.py
+-rw-r--r--   0 runner     (501) staff       (20)    19784 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/docopt.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    11181 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/manage.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3958 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/rst2md.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.987404 nod-1.9.0/external/nod/logvisor/fmt/support/rtd/
+-rw-r--r--   0 runner     (501) staff       (20)      123 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/rtd/conf.py
+-rw-r--r--   0 runner     (501) staff       (20)      112 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/rtd/index.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.988631 nod-1.9.0/external/nod/logvisor/fmt/support/rtd/theme/
+-rw-r--r--   0 runner     (501) staff       (20)      483 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/rtd/theme/layout.html
+-rw-r--r--   0 runner     (501) staff       (20)       24 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/support/rtd/theme/theme.conf
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.012347 nod-1.9.0/external/nod/logvisor/fmt/test/
+-rw-r--r--   0 runner     (501) staff       (20)     8888 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.014736 nod-1.9.0/external/nod/logvisor/fmt/test/add-subdirectory-test/
+-rw-r--r--   0 runner     (501) staff       (20)      595 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/add-subdirectory-test/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      128 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/add-subdirectory-test/main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4870 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/args-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      852 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/assert-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    15233 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/chrono-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2506 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/color-test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.015488 nod-1.9.0/external/nod/logvisor/fmt/test/compile-error-test/
+-rw-r--r--   0 runner     (501) staff       (20)     2382 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/compile-error-test/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    13165 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/compile-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    27324 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/core-test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.018257 nod-1.9.0/external/nod/logvisor/fmt/test/cuda-test/
+-rw-r--r--   0 runner     (501) staff       (20)     3364 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/cuda-test/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      418 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/cuda-test/cpp14.cc
+-rw-r--r--   0 runner     (501) staff       (20)      905 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/cuda-test/cuda-cpp14.cu
+-rw-r--r--   0 runner     (501) staff       (20)     1587 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/enforce-checks-test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.019998 nod-1.9.0/external/nod/logvisor/fmt/test/find-package-test/
+-rw-r--r--   0 runner     (501) staff       (20)      590 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/find-package-test/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      133 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/find-package-test/main.cc
+-rw-r--r--   0 runner     (501) staff       (20)    33227 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/format
+-rw-r--r--   0 runner     (501) staff       (20)    12498 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/format-impl-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    86675 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/format-test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.030054 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/
+-rw-r--r--   0 runner     (501) staff       (20)       54 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)     1214 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      789 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/README.md
+-rwxr-xr-x   0 runner     (501) staff       (20)     2104 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/build.sh
+-rw-r--r--   0 runner     (501) staff       (20)     3275 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/chrono-duration.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1202 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/float.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2403 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/fuzzer-common.h
+-rw-r--r--   0 runner     (501) staff       (20)      592 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2224 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/named-arg.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2024 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/one-arg.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2321 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/two-args.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.032913 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/
+-rw-r--r--   0 runner     (501) staff       (20)       68 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/.clang-format
+-rw-r--r--   0 runner     (501) staff       (20)     1242 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.035084 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gmock/
+-rw-r--r--   0 runner     (501) staff       (20)   454528 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gmock/gmock.h
+-rw-r--r--   0 runner     (501) staff       (20)   532560 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gmock-gtest-all.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.038168 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gtest/
+-rw-r--r--   0 runner     (501) staff       (20)    10112 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gtest/gtest-spi.h
+-rw-r--r--   0 runner     (501) staff       (20)   474089 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gtest/gtest.h
+-rw-r--r--   0 runner     (501) staff       (20)    13892 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest-extra-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2037 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest-extra.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7599 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/gtest-extra.h
+-rw-r--r--   0 runner     (501) staff       (20)      129 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/header-only-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1554 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/mock-allocator.h
+-rw-r--r--   0 runner     (501) staff       (20)    17611 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/module-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    15232 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/os-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8803 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/ostream-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14738 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/posix-mock-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/posix-mock.h
+-rw-r--r--   0 runner     (501) staff       (20)    20963 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/printf-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7655 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/ranges-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2796 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/scan-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6795 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/scan.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.041383 nod-1.9.0/external/nod/logvisor/fmt/test/static-export-test/
+-rw-r--r--   0 runner     (501) staff       (20)      813 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/static-export-test/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      142 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/static-export-test/library.cc
+-rw-r--r--   0 runner     (501) staff       (20)      114 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/static-export-test/main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5431 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/std-format-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1113 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/test-assert.h
+-rw-r--r--   0 runner     (501) staff       (20)     1203 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/test-main.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1301 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/unicode-test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1152 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/util.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2040 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/util.h
+-rw-r--r--   0 runner     (501) staff       (20)    15053 2023-04-09 13:33:45.000000 nod-1.9.0/external/nod/logvisor/fmt/test/xchar-test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.856977 nod-1.9.0/external/nod/logvisor/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.042174 nod-1.9.0/external/nod/logvisor/include/logvisor/
+-rw-r--r--   0 runner     (501) staff       (20)     9216 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/logvisor/logvisor.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.046389 nod-1.9.0/external/nod/logvisor/include/nowide/
+-rw-r--r--   0 runner     (501) staff       (20)     5663 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/args.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1962 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/config.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5483 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/convert.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.046963 nod-1.9.0/external/nod/logvisor/include/nowide/detail/
+-rw-r--r--   0 runner     (501) staff       (20)     3584 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/detail/is_string_container.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      533 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/replacement.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     7384 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/stackstring.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.048407 nod-1.9.0/external/nod/logvisor/include/nowide/utf/
+-rw-r--r--   0 runner     (501) staff       (20)     3543 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/utf/convert.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    14598 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/utf/utf.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1058 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/include/nowide/windows.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.049109 nod-1.9.0/external/nod/logvisor/lib/
+-rw-r--r--   0 runner     (501) staff       (20)    23572 2023-04-09 13:33:41.000000 nod-1.9.0/external/nod/logvisor/lib/logvisor.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.051783 nod-1.9.0/nod/
+-rw-r--r--   0 runner     (501) staff       (20)      424 2023-04-09 13:33:36.000000 nod-1.9.0/nod/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3164 2023-04-09 13:33:36.000000 nod-1.9.0/nod/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)      477 2023-04-09 13:33:36.000000 nod-1.9.0/nod/types.py
+-rw-r--r--   0 runner     (501) staff       (20)      160 2023-04-09 13:35:11.000000 nod-1.9.0/nod/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.054996 nod-1.9.0/nod.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2177 2023-04-09 13:35:11.000000 nod-1.9.0/nod.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    13301 2023-04-09 13:35:11.000000 nod-1.9.0/nod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-09 13:35:11.000000 nod-1.9.0/nod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-04-09 13:35:11.000000 nod-1.9.0/nod.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-09 13:34:06.000000 nod-1.9.0/nod.egg-info/zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)     4142 2023-04-09 13:33:36.000000 nod-1.9.0/nod_wrap.pxd
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.056426 nod-1.9.0/py-nod/
+-rw-r--r--   0 runner     (501) staff       (20)     4183 2023-04-09 13:33:36.000000 nod-1.9.0/py-nod/nod_wrap_util.cxx
+-rw-r--r--   0 runner     (501) staff       (20)      532 2023-04-09 13:33:36.000000 nod-1.9.0/py-nod/nod_wrap_util.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      266 2023-04-09 13:33:36.000000 nod-1.9.0/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      770 2023-04-09 13:35:12.063005 nod-1.9.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     5177 2023-04-09 13:33:36.000000 nod-1.9.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.057162 nod-1.9.0/test/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:11.859956 nod-1.9.0/test/sample_game/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.058264 nod-1.9.0/test/sample_game/files/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-09 13:33:36.000000 nod-1.9.0/test/sample_game/files/a.txt
+-rw-r--r--   0 runner     (501) staff       (20)        4 2023-04-09 13:33:36.000000 nod-1.9.0/test/sample_game/files/b.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.058989 nod-1.9.0/test/sample_game/files/d/
+-rw-r--r--   0 runner     (501) staff       (20)        3 2023-04-09 13:33:36.000000 nod-1.9.0/test/sample_game/files/d/nested.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-09 13:35:12.061257 nod-1.9.0/test/sample_game/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-09 13:33:36.000000 nod-1.9.0/test/sample_game/sys/apploader.img
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-09 13:33:36.000000 nod-1.9.0/test/sample_game/sys/bi2.bin
+-rw-r--r--   0 runner     (501) staff       (20)     1088 2023-04-09 13:33:36.000000 nod-1.9.0/test/sample_game/sys/boot.bin
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-09 13:33:36.000000 nod-1.9.0/test/sample_game/sys/main.dol
+-rw-r--r--   0 runner     (501) staff       (20)     2250 2023-04-09 13:33:36.000000 nod-1.9.0/test/test_packunpack.py
```

### Comparing `nod-1.8.1/.github/dependabot.yml` & `nod-1.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/.github/workflows/python.yml` & `nod-1.9.0/.github/workflows/python.yml`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
           - 'macos-latest'
           - 'windows-latest'
         python:
           - '3.7'
           - '3.8'
           - '3.9'
           - '3.10'
-          - '3.11-dev'
+          - '3.11'
 
     runs-on: ${{ matrix.os }}
     name: Wheel for ${{ matrix.os }} (${{ matrix.python }})
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
@@ -107,21 +107,21 @@
     name: ${{ matrix.os.name }} - Test Python ${{ matrix.python.version }}
     strategy:
       fail-fast: false
       matrix:
         os:
           - {name: 'macOS', image: 'macos-latest', wheel: 'macosx_*'}
           - {name: 'Windows', image: 'windows-latest', wheel: 'win_amd64'}
-          - {name: 'Linux', image: 'ubuntu-latest', wheel: 'manylinux_2_17_x86_64.manylinux2014_x86_64'}
+          - {name: 'Linux', image: 'ubuntu-latest', wheel: 'manylinux2014_x86_64'}
         python:
           - {version: '3.7', wheel: 'cp37-cp37m'}
           - {version: '3.8', wheel: 'cp38-cp38'}
           - {version: '3.9', wheel: 'cp39-cp39'}
           - {version: '3.10', wheel: 'cp310-cp310'}
-          - {version: '3.11-dev', wheel: 'cp311-cp311'}
+          - {version: '3.11', wheel: 'cp311-cp311'}
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
@@ -129,20 +129,20 @@
           python-version: ${{ matrix.python.version }}
 
       - name: Download all the dists
         uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
-            
+
       - name: Install Python packages
         run: python -m pip install --upgrade pip pytest
 
       - name: install built wheel
-        run: python -m pip install dist/*-${{ matrix.python.wheel }}-${{ matrix.os.wheel }}.whl
+        run: python -m pip install dist/*-${{ matrix.python.wheel }}-*${{ matrix.os.wheel }}.whl
         shell: bash
 
       - name: test
         run: python -m pytest
         working-directory: test
 
   pypi:
@@ -155,17 +155,17 @@
         uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
 
       - name: Publish 📦 to TestPyPI
         if: ${{ github.ref == 'refs/heads/main' }}
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.testpypi_password }}
           repository_url: https://test.pypi.org/legacy/
       
       - name: Publish 📦 to PyPI
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.pypi_password }}
```

### Comparing `nod-1.8.1/.gitignore` & `nod-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/.idea/markdown-navigator.xml` & `nod-1.9.0/.idea/markdown-navigator.xml`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/CMakeLists.txt` & `nod-1.9.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/LICENSE` & `nod-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/PKG-INFO` & `nod-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: nod
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python bindings for the nod library.
 Home-page: https://github.com/henriquegemignani/py-nod
 Author: Henrique Gemignani
 License: License :: OSI Approved :: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -64,8 +63,7 @@
 try:
     disc_builder.build_from_directory("dir_out")    
 except RuntimeError as e:
     raise Exception("Failure building the image: {}".format(e))
 
 
 ```
-
```

### Comparing `nod-1.8.1/README.md` & `nod-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/_nod.pyx` & `nod-1.9.0/_nod.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     DiscBuilderGCN as c_DiscBuilderGCN,
     createFProgressFunction,
     Node,
     EBuildResult,
     EBuildResult_Success,
     EBuildResult_Failed,
     EBuildResult_DiskFull,
-    registerLogvisorToExceptionConverter,
-    removeLogvisorToExceptionConverter,
     _handleNativeException,
     checkException,
 )
 
+import nod.types
+
 
 cdef string _str_to_string(str path):
     return path.encode("utf-8")
 
 
 cdef str _view_to_str(c_string_view str_view):
     return PyBytes_FromStringAndSize(str_view.data(), str_view.size()).decode("utf-8")
@@ -53,44 +53,36 @@
     callback(a.decode("utf-8"), progress)
 
 
 cdef void invoke_fprogress_function(object callback, float totalProg, const string& fileName, size_t fileBytesXfered) except *:
     callback(totalProg, fileName.decode("utf-8"), fileBytesXfered)
 
 
-@contextmanager
-def _log_exception_handler():
-    registerLogvisorToExceptionConverter()
-    yield
-    removeLogvisorToExceptionConverter()
-
-
-cdef class DolHeader:
-    @staticmethod
-    cdef create(const c_Header& h):
-        self = DolHeader()
-        self.game_id = PyBytes_FromStringAndSize(h.m_gameID, 6)
-        self.disc_num = h.m_discNum
-        self.disc_version = h.m_discVersion
-        self.audio_streaming = h.m_audioStreaming
-        self.stream_buf_sz = h.m_streamBufSz
-        self.wii_magic = h.m_wiiMagic
-        self.gcn_magic = h.m_gcnMagic
-        self.game_title = PyBytes_FromStringAndSize(h.m_gameTitle, 64)
-        self.disable_hash_verification = h.m_disableHashVerification
-        self.disable_disc_enc = h.m_disableDiscEnc
-        self.debug_mon_off = h.m_debugMonOff
-        self.debug_load_addr = h.m_debugLoadAddr
-        self.dol_off = h.m_dolOff
-        self.fst_off = h.m_fstOff
-        self.fst_sz = h.m_fstSz
-        self.fst_max_sz = h.m_fstMaxSz
-        self.fst_memory_address = h.m_fstMemoryAddress
-        self.user_position = h.m_userPosition
-        self.user_sz = h.m_userSz
+cdef _create_dol_header(const c_Header& h):
+    return nod.types.DolHeader(
+        game_id = PyBytes_FromStringAndSize(h.m_gameID, 6),
+        disc_num = h.m_discNum,
+        disc_version = h.m_discVersion,
+        audio_streaming = h.m_audioStreaming,
+        stream_buf_sz = h.m_streamBufSz,
+        wii_magic = h.m_wiiMagic,
+        gcn_magic = h.m_gcnMagic,
+        game_title = PyBytes_FromStringAndSize(h.m_gameTitle, 64),
+        disable_hash_verification = h.m_disableHashVerification,
+        disable_disc_enc = h.m_disableDiscEnc,
+        debug_mon_off = h.m_debugMonOff,
+        debug_load_addr = h.m_debugLoadAddr,
+        dol_off = h.m_dolOff,
+        fst_off = h.m_fstOff,
+        fst_sz = h.m_fstSz,
+        fst_max_sz = h.m_fstMaxSz,
+        fst_memory_address = h.m_fstMemoryAddress,
+        user_position = h.m_userPosition,
+        user_sz = h.m_userSz,
+    )
 
 
 cdef class ExtractionContext:
     cdef c_ExtractionContext c_context
 
     def __cinit__(self):
         self.c_context = c_ExtractionContext()
@@ -173,15 +165,15 @@
     if node.getKind() == Kind_File:
         result.append(prefix + name)
     else:
         newPrefix = prefix
         if name:
             newPrefix = prefix + name + "/"
         f = node.begin()
-        while f.value() != node.end():
+        while dereference(f) != node.end():
             _files_for(dereference(dereference(f)), newPrefix, result)
             preincrement(dereference(f))
 
 
 cdef class Partition:
     cdef c_DiscBase.IPartition* c_partition
     cdef object discParent
@@ -194,28 +186,27 @@
         partition = Partition(parent)
         partition.c_partition = c_partition
         return partition
 
     def get_dol(self) -> bytes:
         return _getDol(self.c_partition)
 
-    def get_header(self):
-        return DolHeader.create(self.c_partition.getHeader())
+    def get_header(self) -> nod.types.DolHeader:
+        return _create_dol_header(self.c_partition.getHeader())
 
     def extract_to_directory(self, path: str, context: ExtractionContext) -> None:
         def work():
             cdef c_bool extraction_successful = False
             cdef string native_path = _str_to_string(path)
 
-            with _log_exception_handler():
-                with nogil:
-                    extraction_successful = self.c_partition.extractToDirectory(
-                        native_path,
-                        context.c_context
-                    )
+            with nogil:
+                extraction_successful = self.c_partition.extractToDirectory(
+                    native_path,
+                    context.c_context
+                )
             if not extraction_successful:
                 raise RuntimeError("Unable to extract")
         return _handleNativeException(work)
 
     def files(self) -> List[str]:
         cdef Node* node = &self.c_partition.getFSTRoot()
         result = []
@@ -225,15 +216,15 @@
 
     def read_file(self, path: str, offset: int = 0) -> PartReadStream:
         cdef Node* node = &self.c_partition.getFSTRoot()
         cdef c_optional[Node.DirectoryIterator] f
 
         for part in path.split("/"):
             f = node.find(_str_to_string(part))
-            if f.value() != node.end():
+            if dereference(f) != node.end():
                 node = &dereference(dereference(f))
             else:
                 raise FileNotFoundError(f"File {part} not found in '{_view_to_str(node.getName())}'")
             
         return PartReadStream.create(
             dereference(dereference(f)).beginReadStream(offset),
             dereference(dereference(f)).size(),
@@ -263,17 +254,16 @@
 
     def __dealloc__(self):
         del self.c_builder
 
     def build_from_directory(self, directory_in: os.PathLike) -> None:
         def work():
             cdef string native_path = _str_to_string(os.fspath(directory_in))
-            with _log_exception_handler():
-                with nogil:
-                    self.c_builder.buildFromDirectory(native_path)
+            with nogil:
+                self.c_builder.buildFromDirectory(native_path)
         return _handleNativeException(work)
 
     @staticmethod
     def calculate_total_size_required(directory_in: os.PathLike) -> Optional[int]:
         cdef string native_path = _str_to_string(os.fspath(directory_in))
 
         cdef c_optional[uint64_t] size
@@ -281,20 +271,19 @@
             size = c_DiscBuilderGCN.CalculateTotalSizeRequired(native_path)
         
         if size:
             return cython.operator.dereference(size)
         return None
 
 
-def open_disc_from_image(path: os.PathLike) -> Optional[Tuple[DiscBase, bool]]:
+def open_disc_from_image(path: os.PathLike) -> Tuple[DiscBase, bool]:
     def work():
         disc = DiscBase()
         cdef string native_path = _str_to_string(os.fspath(path))
         cdef c_bool is_wii = True
 
-        with _log_exception_handler():
-            with nogil:
-                disc.c_disc = OpenDiscFromImage(native_path, is_wii)
-            checkException()
-            return disc, is_wii
+        with nogil:
+            disc.c_disc = OpenDiscFromImage(native_path, is_wii)
+        checkException()
+        return disc, is_wii
 
     return _handleNativeException(work)
```

### Comparing `nod-1.8.1/ci-scripts/build.sh` & `nod-1.9.0/ci-scripts/build.sh`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/CMakeLists.txt` & `nod-1.9.0/external/nod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/LICENSE` & `nod-1.9.0/external/nod/LICENSE`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/README.md` & `nod-1.9.0/external/nod/README.md`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/driver/main.cpp` & `nod-1.9.0/external/nod/driver/main.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/DirectoryEnumerator.hpp` & `nod-1.9.0/external/nod/include/nod/DirectoryEnumerator.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/DiscBase.hpp` & `nod-1.9.0/external/nod/include/nod/DiscBase.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/DiscGCN.hpp` & `nod-1.9.0/external/nod/include/nod/DiscGCN.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/DiscWii.hpp` & `nod-1.9.0/external/nod/include/nod/DiscWii.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/IDiscIO.hpp` & `nod-1.9.0/external/nod/include/nod/IDiscIO.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/IFileIO.hpp` & `nod-1.9.0/external/nod/include/nod/IFileIO.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/OSUTF.h` & `nod-1.9.0/external/nod/include/nod/OSUTF.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/Util.hpp` & `nod-1.9.0/external/nod/include/nod/Util.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/include/nod/sha1.h` & `nod-1.9.0/external/nod/include/nod/sha1.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/CMakeLists.txt` & `nod-1.9.0/external/nod/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/DirectoryEnumerator.cpp` & `nod-1.9.0/external/nod/lib/DirectoryEnumerator.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/DiscBase.cpp` & `nod-1.9.0/external/nod/lib/DiscBase.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/DiscGCN.cpp` & `nod-1.9.0/external/nod/lib/DiscGCN.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/DiscIOISO.cpp` & `nod-1.9.0/external/nod/lib/DiscIOISO.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/DiscIONFS.cpp` & `nod-1.9.0/external/nod/lib/DiscIONFS.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/DiscIOWBFS.cpp` & `nod-1.9.0/external/nod/lib/DiscIOWBFS.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/DiscWii.cpp` & `nod-1.9.0/external/nod/lib/DiscWii.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/FileIOFILE.cpp` & `nod-1.9.0/external/nod/lib/FileIOFILE.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/FileIOWin32.cpp` & `nod-1.9.0/external/nod/lib/FileIOWin32.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/OSUTF.c` & `nod-1.9.0/external/nod/lib/OSUTF.c`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/Util.cpp` & `nod-1.9.0/external/nod/lib/Util.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/aes.cpp` & `nod-1.9.0/external/nod/lib/aes.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/nod.cpp` & `nod-1.9.0/external/nod/lib/nod.cpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/lib/sha1.c` & `nod-1.9.0/external/nod/lib/sha1.c`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/LICENSE` & `nod-1.9.0/external/nod/logvisor/LICENSE`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/doc.yml` & `nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/linux.yml` & `nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/macos.yml` & `nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/.github/workflows/windows.yml` & `nod-1.9.0/external/nod/logvisor/fmt/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/CONTRIBUTING.md` & `nod-1.9.0/external/nod/logvisor/fmt/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/ChangeLog.rst` & `nod-1.9.0/external/nod/logvisor/fmt/ChangeLog.rst`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/LICENSE.rst` & `nod-1.9.0/external/nod/logvisor/fmt/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/README.rst` & `nod-1.9.0/external/nod/logvisor/fmt/README.rst`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/_static/bootstrap.min.js` & `nod-1.9.0/external/nod/logvisor/fmt/doc/_static/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/_static/breathe.css` & `nod-1.9.0/external/nod/logvisor/fmt/doc/_static/breathe.css`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.eot` & `nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.svg` & `nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.ttf` & `nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.woff` & `nod-1.9.0/external/nod/logvisor/fmt/doc/_static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/_templates/layout.html` & `nod-1.9.0/external/nod/logvisor/fmt/doc/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/_templates/search.html` & `nod-1.9.0/external/nod/logvisor/fmt/doc/_templates/search.html`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/api.rst` & `nod-1.9.0/external/nod/logvisor/fmt/doc/api.rst`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/basic-bootstrap/layout.html` & `nod-1.9.0/external/nod/logvisor/fmt/doc/basic-bootstrap/layout.html`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/alerts.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/alerts.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/badges.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/badges.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/bootstrap.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/bootstrap.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/breadcrumbs.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/breadcrumbs.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/button-groups.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/button-groups.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/buttons.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/buttons.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/carousel.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/carousel.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/close.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/close.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/code.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/code.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/component-animations.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/component-animations.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/dropdowns.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/dropdowns.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/forms.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/forms.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/glyphicons.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/glyphicons.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/grid.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/grid.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/input-groups.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/input-groups.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/jumbotron.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/jumbotron.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/labels.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/labels.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/list-group.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/list-group.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/media.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/media.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/buttons.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/buttons.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/clearfix.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/clearfix.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/forms.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/forms.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/gradients.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/gradients.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/grid-framework.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/grid-framework.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/grid.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/grid.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/hide-text.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/hide-text.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/image.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/image.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/list-group.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/list-group.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/panels.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/panels.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/table-row.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/table-row.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins/vendor-prefixes.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins/vendor-prefixes.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/mixins.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/mixins.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/modals.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/modals.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/navbar.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/navbar.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/navs.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/navs.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/normalize.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/normalize.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/pager.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/pager.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/pagination.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/pagination.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/panels.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/panels.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/popovers.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/popovers.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/print.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/print.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/progress-bars.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/progress-bars.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/responsive-embed.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/responsive-embed.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/responsive-utilities.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/scaffolding.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/scaffolding.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/tables.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/tables.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/theme.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/theme.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/thumbnails.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/thumbnails.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/tooltip.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/tooltip.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/type.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/type.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/utilities.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/utilities.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/variables.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/variables.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/bootstrap/wells.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/bootstrap/wells.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/build.py` & `nod-1.9.0/external/nod/logvisor/fmt/doc/build.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/conf.py` & `nod-1.9.0/external/nod/logvisor/fmt/doc/conf.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/fmt.less` & `nod-1.9.0/external/nod/logvisor/fmt/doc/fmt.less`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/index.rst` & `nod-1.9.0/external/nod/logvisor/fmt/doc/index.rst`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/python-license.txt` & `nod-1.9.0/external/nod/logvisor/fmt/doc/python-license.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/syntax.rst` & `nod-1.9.0/external/nod/logvisor/fmt/doc/syntax.rst`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/doc/usage.rst` & `nod-1.9.0/external/nod/logvisor/fmt/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/args.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/args.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/chrono.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/chrono.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/color.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/color.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/compile.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/compile.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/core.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/core.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/format-inl.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/format-inl.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/format.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/format.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/os.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/os.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/ostream.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/ostream.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/printf.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/printf.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/ranges.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/ranges.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/include/fmt/xchar.h` & `nod-1.9.0/external/nod/logvisor/fmt/include/fmt/xchar.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/src/fmt.cc` & `nod-1.9.0/external/nod/logvisor/fmt/src/fmt.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/src/format.cc` & `nod-1.9.0/external/nod/logvisor/fmt/src/format.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/src/os.cc` & `nod-1.9.0/external/nod/logvisor/fmt/src/os.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/C++.sublime-syntax` & `nod-1.9.0/external/nod/logvisor/fmt/support/C++.sublime-syntax`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/Vagrantfile` & `nod-1.9.0/external/nod/logvisor/fmt/support/Vagrantfile`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/appveyor-build.py` & `nod-1.9.0/external/nod/logvisor/fmt/support/appveyor-build.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/appveyor.yml` & `nod-1.9.0/external/nod/logvisor/fmt/support/appveyor.yml`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/build-docs.py` & `nod-1.9.0/external/nod/logvisor/fmt/support/build-docs.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/build.gradle` & `nod-1.9.0/external/nod/logvisor/fmt/support/build.gradle`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/cmake/JoinPaths.cmake` & `nod-1.9.0/external/nod/logvisor/fmt/support/cmake/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/cmake/cxx14.cmake` & `nod-1.9.0/external/nod/logvisor/fmt/support/cmake/cxx14.cmake`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/compute-powers.py` & `nod-1.9.0/external/nod/logvisor/fmt/support/compute-powers.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/docopt.py` & `nod-1.9.0/external/nod/logvisor/fmt/support/docopt.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/manage.py` & `nod-1.9.0/external/nod/logvisor/fmt/support/manage.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/support/rst2md.py` & `nod-1.9.0/external/nod/logvisor/fmt/support/rst2md.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/add-subdirectory-test/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/test/add-subdirectory-test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/args-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/args-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/assert-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/assert-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/chrono-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/chrono-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/color-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/color-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/compile-error-test/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/test/compile-error-test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/compile-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/compile-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/core-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/core-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/cuda-test/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/test/cuda-test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/cuda-test/cuda-cpp14.cu` & `nod-1.9.0/external/nod/logvisor/fmt/test/cuda-test/cuda-cpp14.cu`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/enforce-checks-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/enforce-checks-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/find-package-test/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/test/find-package-test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/format` & `nod-1.9.0/external/nod/logvisor/fmt/test/format`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/format-impl-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/format-impl-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/format-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/format-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/README.md` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/README.md`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/build.sh` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/build.sh`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/chrono-duration.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/chrono-duration.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/float.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/float.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/fuzzer-common.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/fuzzer-common.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/main.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/main.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/named-arg.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/named-arg.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/one-arg.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/one-arg.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/fuzzing/two-args.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/fuzzing/two-args.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/gtest/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/test/gtest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gmock/gmock.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gmock/gmock.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gmock-gtest-all.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gmock-gtest-all.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gtest/gtest-spi.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gtest/gtest-spi.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/gtest/gtest/gtest.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/gtest/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/gtest-extra-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/gtest-extra-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/gtest-extra.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/gtest-extra.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/gtest-extra.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/gtest-extra.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/mock-allocator.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/mock-allocator.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/module-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/module-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/os-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/os-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/ostream-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/ostream-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/posix-mock-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/posix-mock-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/posix-mock.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/posix-mock.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/printf-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/printf-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/ranges-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/ranges-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/scan-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/scan-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/scan.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/scan.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/static-export-test/CMakeLists.txt` & `nod-1.9.0/external/nod/logvisor/fmt/test/static-export-test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/std-format-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/std-format-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/test-assert.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/test-assert.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/test-main.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/test-main.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/unicode-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/unicode-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/util.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/util.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/util.h` & `nod-1.9.0/external/nod/logvisor/fmt/test/util.h`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/fmt/test/xchar-test.cc` & `nod-1.9.0/external/nod/logvisor/fmt/test/xchar-test.cc`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/logvisor/logvisor.hpp` & `nod-1.9.0/external/nod/logvisor/include/logvisor/logvisor.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/args.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/args.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/config.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/config.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/convert.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/convert.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/detail/is_string_container.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/detail/is_string_container.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/replacement.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/replacement.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/stackstring.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/stackstring.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/utf/convert.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/utf/convert.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/utf/utf.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/utf/utf.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/include/nowide/windows.hpp` & `nod-1.9.0/external/nod/logvisor/include/nowide/windows.hpp`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/external/nod/logvisor/lib/logvisor.cpp` & `nod-1.9.0/external/nod/logvisor/lib/logvisor.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,18 @@
 
 #elif defined(__SWITCH__)
 [[noreturn]] void logvisorAbort() {
   MainLoggers.clear();
   nvExit();
   exit(1);
 }
+#elif defined(EMSCRIPTEN)
+[[noreturn]] void logvisorAbort() {
+  abort();
+}
 #else
 
 void KillProcessTree() {}
 
 #include <execinfo.h>
 [[noreturn]] void logvisorAbort() {
   void* array[128];
```

### Comparing `nod-1.8.1/nod/__main__.py` & `nod-1.9.0/nod/__main__.py`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/nod.egg-info/PKG-INFO` & `nod-1.9.0/nod.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: nod
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python bindings for the nod library.
 Home-page: https://github.com/henriquegemignani/py-nod
 Author: Henrique Gemignani
 License: License :: OSI Approved :: MIT License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -64,8 +63,7 @@
 try:
     disc_builder.build_from_directory("dir_out")    
 except RuntimeError as e:
     raise Exception("Failure building the image: {}".format(e))
 
 
 ```
-
```

### Comparing `nod-1.8.1/nod.egg-info/SOURCES.txt` & `nod-1.9.0/nod.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .gitignore
 .gitmodules
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
-_nod.cpp
 _nod.pyx
 nod_wrap.pxd
 pyproject.toml
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/python.yml
 .idea/markdown-navigator.xml
 .idea/misc.xml
 .idea/modules.xml
 .idea/py-nod.iml
 .idea/vcs.xml
 .idea/markdown-navigator/profiles_settings.xml
+/Users/runner/work/py-nod/py-nod/_nod.cpp
+/Users/runner/work/py-nod/py-nod/py-nod/nod_wrap_util.cxx
 ci-scripts/build.sh
 external/nod/.git
 external/nod/.gitignore
 external/nod/.gitmodules
 external/nod/CMakeLists.txt
 external/nod/Config.cmake.in
 external/nod/LICENSE
@@ -271,14 +272,15 @@
 external/nod/logvisor/include/nowide/windows.hpp
 external/nod/logvisor/include/nowide/detail/is_string_container.hpp
 external/nod/logvisor/include/nowide/utf/convert.hpp
 external/nod/logvisor/include/nowide/utf/utf.hpp
 external/nod/logvisor/lib/logvisor.cpp
 nod/__init__.py
 nod/__main__.py
+nod/types.py
 nod/version.py
 nod.egg-info/PKG-INFO
 nod.egg-info/SOURCES.txt
 nod.egg-info/dependency_links.txt
 nod.egg-info/top_level.txt
 nod.egg-info/zip-safe
 py-nod/nod_wrap_util.cxx
```

### Comparing `nod-1.8.1/nod_wrap.pxd` & `nod-1.9.0/nod_wrap.pxd`

 * *Files 3% similar despite different names*

```diff
@@ -120,11 +120,9 @@
 
 cdef extern from "py-nod/nod_wrap_util.hpp" namespace "nod_wrap":
     function[void(string_view, float)] createProgressCallbackFunction(object, void (*)(object, const string&, float) except *)
     function[void(float, string_view, size_t)] createFProgressFunction(object, void (*)(object, float, const string&, size_t) except *)
 
     object getDol(const IPartition*)
     void doPrint(const IPartition*)
-    void registerLogvisorToExceptionConverter()
-    void removeLogvisorToExceptionConverter()
     object _handleNativeException(object)
     void checkException() except *
```

### Comparing `nod-1.8.1/py-nod/nod_wrap_util.cxx` & `nod-1.9.0/py-nod/nod_wrap_util.cxx`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 class LogvisorToExceptionConverter : public logvisor::ILogger {
 public:
 	LogvisorToExceptionConverter() : ILogger(log_typeid(LogvisorToExceptionConverter)) {}
 
     void report(const char* modName, logvisor::Level severity, fmt::string_view format, fmt::format_args args) override
     {
-		auto state = PyGILState_Ensure();
+        auto state = PyGILState_Ensure();
         auto error_message = fmt::vformat(format, args);
 		PyErr_SetString(PyExc_RuntimeError, error_message.c_str());
-		auto has_err = PyErr_Occurred();
+		PyGILState_Release(state);
     }
 	
     void reportSource(const char* modName, logvisor::Level severity,
                       const char* file, unsigned linenum,
                       fmt::string_view format, fmt::format_args args) override
     {
         // openFile();
@@ -139,15 +139,20 @@
 		currentConverter = nullptr;
 	}
 }
 
 PyObject * _handleNativeException(PyObject * callable) {
 	if (PyErr_Occurred())
 		return NULL;
+
+	registerLogvisorToExceptionConverter();
+	PyObject * result;
 	try {
-		return PyObject_CallFunction(callable, NULL);
+		result = PyObject_CallFunction(callable, NULL);
 	} catch (BreakOutFromNative) {
-		return NULL;
+	    result = NULL;
 	}
+	removeLogvisorToExceptionConverter();
+	return result;
 }
 
 }
```

### Comparing `nod-1.8.1/py-nod/nod_wrap_util.hpp` & `nod-1.9.0/py-nod/nod_wrap_util.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -8,13 +8,11 @@
 
 namespace nod_wrap {
 
 std::function<void(std::string_view, float)> createProgressCallbackFunction(PyObject *, void (*)(PyObject *, const std::string&, float));
 nod::FProgress createFProgressFunction(PyObject *, void (*)(PyObject *, float, const std::string&, size_t));
 
 PyObject * getDol(const nod::IPartition*);
-void registerLogvisorToExceptionConverter();
-void removeLogvisorToExceptionConverter();
 PyObject * _handleNativeException(PyObject *);
 inline void checkException() {}
 
 } // namespace nod_wrap
```

### Comparing `nod-1.8.1/setup.cfg` & `nod-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/setup.py` & `nod-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,48 +43,48 @@
     def build_extension(self, ext):
         cmake_options = ext.cmake_options
         extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
         cmake_args = ['-DCMAKE_ARCHIVE_OUTPUT_DIRECTORY=' + extdir,
                       '-DPYTHON_EXECUTABLE=' + sys.executable,
                       '-DCMAKE_POSITION_INDEPENDENT_CODE=YES']
         library_output_dir = extdir
-        
+
         cfg = 'Debug' if self.debug else 'Release'
         build_args = ['--config', cfg]
-        
+
         if is_windows:
             cmake_args += ['-DCMAKE_ARCHIVE_OUTPUT_DIRECTORY_{}={}'.format(cfg.upper(), extdir)]
             if sys.maxsize > 2 ** 32:
                 cmake_args += ['-A', 'x64']
             build_args += ['--', '/m', '/verbosity:minimal']
             library_name_format = "{}.lib"
         else:
             cmake_args += ['-DCMAKE_BUILD_TYPE=' + cfg]
             build_args += ['--', '-j2']
             library_name_format = "lib{}.a"
-        
+
         env = os.environ.copy()
         env['CXXFLAGS'] = '{} -DVERSION_INFO=\\"{}\\"'.format(env.get('CXXFLAGS', ''),
                                                               self.distribution.get_version())
         if not os.path.exists(self.build_temp):
             os.makedirs(self.build_temp)
-        
+
         subprocess.run(
             ['cmake', cmake_options["dir"]] + cmake_args,
             cwd=self.build_temp,
             env=env,
             check=True
         )
         if self.force:
             subprocess.run(
                 ['cmake', '--build', '.', '--target', 'clean'] + build_args,
                 cwd=self.build_temp,
                 check=True
             )
-        
+
         for target, target_output in cmake_options["targets"].items():
             subprocess.run(
                 ['cmake', '--build', '.', '--target', target] + build_args,
                 cwd=self.build_temp,
                 check=True
             )
             ext.extra_objects.append(
@@ -151,15 +151,15 @@
     create_extension=create_extension,
 )
 
 for ext_module in cythonized_ext_modules:
     ext_module.include_dirs = custom_include_paths
 
 setup(
-    use_scm_version=True,
-    scripts=[
-    ],
+    use_scm_version={
+        "local_scheme": "no-local-version",
+    },
     cmdclass={
         'build_ext': CMakeBuild,
     },
     ext_modules=cythonized_ext_modules,
 )
```

### Comparing `nod-1.8.1/test/sample_game/sys/boot.bin` & `nod-1.9.0/test/sample_game/sys/boot.bin`

 * *Files identical despite different names*

### Comparing `nod-1.8.1/test/test_packunpack.py` & `nod-1.9.0/test/test_packunpack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import hashlib
-import os
 from pathlib import Path
 
 import pytest
 
 import nod
 
 
@@ -24,15 +23,14 @@
     filesystem_root = Path(__file__).parent.joinpath("sample_game")
     image_out = tmp_path_factory.mktemp("iso").joinpath("game.iso")
     disc_builder = nod.DiscBuilderGCN(image_out, fprogress_callback)
     disc_builder.build_from_directory(filesystem_root)
     return image_out
 
 
-
 def test_packunpack(pack_sample_game):
     iso_hash = sha256_checksum(pack_sample_game)
     assert iso_hash == '0d98f9bf2c94051bec6145373c0b2c4baee0b35ccb066eaf354fd5a7b9324816'
 
 
 def test_build_and_check(pack_sample_game):
     result = nod.open_disc_from_image(pack_sample_game)
@@ -53,7 +51,20 @@
     assert f.read(1) == b"3"
     f.seek(1)
     assert f.read(2) == b"23"
 
     f.close()
     with pytest.raises(RuntimeError):
         f.read(1)
+
+
+def test_get_header(pack_sample_game):
+    result: nod.DiscBase = nod.open_disc_from_image(pack_sample_game)[0]
+    data: nod.Partition = result.get_data_partition()
+
+    header: nod.DolHeader = data.get_header()
+    assert header == nod.DolHeader(
+        game_id=b'G2ME0R', disc_num=0, disc_version=0, audio_streaming=1, stream_buf_sz=0, wii_magic=0,
+        gcn_magic=3258163005,
+        game_title=b'Metroid Prime 2: Randomizer - QFHHNLN3'.ljust(64, b'\x00'),
+        disable_hash_verification=0, disable_disc_enc=0, debug_mon_off=0, debug_load_addr=0, dol_off=1459978240,
+        fst_off=9280, fst_sz=96, fst_max_sz=96, fst_memory_address=255680, user_position=1459978176, user_sz=64)
```

