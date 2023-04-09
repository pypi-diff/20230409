# Comparing `tmp/tts_arranger-0.0.3.tar.gz` & `tmp/tts_arranger-0.0.4.tar.gz`

## Comparing `tts_arranger-0.0.3.tar` & `tts_arranger-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,675 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/requirements.txt
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/example.py
--rw-r--r--   0        0        0    28543 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/tts_arranger.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/data/replace
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/data/replace_de
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/data/replace_en
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    17107 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/LICENSE
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 tts_arranger-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/example.py
+-rw-r--r--   0        0        0    28680 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/tts_arranger.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_csv.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/csv.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/csv.meta.json
+-rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
+-rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json
+-rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json
+-rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
+-rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/data/replace
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/data/replace_de
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/data/replace_en
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json
+-rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
+-rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json
+-rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json
+-rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
+-rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0    17107 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/LICENSE
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/PKG-INFO
```

### Comparing `tts_arranger-0.0.3/src/tts_arranger/tts_arranger.py` & `tts_arranger-0.0.4/src/tts_arranger/tts_arranger.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import re
 import string
 import sys
 import time
 from dataclasses import dataclass
 from pathlib import Path
+from typing import Callable
 
 import TTS
 from num2words import num2words
 from pydub import AudioSegment
 from pydub.silence import detect_silence
 from TTS.utils.manage import ModelManager
 from TTS.utils.synthesizer import Synthesizer
@@ -49,38 +50,38 @@
 
     Args:
         model (str): model to be used, defaults to 'tts_models/en/vctk/vits'
         vocoder (str): vocoder to be used
         preferred_speakers (list): list containing strings of preferred speaker names to be used instead of all available speakers of the selected model (not yet implemented)
     """
 
-    def __init__(self, model='tts_models/en/vctk/vits', vocoder='', preferred_speakers=None) -> None:
+    def __init__(self, model='', vocoder='', preferred_speakers: list[str] | None = None) -> None:
+        if not model:
+            model = 'tts_models/en/vctk/vits'
+
         self.model = model
         self.vocoder = vocoder
         self.silence_length = 100
         self.silence_threshold = -60
         # self.pause_post_regular =
 
         # self.quotes = quotes
         self.current_speaker_idx = 0
 
-        self.speakers = []
+        self.speakers: list[str] = []
 
         # Config
         self.pause_sentence = 750
         self.pause_question_exclamation = 1000
         self.pause_parentheses = 300
         self.pause_dash = 300
         self.pause_newline = 250
         self.pause_colon = 100
 
-        if not preferred_speakers:
-            preferred_speakers = []
-
-        self.preferred_speakers = []
+        self.preferred_speakers = preferred_speakers or []
 
         # if not self.default_speakers:
         #     with open(os.path.dirname(os.path.realpath(__file__)) + '/speakers', 'r') as speaker_file:
         #         self.default_speakers = speaker_file.read().split()
 
         # if speakers:
         #     self.default_speakers = speakers
@@ -484,15 +485,15 @@
 
         return final_items
 
     def _merge_similar_items(self, items=[]) -> list:
         """
         Merge similar items for smoother synthesizing and avoiding unwanted pauses
         """
-        final_items = []
+        final_items: list[TTS_Item] = []
 
         if items:
             start_item = -1
             merged_item = TTS_Item()
 
             for i, item in enumerate(items):
                 if start_item < 0:
@@ -522,15 +523,15 @@
                         if final_items[-1] != merged_item:
                             final_items.append(merged_item)
                     else:
                         final_items.append(merged_item)
 
         return final_items
 
-    def synthesize_and_write(self, tts_items: list[TTS_Item], output_filename: str, callback=None):
+    def synthesize_and_write(self, tts_items: list[TTS_Item], output_filename: str, callback: Callable[[int, int], None] | None = None):
         """
         Synthesize and write list of items as an audio file
 
         Args:
             tts_items (list[TTS_Item]): List of items to be synthesized
             output_filename (str): Absolute path and filename of output audio file including file type extension (for example mp3, ogg)
             callback (function): Reference to function to be called after synthesizing of an item if finished, parameters: index (int), total number of items (int)
@@ -566,15 +567,15 @@
                 time_total += time_now - time_last
                 characters_total += len(tts_item.text)
 
                 if characters_total > 0:
                     time_needed = ((time_total / characters_total) * characters_sum) - time_total
 
                 # Report progress
