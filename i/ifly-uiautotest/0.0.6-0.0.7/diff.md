# Comparing `tmp/ifly_uiautotest-0.0.6.tar.gz` & `tmp/ifly_uiautotest-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ifly_uiautotest-0.0.6.tar", last modified: Wed Mar 29 12:42:55 2023, max compression
+gzip compressed data, was "dist\ifly_uiautotest-0.0.7.tar", last modified: Sun Apr  9 04:54:41 2023, max compression
```

## Comparing `ifly_uiautotest-0.0.6.tar` & `ifly_uiautotest-0.0.7.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/atomicwrites/
--rw-rw-rw-   0        0        0     6970 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/atomicwrites/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/attr/
--rw-rw-rw-   0        0        0     3602 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/converters.py
--rw-rw-rw-   0        0        0     1915 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/exceptions.py
--rw-rw-rw-   0        0        0     1038 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/filters.py
--rw-rw-rw-   0        0        0     1400 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/setters.py
--rw-rw-rw-   0        0        0    20501 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/validators.py
--rw-rw-rw-   0        0        0     4094 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/_cmp.py
--rw-rw-rw-   0        0        0     5435 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/_compat.py
--rw-rw-rw-   0        0        0      826 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/_config.py
--rw-rw-rw-   0        0        0    14545 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/_funcs.py
--rw-rw-rw-   0        0        0    96087 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/_make.py
--rw-rw-rw-   0        0        0     6059 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/_next_gen.py
--rw-rw-rw-   0        0        0     2121 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/_version_info.py
--rw-rw-rw-   0        0        0     1947 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/attrs/
--rw-rw-rw-   0        0        0       70 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attrs/converters.py
--rw-rw-rw-   0        0        0       70 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attrs/exceptions.py
--rw-rw-rw-   0        0        0       67 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attrs/filters.py
--rw-rw-rw-   0        0        0       67 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attrs/setters.py
--rw-rw-rw-   0        0        0       70 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attrs/validators.py
--rw-rw-rw-   0        0        0     1149 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/attrs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/colorama/
--rw-rw-rw-   0        0        0     2522 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/colorama/ansi.py
--rw-rw-rw-   0        0        0    10830 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/colorama/winterm.py
--rw-rw-rw-   0        0        0      239 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/colorama/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/cookiecutter/
--rw-rw-rw-   0        0        0     5140 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/cli.py
--rw-rw-rw-   0        0        0     4429 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/config.py
--rw-rw-rw-   0        0        0     2297 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/environment.py
--rw-rw-rw-   0        0        0     3927 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/exceptions.py
--rw-rw-rw-   0        0        0     1684 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/extensions.py
--rw-rw-rw-   0        0        0     1034 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/find.py
--rw-rw-rw-   0        0        0    13632 2023-03-29 07:24:45.000000 ifly_uiautotest-0.0.6/cookiecutter/generate.py
--rw-rw-rw-   0        0        0     4168 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/hooks.py
--rw-rw-rw-   0        0        0     1596 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/log.py
--rw-rw-rw-   0        0        0     3698 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/main.py
--rw-rw-rw-   0        0        0     7670 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/prompt.py
--rw-rw-rw-   0        0        0     1567 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/replay.py
--rw-rw-rw-   0        0        0     4272 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/repository.py
--rw-rw-rw-   0        0        0     2734 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/utils.py
--rw-rw-rw-   0        0        0     3890 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/vcs.py
--rw-rw-rw-   0        0        0     4480 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/zipfile.py
--rw-rw-rw-   0        0        0       85 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/__init__.py
--rw-rw-rw-   0        0        0      258 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.6/cookiecutter/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/ifly_autotest/
--rw-rw-rw-   0        0        0     1431 2023-03-29 12:39:44.000000 ifly_uiautotest-0.0.6/ifly_autotest/ifly_autotest.py
--rw-rw-rw-   0        0        0       20 2023-03-28 06:27:23.000000 ifly_uiautotest-0.0.6/ifly_autotest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-29 12:42:52.000000 ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-03-29 12:42:52.000000 ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      599 2023-03-29 12:42:52.000000 ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-03-29 12:42:52.000000 ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/requires.txt
--rw-rw-rw-   0        0        0     4466 2023-03-29 12:42:53.000000 ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      140 2023-03-29 12:42:52.000000 ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/importlib_metadata/
--rw-rw-rw-   0        0        0     1862 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1826 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1154 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     2166 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/importlib_metadata/_text.py
--rw-rw-rw-   0        0        0    30503 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/importlib_metadata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/iniconfig/
--rw-rw-rw-   0        0        0     5225 2023-03-28 06:59:52.000000 ifly_uiautotest-0.0.6/iniconfig/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-01-05 03:23:29.000000 ifly_uiautotest-0.0.6/LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/packaging/
--rw-rw-rw-   0        0        0     8475 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/markers.py
--rw-rw-rw-   0        0        0     4664 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/version.py
--rw-rw-rw-   0        0        0    11488 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/_structures.py
--rw-rw-rw-   0        0        0      661 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/packaging/__init__.py
--rw-rw-rw-   0        0        0      599 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/pluggy/
--rw-rw-rw-   0        0        0     2097 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pluggy/_callers.py
--rw-rw-rw-   0        0        0    11496 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pluggy/_hooks.py
--rw-rw-rw-   0        0        0    14752 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pluggy/_manager.py
--rw-rw-rw-   0        0        0     1535 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pluggy/_result.py
--rw-rw-rw-   0        0        0     1541 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pluggy/_tracing.py
--rw-rw-rw-   0        0        0      142 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pluggy/_version.py
--rw-rw-rw-   0        0        0      489 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pluggy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/py/
--rw-rw-rw-   0        0        0      222 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/test.py
--rw-rw-rw-   0        0        0     4021 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_builtin.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/py/_code/
--rw-rw-rw-   0        0        0     3174 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_code/assertion.py
--rw-rw-rw-   0        0        0    27492 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_code/code.py
--rw-rw-rw-   0        0        0    14050 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_code/source.py
--rw-rw-rw-   0        0        0    11450 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_code/_assertionnew.py
--rw-rw-rw-   0        0        0    17869 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_code/_assertionold.py
--rw-rw-rw-   0        0        0     2765 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_code/_py2traceback.py
--rw-rw-rw-   0        0        0       46 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_code/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_error.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/py/_io/
--rw-rw-rw-   0        0        0    11652 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_io/capture.py
--rw-rw-rw-   0        0        0     2483 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_io/saferepr.py
--rw-rw-rw-   0        0        0    14714 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_io/terminalwriter.py
--rw-rw-rw-   0        0        0       29 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_io/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/py/_log/
--rw-rw-rw-   0        0        0     6003 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_log/log.py
--rw-rw-rw-   0        0        0     2565 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_log/warning.py
--rw-rw-rw-   0        0        0       74 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/py/_path/
--rw-rw-rw-   0        0        0     3333 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_path/cacheutil.py
--rw-rw-rw-   0        0        0    14818 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_path/common.py
--rw-rw-rw-   0        0        0    36759 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_path/local.py
--rw-rw-rw-   0        0        0    14715 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_path/svnurl.py
--rw-rw-rw-   0        0        0    43825 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_path/svnwc.py
--rw-rw-rw-   0        0        0       32 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_path/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/py/_process/
--rw-rw-rw-   0        0        0     1814 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_process/cmdexec.py
--rw-rw-rw-   0        0        0     3692 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_process/forkedfunc.py
--rw-rw-rw-   0        0        0      648 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_process/killproc.py
--rw-rw-rw-   0        0        0       40 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_process/__init__.py
--rw-rw-rw-   0        0        0      668 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_std.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/py/_vendored_packages/
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/py/_vendored_packages/apipkg/
--rw-rw-rw-   0        0        0      142 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_vendored_packages/apipkg/version.py
--rw-rw-rw-   0        0        0     6978 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_vendored_packages/apipkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/py/_vendored_packages/iniconfig/
--rw-rw-rw-   0        0        0     5208 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_vendored_packages/iniconfig/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_vendored_packages/__init__.py
--rw-rw-rw-   0        0        0      144 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_version.py
--rw-rw-rw-   0        0        0     8364 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/_xmlgen.py
--rw-rw-rw-   0        0        0     6022 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/py/__metainfo.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/pyparsing/
--rw-rw-rw-   0        0        0     6429 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/common.py
--rw-rw-rw-   0        0        0   212214 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/pyparsing/diagram/
--rw-rw-rw-   0        0        0    22136 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9030 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    38299 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25339 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/results.py
--rw-rw-rw-   0        0        0    13388 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10381 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/util.py
--rw-rw-rw-   0        0        0     9095 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pyparsing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/pytest/
--rw-rw-rw-   0        0        0      902 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pytest/collect.py
--rw-rw-rw-   0        0        0     5199 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pytest/__init__.py
--rw-rw-rw-   0        0        0      116 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/pytest/__main__.py
--rw-rw-rw-   0        0        0      177 2023-01-05 03:22:22.000000 ifly_uiautotest-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1508 2023-03-29 12:42:41.000000 ifly_uiautotest-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:55.000000 ifly_uiautotest-0.0.6/tomli/
--rw-rw-rw-   0        0        0    21659 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/tomli/_parser.py
--rw-rw-rw-   0        0        0     2818 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/tomli/_re.py
--rw-rw-rw-   0        0        0      126 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/tomli/_types.py
--rw-rw-rw-   0        0        0      299 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/tomli/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/_pytest/
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/_pytest/assertion/
--rw-rw-rw-   0        0        0    44251 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/assertion/rewrite.py
--rw-rw-rw-   0        0        0     3286 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/assertion/truncate.py
--rw-rw-rw-   0        0        0    17035 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/assertion/util.py
--rw-rw-rw-   0        0        0     6475 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/assertion/__init__.py
--rw-rw-rw-   0        0        0    20765 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/cacheprovider.py
--rw-rw-rw-   0        0        0    31121 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/capture.py
--rw-rw-rw-   0        0        0    12671 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/compat.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/_pytest/config/
--rw-rw-rw-   0        0        0    20740 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/config/argparsing.py
--rw-rw-rw-   0        0        0     2394 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/config/compat.py
--rw-rw-rw-   0        0        0      260 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/config/exceptions.py
--rw-rw-rw-   0        0        0     7572 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/config/findpaths.py
--rw-rw-rw-   0        0        0    59652 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/config/__init__.py
--rw-rw-rw-   0        0        0    13413 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/debugging.py
--rw-rw-rw-   0        0        0     5464 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/deprecated.py
--rw-rw-rw-   0        0        0    25476 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/doctest.py
--rw-rw-rw-   0        0        0     3187 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/faulthandler.py
--rw-rw-rw-   0        0        0    64860 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/fixtures.py
--rw-rw-rw-   0        0        0     1339 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/freeze_support.py
--rw-rw-rw-   0        0        0     8492 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/helpconfig.py
--rw-rw-rw-   0        0        0    32523 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/hookspec.py
--rw-rw-rw-   0        0        0    25594 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/junitxml.py
--rw-rw-rw-   0        0        0    16587 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/legacypath.py
--rw-rw-rw-   0        0        0    30227 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/logging.py
--rw-rw-rw-   0        0        0    32280 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/main.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/_pytest/mark/
--rw-rw-rw-   0        0        0     6412 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/mark/expression.py
--rw-rw-rw-   0        0        0    20512 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/mark/structures.py
--rw-rw-rw-   0        0        0     9010 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/mark/__init__.py
--rw-rw-rw-   0        0        0    12897 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/monkeypatch.py
--rw-rw-rw-   0        0        0    26035 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/nodes.py
--rw-rw-rw-   0        0        0     1370 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/nose.py
--rw-rw-rw-   0        0        0    10034 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/outcomes.py
--rw-rw-rw-   0        0        0     3950 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/pastebin.py
--rw-rw-rw-   0        0        0    24118 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/pathlib.py
--rw-rw-rw-   0        0        0    61109 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/pytester.py
--rw-rw-rw-   0        0        0     2327 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/pytester_assertions.py
--rw-rw-rw-   0        0        0    67157 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/python.py
--rw-rw-rw-   0        0        0    36652 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/python_api.py
--rw-rw-rw-   0        0        0      709 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/python_path.py
--rw-rw-rw-   0        0        0    10358 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/recwarn.py
--rw-rw-rw-   0        0        0    19898 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/reports.py
--rw-rw-rw-   0        0        0    18354 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/runner.py
--rw-rw-rw-   0        0        0     2882 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/scope.py
--rw-rw-rw-   0        0        0     3263 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/setuponly.py
--rw-rw-rw-   0        0        0     1215 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/setupplan.py
--rw-rw-rw-   0        0        0    10171 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/skipping.py
--rw-rw-rw-   0        0        0     3055 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/stash.py
--rw-rw-rw-   0        0        0     4340 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/stepwise.py
--rw-rw-rw-   0        0        0    50217 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/terminal.py
--rw-rw-rw-   0        0        0     2915 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/threadexception.py
--rw-rw-rw-   0        0        0      375 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/timing.py
--rw-rw-rw-   0        0        0     7811 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/tmpdir.py
--rw-rw-rw-   0        0        0    14452 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/unittest.py
--rw-rw-rw-   0        0        0     3191 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/unraisableexception.py
--rw-rw-rw-   0        0        0     4586 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/warnings.py
--rw-rw-rw-   0        0        0     3458 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/warning_types.py
--rw-rw-rw-   0        0        0     3810 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_argcomplete.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/_pytest/_code/
--rw-rw-rw-   0        0        0    43982 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_code/code.py
--rw-rw-rw-   0        0        0     7436 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_code/source.py
--rw-rw-rw-   0        0        0      483 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_code/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 12:42:54.000000 ifly_uiautotest-0.0.6/_pytest/_io/
--rw-rw-rw-   0        0        0     4592 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_io/saferepr.py
--rw-rw-rw-   0        0        0     8152 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_io/terminalwriter.py
--rw-rw-rw-   0        0        0     1253 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_io/wcwidth.py
--rw-rw-rw-   0        0        0      154 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_io/__init__.py
--rw-rw-rw-   0        0        0      142 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/_version.py
--rw-rw-rw-   0        0        0      356 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.6/_pytest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/atomicwrites/
+-rw-rw-rw-   0        0        0     6970 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/atomicwrites/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/attr/
+-rw-rw-rw-   0        0        0     3602 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/converters.py
+-rw-rw-rw-   0        0        0     1915 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/exceptions.py
+-rw-rw-rw-   0        0        0     1038 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/filters.py
+-rw-rw-rw-   0        0        0     1400 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/setters.py
+-rw-rw-rw-   0        0        0    20501 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/validators.py
+-rw-rw-rw-   0        0        0     4094 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/_cmp.py
+-rw-rw-rw-   0        0        0     5435 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/_compat.py
+-rw-rw-rw-   0        0        0      826 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/_config.py
+-rw-rw-rw-   0        0        0    14545 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/_funcs.py
+-rw-rw-rw-   0        0        0    96087 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/_make.py
+-rw-rw-rw-   0        0        0     6059 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/_next_gen.py
+-rw-rw-rw-   0        0        0     2121 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/_version_info.py
+-rw-rw-rw-   0        0        0     1947 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/attrs/
+-rw-rw-rw-   0        0        0       70 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attrs/converters.py
+-rw-rw-rw-   0        0        0       70 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attrs/exceptions.py
+-rw-rw-rw-   0        0        0       67 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attrs/filters.py
+-rw-rw-rw-   0        0        0       67 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attrs/setters.py
+-rw-rw-rw-   0        0        0       70 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attrs/validators.py
+-rw-rw-rw-   0        0        0     1149 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/attrs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/colorama/
+-rw-rw-rw-   0        0        0     2522 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10830 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/colorama/winterm.py
+-rw-rw-rw-   0        0        0      239 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/colorama/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/cookiecutter/
+-rw-rw-rw-   0        0        0     5140 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/cli.py
+-rw-rw-rw-   0        0        0     4429 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/config.py
+-rw-rw-rw-   0        0        0     2297 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/environment.py
+-rw-rw-rw-   0        0        0     3927 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/exceptions.py
+-rw-rw-rw-   0        0        0     1684 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/extensions.py
+-rw-rw-rw-   0        0        0     1034 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/find.py
+-rw-rw-rw-   0        0        0    13632 2023-03-29 07:24:45.000000 ifly_uiautotest-0.0.7/cookiecutter/generate.py
+-rw-rw-rw-   0        0        0     4168 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/hooks.py
+-rw-rw-rw-   0        0        0     1596 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/log.py
+-rw-rw-rw-   0        0        0     3698 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/main.py
+-rw-rw-rw-   0        0        0     7670 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/prompt.py
+-rw-rw-rw-   0        0        0     1567 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/replay.py
+-rw-rw-rw-   0        0        0     4272 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/repository.py
+-rw-rw-rw-   0        0        0     2734 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/utils.py
+-rw-rw-rw-   0        0        0     3890 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/vcs.py
+-rw-rw-rw-   0        0        0     4480 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/zipfile.py
+-rw-rw-rw-   0        0        0       85 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/__init__.py
+-rw-rw-rw-   0        0        0      258 2023-03-20 09:11:42.000000 ifly_uiautotest-0.0.7/cookiecutter/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/ifly_autotest/
+-rw-rw-rw-   0        0        0     1431 2023-03-29 12:39:44.000000 ifly_uiautotest-0.0.7/ifly_autotest/ifly_autotest.py
+-rw-rw-rw-   0        0        0       20 2023-03-28 06:27:23.000000 ifly_uiautotest-0.0.7/ifly_autotest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-09 04:54:39.000000 ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-09 04:54:39.000000 ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      575 2023-04-09 04:54:39.000000 ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-04-09 04:54:39.000000 ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     4466 2023-04-09 04:54:39.000000 ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      140 2023-04-09 04:54:39.000000 ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/importlib_metadata/
+-rw-rw-rw-   0        0        0     1862 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1826 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1154 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     2166 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/importlib_metadata/_text.py
+-rw-rw-rw-   0        0        0    30503 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/importlib_metadata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/iniconfig/
+-rw-rw-rw-   0        0        0     5225 2023-03-28 06:59:52.000000 ifly_uiautotest-0.0.7/iniconfig/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-01-05 03:23:29.000000 ifly_uiautotest-0.0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/packaging/
+-rw-rw-rw-   0        0        0     8475 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/markers.py
+-rw-rw-rw-   0        0        0     4664 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/version.py
+-rw-rw-rw-   0        0        0    11488 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/_structures.py
+-rw-rw-rw-   0        0        0      661 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/packaging/__init__.py
+-rw-rw-rw-   0        0        0      575 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/pluggy/
+-rw-rw-rw-   0        0        0     2097 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pluggy/_callers.py
+-rw-rw-rw-   0        0        0    11496 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pluggy/_hooks.py
+-rw-rw-rw-   0        0        0    14752 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pluggy/_manager.py
+-rw-rw-rw-   0        0        0     1535 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pluggy/_result.py
+-rw-rw-rw-   0        0        0     1541 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pluggy/_tracing.py
+-rw-rw-rw-   0        0        0      142 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pluggy/_version.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pluggy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/
+-rw-rw-rw-   0        0        0      222 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/test.py
+-rw-rw-rw-   0        0        0     4021 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_builtin.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/_code/
+-rw-rw-rw-   0        0        0     3174 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_code/assertion.py
+-rw-rw-rw-   0        0        0    27492 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_code/code.py
+-rw-rw-rw-   0        0        0    14050 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_code/source.py
+-rw-rw-rw-   0        0        0    11450 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_code/_assertionnew.py
+-rw-rw-rw-   0        0        0    17869 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_code/_assertionold.py
+-rw-rw-rw-   0        0        0     2765 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_code/_py2traceback.py
+-rw-rw-rw-   0        0        0       46 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_code/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_error.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/_io/
+-rw-rw-rw-   0        0        0    11652 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_io/capture.py
+-rw-rw-rw-   0        0        0     2483 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_io/saferepr.py
+-rw-rw-rw-   0        0        0    14714 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_io/terminalwriter.py
+-rw-rw-rw-   0        0        0       29 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_io/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/_log/
+-rw-rw-rw-   0        0        0     6003 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_log/log.py
+-rw-rw-rw-   0        0        0     2565 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_log/warning.py
+-rw-rw-rw-   0        0        0       74 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/_path/
+-rw-rw-rw-   0        0        0     3333 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_path/cacheutil.py
+-rw-rw-rw-   0        0        0    14818 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_path/common.py
+-rw-rw-rw-   0        0        0    36759 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_path/local.py
+-rw-rw-rw-   0        0        0    14715 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_path/svnurl.py
+-rw-rw-rw-   0        0        0    43825 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_path/svnwc.py
+-rw-rw-rw-   0        0        0       32 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_path/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/_process/
+-rw-rw-rw-   0        0        0     1814 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_process/cmdexec.py
+-rw-rw-rw-   0        0        0     3692 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_process/forkedfunc.py
+-rw-rw-rw-   0        0        0      648 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_process/killproc.py
+-rw-rw-rw-   0        0        0       40 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_process/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_std.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/_vendored_packages/
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/_vendored_packages/apipkg/
+-rw-rw-rw-   0        0        0      142 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_vendored_packages/apipkg/version.py
+-rw-rw-rw-   0        0        0     6978 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_vendored_packages/apipkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/py/_vendored_packages/iniconfig/
+-rw-rw-rw-   0        0        0     5208 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_vendored_packages/iniconfig/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_vendored_packages/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_version.py
+-rw-rw-rw-   0        0        0     8364 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/_xmlgen.py
+-rw-rw-rw-   0        0        0     6022 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/py/__metainfo.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/pyparsing/
+-rw-rw-rw-   0        0        0     6429 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/common.py
+-rw-rw-rw-   0        0        0   212214 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    22136 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9030 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    38299 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25339 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13388 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10381 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/util.py
+-rw-rw-rw-   0        0        0     9095 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pyparsing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/pytest/
+-rw-rw-rw-   0        0        0      902 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pytest/collect.py
+-rw-rw-rw-   0        0        0     5199 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pytest/__init__.py
+-rw-rw-rw-   0        0        0      116 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/pytest/__main__.py
+-rw-rw-rw-   0        0        0      177 2023-01-05 03:22:22.000000 ifly_uiautotest-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1492 2023-04-09 04:54:11.000000 ifly_uiautotest-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:41.000000 ifly_uiautotest-0.0.7/tomli/
+-rw-rw-rw-   0        0        0    21659 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2818 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/tomli/_re.py
+-rw-rw-rw-   0        0        0      126 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/tomli/_types.py
+-rw-rw-rw-   0        0        0      299 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/tomli/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/_pytest/
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/_pytest/assertion/
+-rw-rw-rw-   0        0        0    44251 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/assertion/rewrite.py
+-rw-rw-rw-   0        0        0     3286 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/assertion/truncate.py
+-rw-rw-rw-   0        0        0    17035 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/assertion/util.py
+-rw-rw-rw-   0        0        0     6475 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/assertion/__init__.py
+-rw-rw-rw-   0        0        0    20765 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/cacheprovider.py
+-rw-rw-rw-   0        0        0    31121 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/capture.py
+-rw-rw-rw-   0        0        0    12671 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/compat.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/_pytest/config/
+-rw-rw-rw-   0        0        0    20740 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/config/argparsing.py
+-rw-rw-rw-   0        0        0     2394 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/config/compat.py
+-rw-rw-rw-   0        0        0      260 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/config/exceptions.py
+-rw-rw-rw-   0        0        0     7572 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/config/findpaths.py
+-rw-rw-rw-   0        0        0    59652 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/config/__init__.py
+-rw-rw-rw-   0        0        0    13413 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/debugging.py
+-rw-rw-rw-   0        0        0     5464 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/deprecated.py
+-rw-rw-rw-   0        0        0    25476 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/doctest.py
+-rw-rw-rw-   0        0        0     3187 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/faulthandler.py
+-rw-rw-rw-   0        0        0    64860 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/fixtures.py
+-rw-rw-rw-   0        0        0     1339 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/freeze_support.py
+-rw-rw-rw-   0        0        0     8492 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/helpconfig.py
+-rw-rw-rw-   0        0        0    32523 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/hookspec.py
+-rw-rw-rw-   0        0        0    25594 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/junitxml.py
+-rw-rw-rw-   0        0        0    16587 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/legacypath.py
+-rw-rw-rw-   0        0        0    30227 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/logging.py
+-rw-rw-rw-   0        0        0    32280 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/main.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/_pytest/mark/
+-rw-rw-rw-   0        0        0     6412 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/mark/expression.py
+-rw-rw-rw-   0        0        0    20512 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/mark/structures.py
+-rw-rw-rw-   0        0        0     9010 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/mark/__init__.py
+-rw-rw-rw-   0        0        0    12897 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/monkeypatch.py
+-rw-rw-rw-   0        0        0    26035 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/nodes.py
+-rw-rw-rw-   0        0        0     1370 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/nose.py
+-rw-rw-rw-   0        0        0    10034 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/outcomes.py
+-rw-rw-rw-   0        0        0     3950 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/pastebin.py
+-rw-rw-rw-   0        0        0    24118 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/pathlib.py
+-rw-rw-rw-   0        0        0    61109 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/pytester.py
+-rw-rw-rw-   0        0        0     2327 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/pytester_assertions.py
+-rw-rw-rw-   0        0        0    67157 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/python.py
+-rw-rw-rw-   0        0        0    36652 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/python_api.py
+-rw-rw-rw-   0        0        0      709 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/python_path.py
+-rw-rw-rw-   0        0        0    10358 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/recwarn.py
+-rw-rw-rw-   0        0        0    19898 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/reports.py
+-rw-rw-rw-   0        0        0    18354 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/runner.py
+-rw-rw-rw-   0        0        0     2882 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/scope.py
+-rw-rw-rw-   0        0        0     3263 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/setuponly.py
+-rw-rw-rw-   0        0        0     1215 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/setupplan.py
+-rw-rw-rw-   0        0        0    10171 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/skipping.py
+-rw-rw-rw-   0        0        0     3055 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/stash.py
+-rw-rw-rw-   0        0        0     4340 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/stepwise.py
+-rw-rw-rw-   0        0        0    50217 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/terminal.py
+-rw-rw-rw-   0        0        0     2915 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/threadexception.py
+-rw-rw-rw-   0        0        0      375 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/timing.py
+-rw-rw-rw-   0        0        0     7811 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/tmpdir.py
+-rw-rw-rw-   0        0        0    14452 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/unittest.py
+-rw-rw-rw-   0        0        0     3191 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/unraisableexception.py
+-rw-rw-rw-   0        0        0     4586 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/warnings.py
+-rw-rw-rw-   0        0        0     3458 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/warning_types.py
+-rw-rw-rw-   0        0        0     3810 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_argcomplete.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/_pytest/_code/
+-rw-rw-rw-   0        0        0    43982 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_code/code.py
+-rw-rw-rw-   0        0        0     7436 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_code/source.py
+-rw-rw-rw-   0        0        0      483 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_code/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:54:40.000000 ifly_uiautotest-0.0.7/_pytest/_io/
+-rw-rw-rw-   0        0        0     4592 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_io/saferepr.py
+-rw-rw-rw-   0        0        0     8152 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_io/terminalwriter.py
+-rw-rw-rw-   0        0        0     1253 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_io/wcwidth.py
+-rw-rw-rw-   0        0        0      154 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_io/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/_version.py
+-rw-rw-rw-   0        0        0      356 2023-03-28 06:58:13.000000 ifly_uiautotest-0.0.7/_pytest/__init__.py
```

### Comparing `ifly_uiautotest-0.0.6/atomicwrites/__init__.py` & `ifly_uiautotest-0.0.7/atomicwrites/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/converters.py` & `ifly_uiautotest-0.0.7/attr/converters.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/exceptions.py` & `ifly_uiautotest-0.0.7/attr/exceptions.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/filters.py` & `ifly_uiautotest-0.0.7/attr/filters.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/setters.py` & `ifly_uiautotest-0.0.7/attr/setters.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/validators.py` & `ifly_uiautotest-0.0.7/attr/validators.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/_cmp.py` & `ifly_uiautotest-0.0.7/attr/_cmp.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/_compat.py` & `ifly_uiautotest-0.0.7/attr/_compat.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/_config.py` & `ifly_uiautotest-0.0.7/attr/_config.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/_funcs.py` & `ifly_uiautotest-0.0.7/attr/_funcs.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/_make.py` & `ifly_uiautotest-0.0.7/attr/_make.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/_next_gen.py` & `ifly_uiautotest-0.0.7/attr/_next_gen.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/_version_info.py` & `ifly_uiautotest-0.0.7/attr/_version_info.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attr/__init__.py` & `ifly_uiautotest-0.0.7/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/attrs/__init__.py` & `ifly_uiautotest-0.0.7/attrs/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/colorama/ansi.py` & `ifly_uiautotest-0.0.7/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/colorama/ansitowin32.py` & `ifly_uiautotest-0.0.7/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/colorama/initialise.py` & `ifly_uiautotest-0.0.7/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/colorama/win32.py` & `ifly_uiautotest-0.0.7/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/colorama/winterm.py` & `ifly_uiautotest-0.0.7/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/cli.py` & `ifly_uiautotest-0.0.7/cookiecutter/cli.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/config.py` & `ifly_uiautotest-0.0.7/cookiecutter/config.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/environment.py` & `ifly_uiautotest-0.0.7/cookiecutter/environment.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/exceptions.py` & `ifly_uiautotest-0.0.7/cookiecutter/exceptions.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/extensions.py` & `ifly_uiautotest-0.0.7/cookiecutter/extensions.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/find.py` & `ifly_uiautotest-0.0.7/cookiecutter/find.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/generate.py` & `ifly_uiautotest-0.0.7/cookiecutter/generate.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/hooks.py` & `ifly_uiautotest-0.0.7/cookiecutter/hooks.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/log.py` & `ifly_uiautotest-0.0.7/cookiecutter/log.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/main.py` & `ifly_uiautotest-0.0.7/cookiecutter/main.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/prompt.py` & `ifly_uiautotest-0.0.7/cookiecutter/prompt.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/replay.py` & `ifly_uiautotest-0.0.7/cookiecutter/replay.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/repository.py` & `ifly_uiautotest-0.0.7/cookiecutter/repository.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/utils.py` & `ifly_uiautotest-0.0.7/cookiecutter/utils.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/vcs.py` & `ifly_uiautotest-0.0.7/cookiecutter/vcs.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/cookiecutter/zipfile.py` & `ifly_uiautotest-0.0.7/cookiecutter/zipfile.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/ifly_autotest/ifly_autotest.py` & `ifly_uiautotest-0.0.7/ifly_autotest/ifly_autotest.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/PKG-INFO` & `ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ifly-uiautotest
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: UNKNOWN
-Author: hnzhu2
-Author-email: hnzhu2@iflytek.com
+Author: 
+Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ifly_uiautotest-0.0.6/ifly_uiautotest.egg-info/SOURCES.txt` & `ifly_uiautotest-0.0.7/ifly_uiautotest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/importlib_metadata/_adapters.py` & `ifly_uiautotest-0.0.7/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/importlib_metadata/_collections.py` & `ifly_uiautotest-0.0.7/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/importlib_metadata/_compat.py` & `ifly_uiautotest-0.0.7/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/importlib_metadata/_functools.py` & `ifly_uiautotest-0.0.7/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/importlib_metadata/_itertools.py` & `ifly_uiautotest-0.0.7/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/importlib_metadata/_meta.py` & `ifly_uiautotest-0.0.7/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/importlib_metadata/_text.py` & `ifly_uiautotest-0.0.7/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/importlib_metadata/__init__.py` & `ifly_uiautotest-0.0.7/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/iniconfig/__init__.py` & `ifly_uiautotest-0.0.7/iniconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/LICENSE` & `ifly_uiautotest-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/markers.py` & `ifly_uiautotest-0.0.7/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/requirements.py` & `ifly_uiautotest-0.0.7/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/specifiers.py` & `ifly_uiautotest-0.0.7/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/tags.py` & `ifly_uiautotest-0.0.7/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/utils.py` & `ifly_uiautotest-0.0.7/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/version.py` & `ifly_uiautotest-0.0.7/packaging/version.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/_manylinux.py` & `ifly_uiautotest-0.0.7/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/_musllinux.py` & `ifly_uiautotest-0.0.7/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/_structures.py` & `ifly_uiautotest-0.0.7/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/packaging/__about__.py` & `ifly_uiautotest-0.0.7/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/PKG-INFO` & `ifly_uiautotest-0.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ifly_uiautotest
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: UNKNOWN
-Author: hnzhu2
-Author-email: hnzhu2@iflytek.com
+Author: 
+Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ifly_uiautotest-0.0.6/pluggy/_callers.py` & `ifly_uiautotest-0.0.7/pluggy/_callers.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pluggy/_hooks.py` & `ifly_uiautotest-0.0.7/pluggy/_hooks.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pluggy/_manager.py` & `ifly_uiautotest-0.0.7/pluggy/_manager.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pluggy/_result.py` & `ifly_uiautotest-0.0.7/pluggy/_result.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pluggy/_tracing.py` & `ifly_uiautotest-0.0.7/pluggy/_tracing.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_builtin.py` & `ifly_uiautotest-0.0.7/py/_builtin.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_code/assertion.py` & `ifly_uiautotest-0.0.7/py/_code/assertion.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_code/code.py` & `ifly_uiautotest-0.0.7/py/_code/code.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_code/source.py` & `ifly_uiautotest-0.0.7/py/_code/source.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_code/_assertionnew.py` & `ifly_uiautotest-0.0.7/py/_code/_assertionnew.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_code/_assertionold.py` & `ifly_uiautotest-0.0.7/py/_code/_assertionold.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_code/_py2traceback.py` & `ifly_uiautotest-0.0.7/py/_code/_py2traceback.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_error.py` & `ifly_uiautotest-0.0.7/py/_error.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_io/capture.py` & `ifly_uiautotest-0.0.7/py/_io/capture.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_io/saferepr.py` & `ifly_uiautotest-0.0.7/py/_io/saferepr.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_io/terminalwriter.py` & `ifly_uiautotest-0.0.7/py/_io/terminalwriter.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_log/log.py` & `ifly_uiautotest-0.0.7/py/_log/log.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_log/warning.py` & `ifly_uiautotest-0.0.7/py/_log/warning.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_path/cacheutil.py` & `ifly_uiautotest-0.0.7/py/_path/cacheutil.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_path/common.py` & `ifly_uiautotest-0.0.7/py/_path/common.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_path/local.py` & `ifly_uiautotest-0.0.7/py/_path/local.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_path/svnurl.py` & `ifly_uiautotest-0.0.7/py/_path/svnurl.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_path/svnwc.py` & `ifly_uiautotest-0.0.7/py/_path/svnwc.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_process/cmdexec.py` & `ifly_uiautotest-0.0.7/py/_process/cmdexec.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_process/forkedfunc.py` & `ifly_uiautotest-0.0.7/py/_process/forkedfunc.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_process/killproc.py` & `ifly_uiautotest-0.0.7/py/_process/killproc.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_std.py` & `ifly_uiautotest-0.0.7/py/_std.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_vendored_packages/apipkg/__init__.py` & `ifly_uiautotest-0.0.7/py/_vendored_packages/apipkg/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_vendored_packages/iniconfig/__init__.py` & `ifly_uiautotest-0.0.7/py/_vendored_packages/iniconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/_xmlgen.py` & `ifly_uiautotest-0.0.7/py/_xmlgen.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/py/__init__.py` & `ifly_uiautotest-0.0.7/py/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/actions.py` & `ifly_uiautotest-0.0.7/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/common.py` & `ifly_uiautotest-0.0.7/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/core.py` & `ifly_uiautotest-0.0.7/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/diagram/__init__.py` & `ifly_uiautotest-0.0.7/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/exceptions.py` & `ifly_uiautotest-0.0.7/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/helpers.py` & `ifly_uiautotest-0.0.7/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/results.py` & `ifly_uiautotest-0.0.7/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/testing.py` & `ifly_uiautotest-0.0.7/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/unicode.py` & `ifly_uiautotest-0.0.7/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/util.py` & `ifly_uiautotest-0.0.7/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pyparsing/__init__.py` & `ifly_uiautotest-0.0.7/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pytest/collect.py` & `ifly_uiautotest-0.0.7/pytest/collect.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/pytest/__init__.py` & `ifly_uiautotest-0.0.7/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/setup.py` & `ifly_uiautotest-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ifly_uiautotest",
-    version="0.0.6",
-    author="hnzhu2",
-    author_email="hnzhu2@iflytek.com",
+    version="0.0.7",
+    author="",
+    author_email="",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
         entry_points={
         'console_scripts': [
@@ -34,15 +34,15 @@
             'pocoui==1.0.87',
             'allure-combine==1.0.6',
             'allure-pytest==2.9.45',
             'allure-python-commons==2.9.45',
             'openpyxl==3.0.10',
             'pytest-ordering==0.6',
             'pytest-repeat==0.9.1',
-            'numpy',
+            'numpy==1.19.5',
             'opencv-contrib-python',
             'Levenshtein',
             'onnxruntime',
             'pyclipper',
             'requests',
             'Shapely==1.7.1',
             'tqdm',
```

### Comparing `ifly_uiautotest-0.0.6/tomli/_parser.py` & `ifly_uiautotest-0.0.7/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/tomli/_re.py` & `ifly_uiautotest-0.0.7/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/assertion/rewrite.py` & `ifly_uiautotest-0.0.7/_pytest/assertion/rewrite.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/assertion/truncate.py` & `ifly_uiautotest-0.0.7/_pytest/assertion/truncate.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/assertion/util.py` & `ifly_uiautotest-0.0.7/_pytest/assertion/util.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/assertion/__init__.py` & `ifly_uiautotest-0.0.7/_pytest/assertion/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/cacheprovider.py` & `ifly_uiautotest-0.0.7/_pytest/cacheprovider.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/capture.py` & `ifly_uiautotest-0.0.7/_pytest/capture.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/compat.py` & `ifly_uiautotest-0.0.7/_pytest/compat.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/config/argparsing.py` & `ifly_uiautotest-0.0.7/_pytest/config/argparsing.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/config/compat.py` & `ifly_uiautotest-0.0.7/_pytest/config/compat.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/config/findpaths.py` & `ifly_uiautotest-0.0.7/_pytest/config/findpaths.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/config/__init__.py` & `ifly_uiautotest-0.0.7/_pytest/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/debugging.py` & `ifly_uiautotest-0.0.7/_pytest/debugging.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/deprecated.py` & `ifly_uiautotest-0.0.7/_pytest/deprecated.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/doctest.py` & `ifly_uiautotest-0.0.7/_pytest/doctest.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/faulthandler.py` & `ifly_uiautotest-0.0.7/_pytest/faulthandler.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/fixtures.py` & `ifly_uiautotest-0.0.7/_pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/freeze_support.py` & `ifly_uiautotest-0.0.7/_pytest/freeze_support.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/helpconfig.py` & `ifly_uiautotest-0.0.7/_pytest/helpconfig.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/hookspec.py` & `ifly_uiautotest-0.0.7/_pytest/hookspec.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/junitxml.py` & `ifly_uiautotest-0.0.7/_pytest/junitxml.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/legacypath.py` & `ifly_uiautotest-0.0.7/_pytest/legacypath.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/logging.py` & `ifly_uiautotest-0.0.7/_pytest/logging.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/main.py` & `ifly_uiautotest-0.0.7/_pytest/main.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/mark/expression.py` & `ifly_uiautotest-0.0.7/_pytest/mark/expression.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/mark/structures.py` & `ifly_uiautotest-0.0.7/_pytest/mark/structures.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/mark/__init__.py` & `ifly_uiautotest-0.0.7/_pytest/mark/__init__.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/monkeypatch.py` & `ifly_uiautotest-0.0.7/_pytest/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/nodes.py` & `ifly_uiautotest-0.0.7/_pytest/nodes.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/nose.py` & `ifly_uiautotest-0.0.7/_pytest/nose.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/outcomes.py` & `ifly_uiautotest-0.0.7/_pytest/outcomes.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/pastebin.py` & `ifly_uiautotest-0.0.7/_pytest/pastebin.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/pathlib.py` & `ifly_uiautotest-0.0.7/_pytest/pathlib.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/pytester.py` & `ifly_uiautotest-0.0.7/_pytest/pytester.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/pytester_assertions.py` & `ifly_uiautotest-0.0.7/_pytest/pytester_assertions.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/python.py` & `ifly_uiautotest-0.0.7/_pytest/python.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/python_api.py` & `ifly_uiautotest-0.0.7/_pytest/python_api.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/python_path.py` & `ifly_uiautotest-0.0.7/_pytest/python_path.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/recwarn.py` & `ifly_uiautotest-0.0.7/_pytest/recwarn.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/reports.py` & `ifly_uiautotest-0.0.7/_pytest/reports.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/runner.py` & `ifly_uiautotest-0.0.7/_pytest/runner.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/scope.py` & `ifly_uiautotest-0.0.7/_pytest/scope.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/setuponly.py` & `ifly_uiautotest-0.0.7/_pytest/setuponly.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/setupplan.py` & `ifly_uiautotest-0.0.7/_pytest/setupplan.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/skipping.py` & `ifly_uiautotest-0.0.7/_pytest/skipping.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/stash.py` & `ifly_uiautotest-0.0.7/_pytest/stash.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/stepwise.py` & `ifly_uiautotest-0.0.7/_pytest/stepwise.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/terminal.py` & `ifly_uiautotest-0.0.7/_pytest/terminal.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/threadexception.py` & `ifly_uiautotest-0.0.7/_pytest/threadexception.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/tmpdir.py` & `ifly_uiautotest-0.0.7/_pytest/tmpdir.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/unittest.py` & `ifly_uiautotest-0.0.7/_pytest/unittest.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/unraisableexception.py` & `ifly_uiautotest-0.0.7/_pytest/unraisableexception.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/warnings.py` & `ifly_uiautotest-0.0.7/_pytest/warnings.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/warning_types.py` & `ifly_uiautotest-0.0.7/_pytest/warning_types.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/_argcomplete.py` & `ifly_uiautotest-0.0.7/_pytest/_argcomplete.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/_code/code.py` & `ifly_uiautotest-0.0.7/_pytest/_code/code.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/_code/source.py` & `ifly_uiautotest-0.0.7/_pytest/_code/source.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/_io/saferepr.py` & `ifly_uiautotest-0.0.7/_pytest/_io/saferepr.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/_io/terminalwriter.py` & `ifly_uiautotest-0.0.7/_pytest/_io/terminalwriter.py`

 * *Files identical despite different names*

### Comparing `ifly_uiautotest-0.0.6/_pytest/_io/wcwidth.py` & `ifly_uiautotest-0.0.7/_pytest/_io/wcwidth.py`

 * *Files identical despite different names*