-                if callback:
+                if callback is not None:
                     callback(idx, len(tts_items))
             except KeyboardInterrupt:
                 log(LOG_TYPE.ERROR, 'Stopped by user.')
                 sys.exit()
             except Exception as e:
                 # with open(self.temp_dir.name + '/tts-error.log', 'a+') as f:
                 #     f.write(f'Error synthesizing "{output_filename}"\n')
@@ -584,34 +585,32 @@
         self.write(segments, output_filename)
 
     def synthesize_tts_item(self, tts_item: TTS_Item) -> AudioSegment:
         """
         Synthesize a single item and return a pydub AudioSegment
         """
         segment = AudioSegment.empty()
-        # if self.synthesizer is not None:
+
         if tts_item.text:
             try:
-                # Suppress tts output
-
                 speaker = ''
 
                 if self.synthesizer.tts_model:
                     if self.synthesizer.tts_model.num_speakers > 1:
                         speaker = tts_item.speaker
 
                         # Use index if no explicit speaker name is given, wrap around speakers to avoid undefined indexes
                         if not speaker:
                             speaker = self.speakers[tts_item.speaker_idx % len(self.speakers)]
 
                             if self.preferred_speakers:
-                                # if len(self.preferred_speakers) >= tts_item.speaker_idx:
                                 if self.preferred_speakers[tts_item.speaker_idx % len(self.preferred_speakers)] in self.speakers:
                                     speaker = self.preferred_speakers[tts_item.speaker_idx % len(self.preferred_speakers)]
 
+                # Suppress tts output
                 with contextlib.redirect_stdout(None):
                     wav = self.synthesizer.tts(
                         text=tts_item.text,
                         speaker_name=speaker,
                     )
             except Exception as e:
                 raise Exception(f'Error synthesizing "{tts_item.text}: {e}"')
@@ -641,27 +640,27 @@
         Compress, convert and write AudioSegment as a given output file path and name
         """
         # Clean up to free up some memory
         # self.synthesizer = None
         # gc.collect()
 
         # Set default format to mp3
-        format = 'mp3'
-
-        file_format = os.path.splitext(output_filename)[1][1:]
-
-        if file_format:
-            format = file_format
-
-        log(LOG_TYPE.INFO, f'Compressing, converting and saving as {output_filename}')
+        format = os.path.splitext(output_filename)[1][1:] or 'mp3'
 
         folder = os.path.dirname(os.path.abspath(output_filename))
 
         if not os.path.exists(folder):
             os.makedirs(folder, exist_ok=True)
 
+        # Ensure output file name has a file extension
+        output_filename = os.path.splitext(output_filename)[0] + '.' + format
+
+        log(LOG_TYPE.INFO, f'Compressing, converting and saving as {output_filename}')
+
         comp_expansion = 12.5
         comp_raise = 0.0001
 
         # Apply dynamic compression
         # segment.export(output_filename, format, parameters=['-filter', 'speechnorm=e=25:r=0.0001:l=1', '-filter', 'loudnorm=tp=-1.0:offset=7'])
-        segment.export(output_filename, format, parameters=['-filter', f'speechnorm=e={comp_expansion}:r={comp_raise}:l=1'])
+        params = ['-filter', f'speechnorm=e={comp_expansion}:r={comp_raise}:l=1']
+        bitrate = '320k' if format == 'mp3' else None
+        segment.export(output_filename, format, parameters=params, bitrate=bitrate)
```

### Comparing `tts_arranger-0.0.3/src/tts_arranger/utils/audio.py` & `tts_arranger-0.0.4/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.3/src/tts_arranger/utils/log.py` & `tts_arranger-0.0.4/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.3/tests/tts_arranger_test.py` & `tts_arranger-0.0.4/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.3/LICENSE` & `tts_arranger-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.3/README.md` & `tts_arranger-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.3/pyproject.toml` & `tts_arranger-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.0.3"
+version = "0.0.4"
 
 dependencies = [
   "numpy>=1.22.4",
   "pydub>=0.25.1",
   "scipy>=1.9.0",
   "TTS>=0.10.2",
   "num2words>=0.5.11"
```

### Comparing `tts_arranger-0.0.3/PKG-INFO` & `tts_arranger-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

