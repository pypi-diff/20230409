# Comparing `tmp/tts_arranger-0.0.4.tar.gz` & `tmp/tts_arranger-0.0.5.tar.gz`

## Comparing `tts_arranger-0.0.4.tar` & `tts_arranger-0.0.5.tar`

### file list

```diff
@@ -1,675 +1,681 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/requirements.txt
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/example.py
--rw-r--r--   0        0        0    28680 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/tts_arranger.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_csv.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/csv.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/csv.meta.json
--rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json
--rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json
--rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
--rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json
--rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
--rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json
--rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
--rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json
--rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json
--rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json
--rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json
--rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json
--rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/data/replace
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/data/replace_de
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/data/replace_en
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json
--rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json
--rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json
--rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
--rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json
--rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
--rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json
--rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
--rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json
--rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json
--rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json
--rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json
--rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json
--rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json
--rw-r--r--   0        0        0    17107 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/LICENSE
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 tts_arranger-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    30020 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0    12453 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/tts_writer_example.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_csv.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/csv.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/csv.meta.json
+-rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
+-rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json
+-rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json
+-rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
+-rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/data/replace
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/data/replace_de
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/data/replace_en
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json
+-rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
+-rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json
+-rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json
+-rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
+-rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/LICENSE
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/PKG-INFO
```

### Comparing `tts_arranger-0.0.4/src/tts_arranger/tts_arranger.py` & `tts_arranger-0.0.5/src/tts_arranger/tts_processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,66 +3,48 @@
 import csv
 import datetime
 import os
 import re
 import string
 import sys
 import time
-from dataclasses import dataclass
 from pathlib import Path
-from typing import Callable
+from typing import Callable, Optional
 
-import TTS
-from num2words import num2words
-from pydub import AudioSegment
-from pydub.silence import detect_silence
-from TTS.utils.manage import ModelManager
-from TTS.utils.synthesizer import Synthesizer
+import numpy as np  # type: ignore
+import TTS  # type: ignore
+from num2words import num2words  # type: ignore
+from pydub import AudioSegment  # type: ignore
+from pydub.silence import detect_silence  # type: ignore
+from TTS.utils.manage import ModelManager  # type: ignore
+from TTS.utils.synthesizer import Synthesizer  # type: ignore
 
+from .items.tts_item import TTS_Item
 from .utils.audio import numpy_to_segment
 from .utils.log import LOG_TYPE, bcolors, log
 
 
-@dataclass
-class TTS_Item:
-    """
-    Represents a tts item containing various information
-
-    Args:
-        text (str): Text to be synthesized, can be left empty in combination with length > 0 to create pause
-        speaker (str): speaker name to be used
-        speaker_idx (int): speaker index to be used if no speaker name is given; wraps around based on the actual available speaker indexes per model
-        length (int): minimum length in milliseconds; will be padded if actual synthesized text fragment is shorter and ignored if it is longer     
-    """
-    text: str = ''
-    speaker: str = ''
-    speaker_idx: int = 0
-    length: int = 0
-
-    def __post_init__(self):
-        # Mark pauses by invalidating speaker index
-        if self.text == '' and self.length > 0:
-            self.speaker_idx = -1
-
-
-class TTS_Arranger:
-    """
-    Offers functionality for processing a list of TTS_Items
-
-    Args:
-        model (str): model to be used, defaults to 'tts_models/en/vctk/vits'
-        vocoder (str): vocoder to be used
-        preferred_speakers (list): list containing strings of preferred speaker names to be used instead of all available speakers of the selected model (not yet implemented)
-    """
-
-    def __init__(self, model='', vocoder='', preferred_speakers: list[str] | None = None) -> None:
-        if not model:
-            model = 'tts_models/en/vctk/vits'
+class TTS_Processor:
+    def __init__(self, model='', vocoder: str = '', preferred_speakers: Optional[list[str]] = None) -> None:
+        """
+        Initializes a new instance of the TTS class.
+
+        :param model: Name of the text-to-speech model to use.
+        :type model: str
+
+        :param vocoder: Name of the vocoder to use.
+        :type vocoder: str
 
-        self.model = model
+        :param preferred_speakers: A list of preferred speaker names for multi-speaker models to be used instead of the available speakers of the selected model (not yet implemented).
+                                If set to None, the default speaker(s) will be used.
+        :type preferred_speakers: list[str] or None
+
+        :return: None
+        """
+        self.model = model or 'tts_models/en/vctk/vits'
         self.vocoder = vocoder
         self.silence_length = 100
         self.silence_threshold = -60
         # self.pause_post_regular =
 
         # self.quotes = quotes
         self.current_speaker_idx = 0
@@ -87,65 +69,55 @@
         #     self.default_speakers = speakers
 
         self.replace = {}
 
         source_dir = Path(__file__).resolve().parent
 
         # Load general replace list
-        with open(str(source_dir) + '/data/replace', 'r') as file:
-            reader = csv.reader(file, delimiter='\t')
-            for row in reader:
+        with open(source_dir / 'data/replace', 'r') as file:
+            for row in csv.reader(file, delimiter='\t'):
                 self.replace[row[0]] = row[1]
 
         # Load language specific replace list
-        lang = 'en'
-
-        model_splitted = model.split('/')
+        lang = self.model.split('/')[1] if '/' in self.model else 'en'
 
-        if model_splitted:
-            if len(model_splitted) >= 2:
-                lang = model_splitted[1]
-
-        with open(str(source_dir) + f'/data/replace_{lang}', 'r') as file:
-            reader = csv.reader(file, delimiter='\t')
-            for row in reader:
+        with open(source_dir / f'data/replace_{lang}', 'r') as file:
+            for row in csv.reader(file, delimiter='\t'):
                 self.replace[row[0]] = row[1]
 
     # def __del__(self):
     #     self.temp_dir.cleanup()
     #     self.synthesizer = None
     #     gc.collect()
 
-    def initialize(self):
+    def initialize(self) -> None:
         """
-        Initializes the TTS system and fills the speaker list
+        Initializes the text-to-speech (TTS) system, downloads the specified models, and populates the speaker list.
+
+        :return: None
         """
         log(LOG_TYPE.INFO, f'Initializing speech synthesizer')
-        self.manager = ModelManager(str(Path(TTS.__file__).resolve().parent) + '/.models.json')
+        models_dir = Path(TTS.__file__).resolve().parent / '.models.json'
+        self.manager = ModelManager(str(models_dir))
 
         with contextlib.redirect_stdout(None):
-            model_path, config_path, _ = self.manager.download_model(self.model)
-
-            vocoder_path = ''
-            vocoder_config_path = ''
-
-            if self.vocoder:
-                vocoder_path, vocoder_config_path, _ = self.manager.download_model(self.vocoder)
+            (model_path, config_path, _), (vocoder_path, vocoder_config_path, _) = [
+                self.manager.download_model(m) if m else ('', '', '') for m in (self.model, self.vocoder)
+            ]
 
             self.synthesizer = Synthesizer(
                 tts_checkpoint=model_path,
                 tts_config_path=config_path,
                 vocoder_checkpoint=vocoder_path,
-                vocoder_config=vocoder_config_path,
+                vocoder_config=vocoder_config_path if self.vocoder else '',
             )
 
             # Get speaker list from model
-            if self.synthesizer.tts_model:
-                if self.synthesizer.tts_model.num_speakers > 1:
-                    self.speakers = list(self.synthesizer.tts_model.speaker_manager.name_to_id.keys())
+            if self.synthesizer.tts_model and self.synthesizer.tts_model.num_speakers > 1:
+                self.speakers = list(self.synthesizer.tts_model.speaker_manager.name_to_id.keys())
 
     # def _find_and_break(self, tts_items: list[TTS_Item], break_at: list[str], break_after: int) -> list[TTS_Item]:
     #     final_items = []
 
     #     for tts_item in tts_items:
     #         line = tts_item.text
     #         found = False
@@ -167,89 +139,90 @@
     #                 final_items += self._find_and_break([TTS_Item(line[break_after:].strip(), tts_item.speaker, tts_item.pause_pre,
     #                                                     tts_item.pause_post, tts_item.strip_silence)], break_at, break_after)
     #         else:
     #             final_items.append(TTS_Item(line.strip(), tts_item.speaker, tts_item.pause_pre, tts_item.pause_post, tts_item.strip_silence))
 
     #     return final_items
 
-    def _minimize_tailing_punctuation(self, text: str) -> str:
+    def _de_thorsten_tacotron2_DDC_tweaks(self, tts_item: TTS_Item) -> TTS_Item:
         """
-        Minimize tailing punctuation to work around issues with some models
+        Apply tweaks for tts_models/de/thorsten/tacotron2-DDC.
+
+        :param tts_item: The input TTS item to be processed.
+        :type tts_item: TTS_Item
+
+        :return: The processed TTS item with applied tweaks.
+        :rtype: TTS_Item
         """
-        lenght = 0
+        str_months = ('Januar', 'Februar', 'März', 'April', 'Mai', 'Juni', 'Juli', 'August', 'September', 'Oktober', 'November', 'Dezember')
 
-        for i in reversed(text):
-            if i in string.punctuation + ' ':
-                lenght += 1
+        # Ordinal numbers
+        def replace_number(match):
+            num = match.group(0)
+            if tts_item.text[match.end():].strip().startswith(str_months):
+                return num2words(num, lang='de', to='ordinal')
             else:
-                return text[:len(text) - (lenght - 1)]
-        return text
+                return num
+
+        tts_item.text = re.sub(r'\b[0-9]+\.', replace_number, tts_item.text)
+
+        # Year numbers
+        start = 0
+        while result := re.search(r'\b[0-9]{4,4}\b', tts_item.text[start:]):
+            len_original = 0
+            numword = ''
+            # When followed by month names
+            if tts_item.text[:start + result.span()[0]].strip().endswith(('Jahr', 'in', 'vor', 'nach') + str_months):
+                match = tts_item.text[start + result.span()[0]:start + result.span()[1]]
+
+                if int(match) < 2000:
+                    len_original = len(match)
+                    numword = num2words(match, lang='de', to='year')
+                    tts_item.text = tts_item.text[:start + result.span()[0]] + numword + tts_item.text[start + result.span()[1]:]
+            start += result.span()[1] - len_original + len(numword)
+        return tts_item
 
     def _prepare_item(self, tts_item: TTS_Item) -> list[TTS_Item]:
         """
-        Preprocess item in various ways (character replacement, splitting, etc.) and return a list of resulting items
+        Preprocess the given input TTS item by performing character replacement, splitting, and other operations as needed.
+
+        :param tts_item: The input TTS item to preprocess.
+        :type tts_item: TTS_Item
+
+        :return: A list of TTS items resulting from the preprocessing.
+        :rtype: list[TTS_Item]
         """
 
         if tts_item.speaker_idx != -1:
             # try:
             #     speaker_idx = TTS_Arranger.default_speakers.index(tts_item.speaker)
             # except ValueError:
             #     log(LOG_TYPE.ERROR, f'Speaker index "{tts_item.speaker}" is unknown, falling back to default speaker.')
             #     speaker_idx = 0
 
-            # Some tweaks for tts_models/de/thorsten/tacotron2-DDC
             if self.model == 'tts_models/de/thorsten/tacotron2-DDC':
-                str_months = ('Januar', 'Februar', 'März', 'April', 'Mai', 'Juni', 'Juli', 'August', 'September', 'Oktober', 'November', 'Dezember')
-
-                # Ordinal numbers
-                start = 0
-                while result := re.search(r'\b[0-9]+\.', tts_item.text[start:]):
-                    len_original = 0
-                    numword = ''
-                    # When followed by month names
-                    if tts_item.text[start + result.span()[1]:].strip().startswith(str_months):
-                        match = tts_item.text[start + result.span()[0]:start + result.span()[1]]
-                        len_original = len(match)
-                        numword = num2words(match, lang='de', to='ordinal')
-                        tts_item.text = tts_item.text[:start + result.span()[0]] + numword + tts_item.text[start + result.span()[1]:]
-                    start += result.span()[1] - len_original + len(numword)
-
-                # Year numbers
-                start = 0
-                while result := re.search(r'\b[0-9]{4,4}\b', tts_item.text[start:]):
-                    len_original = 0
-                    numword = ''
-                    # When followed by month names
-                    if tts_item.text[:start + result.span()[0]].strip().endswith(('Jahr', 'in', 'vor', 'nach') + str_months):
-                        match = tts_item.text[start + result.span()[0]:start + result.span()[1]]
-
-                        if int(match) < 2000:
-                            len_original = len(match)
-                            numword = num2words(match, lang='de', to='year')
-                            tts_item.text = tts_item.text[:start + result.span()[0]] + numword + tts_item.text[start + result.span()[1]:]
-                    start += result.span()[1] - len_original + len(numword)
-
-            # Some general preprocessing
+                tts_item = self._de_thorsten_tacotron2_DDC_tweaks(tts_item)
 
+            # General preprocessing
             text = tts_item.text
 
             # Remove Japanese characters etc.
             text = ''.join(filter(lambda character: ord(character) < 0x3000, text))
 
             # Replace problematic characters, abbreviations etc
             for k, v in self.replace.items():
                 text = re.sub(k, v, text)
 
             tts_item.text = text
 
             tts_items = [tts_item]
 
-            tts_items = self._break_single(tts_items, r'\n', pause_post=self.pause_newline)
-            tts_items = self._break_single(tts_items, r'[;:]\s', pause_post=self.pause_colon)
-            tts_items = self._break_single(tts_items, r'[—–]', pause_post=self.pause_dash)
+            tts_items = self._break_single(tts_items, r'\n', pause_post_ms=self.pause_newline)
+            tts_items = self._break_single(tts_items, r'[;:]\s', pause_post_ms=self.pause_colon)
+            tts_items = self._break_single(tts_items, r'[—–]', pause_post_ms=self.pause_dash)
             # tts_items = self._break_single(tts_items, r'[\.!\?]\s', keep=True)
             # tts_items = self.break_single(tts_items, '…')
 
             # Break items if too long (memory consumption)
             # TODO: disabled for now as recent versions of TTS don’t seem to leak memory that much
             # tts_items = self.find_and_break(tts_items, [
             #                                 '. ', '! ', '? ', ': ', ';', ') ', '] ', '} ', ', ', ' '], self.max_chars)
@@ -261,17 +234,17 @@
             #     tts_items = self.break_speakers(tts_items, ('‘', '’'), True, pause_pre=100, pause_post=100)
             #     tts_items = self.break_speakers(tts_items, ('„', '“'), True, pause_pre=100, pause_post=100)
             #     tts_items = self.break_speakers(tts_items, ('‚', '‘'), True, pause_pre=100, pause_post=100)
             #     tts_items = self.break_speakers(tts_items, ('»', '«'), True, pause_pre=100, pause_post=100)
             #     tts_items = self.break_speakers(tts_items, ('«', '»'), True, pause_pre=100, pause_post=100)
             #     tts_items = self.break_speakers(tts_items, ('"', '"'), True, pause_pre=100, pause_post=100)
 
-            tts_items = self._break_items(tts_items, ('(', ')'), pause_pre=self.pause_parentheses, pause_post=self.pause_parentheses)
-            tts_items = self._break_items(tts_items, ('—', '—'), pause_pre=self.pause_parentheses, pause_post=self.pause_parentheses)
-            tts_items = self._break_items(tts_items, ('– ', ' –'), pause_pre=self.pause_parentheses, pause_post=self.pause_parentheses)
+            tts_items = self._break_items(tts_items, ('(', ')'), pause_pre_ms=self.pause_parentheses, pause_post_ms=self.pause_parentheses)
+            tts_items = self._break_items(tts_items, ('—', '—'), pause_pre_ms=self.pause_parentheses, pause_post_ms=self.pause_parentheses)
+            tts_items = self._break_items(tts_items, ('– ', ' –'), pause_pre_ms=self.pause_parentheses, pause_post_ms=self.pause_parentheses)
             # tts_items = self.break_start_end(tts_items, ('- ', ' -'), pause_pre=300, pause_post=300)
             # tts_items = self.break_start_end(tts_items, (r'\s[-–—]-?\s', r'\s[-–—]-?\s'), pause_post=150)
             # tts_items = self.break_start_end(tts_items, (r'\(', r'\)'), pause_post=150)
             tts_items = self._break_items(tts_items, ('*', '*'))
 
             final_items = []
 
@@ -284,15 +257,15 @@
                 # text = re.sub(r'([\.\?\!;:]) ', r'\1\n', text)
                 text = re.sub(r'[–—]', r'-', text)
                 text = re.sub(r'[„“”]', r'"', text)
                 text = re.sub(r'[‘’]', r"'", text)
 
                 # Remove all remaining punctuation after first occurrence
                 # text = re.sub(r'([\.\?\!;:])\s?[\.\?\!;:,\)\"\'.\]]+', r'\1', text)
-                text = self._minimize_tailing_punctuation(text)
+                text = text.rstrip(string.punctuation + ' ')
 
                 # Strip starting punctuation and normalize ending punctuation
                 text = text.strip().lstrip(string.punctuation).strip()
 
                 if self.model != 'tts_models/en/vctk/vits':
                     # Add a full stop if necessary to avoid synthesizing problems with some models
                     text = re.sub(r'([a-zA-Z0-9])$', r'\1.', text)
@@ -311,17 +284,32 @@
             #     tts_items[-1].properties.pause_pre += pause_pre
             #     tts_items[-1].properties.pause_post += pause_post
         else:
             final_items = [tts_item]
 
         return final_items
 
-    def _break_single(self, tts_items: list[TTS_Item], break_at: str, keep: bool = False, pause_post: int = 0) -> list[TTS_Item]:
+    def _break_single(self, tts_items: list[TTS_Item], break_at: str, keep: bool = False, pause_post_ms: int = 0) -> list[TTS_Item]:
         """
-        Break item at specific single character
+        Break the given list of input TTS items at the specified single character and return a list of resulting input TTS items.
+
+        :param tts_items: The list of input TTS items to break.
+        :type tts_items: list[TTS_Item]
+
+        :param break_at: The single character at which to break the input TTS items.
+        :type break_at: str
+
+        :param keep: Whether to keep the breaking character in the resulting TTS items. Default is False.
+        :type keep: bool
+
+        :param pause_post: The duration of a pause (in ms) to insert after each broken TTS item. Default is 0.
+        :type pause_post: int
+
+        :return: A list of TTS items resulting from the breaking.
+        :rtype: list[TTS_Item]
         """
         final_items = []
 
         for tts_item in tts_items:
             text = tts_item.text
 
             if not text and tts_item.length > 0:
@@ -339,44 +327,66 @@
 
                     item_text = text[m.start():m.end() - length]
 
                     if item_text:
 
                         # From last group to end of current group
                         final_items.append(TTS_Item(item_text, tts_item.speaker, tts_item.speaker_idx, tts_item.length))
-                        if pause_post > 0:
-                            final_items.append(TTS_Item(length=pause_post))
+                        if pause_post_ms > 0:
+                            final_items.append(TTS_Item(length=pause_post_ms))
                         last_start = m.end()
 
                 # From end of last group to end of text
                 text = text[last_start:].strip()
 
                 if text:
                     final_items.append(TTS_Item(text, tts_item.speaker, tts_item.speaker_idx, tts_item.length))
 
         return final_items
 
     def _get_character(self, text: str, pos: int) -> str:
         """
-        Get character at a specific position in a string
-        """
-        character = ''
+        Get the character at the specified position in the given string and return it as a string.
+
+        :param text: The string to get the character from.
+        :type text: str
 
-        if pos > 0 and pos < len(text):
-            character = text[pos]
-        return character
+        :param pos: The position of the character to get.
+        :type pos: int
 
-    def _break_items(self, tts_items: list[TTS_Item], start_end: tuple = (), pause_pre: int = 0, pause_post: int = 0) -> list[TTS_Item]:
+        :return: The character at the specified position, or an empty string if the position is out of bounds.
+        :rtype: str
         """
-        Break items in list of items based on opening and closing characters (like parenthesis) and return new list
+        if 0 <= pos < len(text):
+            return text[pos]
+        return ''
+
+    def _break_items(self, tts_items: list[TTS_Item], start_end: tuple = (), pause_pre_ms: int = 0, pause_post_ms: int = 0) -> list[TTS_Item]:
+        """
+        Break items in a list of TTS items based on opening and closing characters (like parenthesis) and return a new list.
+
+        :param tts_items: A list of TTS items to be broken down.
+        :type tts_items: list[TTS_Item]
+
+        :param start_end: A tuple of the opening and closing characters used to break down the items, defaults to ().
+        :type start_end: tuple[int, int]
+
+        :param pause_pre_ms: The duration of a pause (in ms) to be inserted before the opening character, defaults to 0.
+        :type pause_pre_ms: int
+
+        :param pause_post_ms: The duration of a pause (in ms) to be inserted after the closing character, defaults to 0.
+        :type pause_post_ms: int
+
+        :return: A new list of TTS items that have been broken down based on the specified opening and closing characters.
+        :rtype: list[TTS_Item]
         """
         final_items = []
 
         if tts_items:
-            lenght = len(start_end[0])
+            length = len(start_end[0])
 
             opened = False
             current_speaker = ''
             current_speaker_idx = 0
 
             for tts_item in tts_items:
                 pos = 0
@@ -415,34 +425,34 @@
                                     add_item = True
                                     # print(f'Close')
                         elif c in ['.', ',', ';', ':']:
                             # Attach closing punctuation to last text segment
                             if pos == idx:
                                 if len(final_items) > 0:
                                     final_items[-1].text += c
-                                    pos += lenght
+                                    pos += length
                     else:
                         # If open and closing pattern are not the same
                         if c == start_end[0]:
                             if self._get_character(tts_item.text, idx - 1) in string.punctuation + ' ':
                                 add_item = True
                                 # print(f'Open')
                         elif c == start_end[1]:
                             if self._get_character(tts_item.text, idx + 1) in string.punctuation + ' ':
                                 add_item = True
 
-                                if pause_pre > 0:
-                                    final_items.append(TTS_Item(length=pause_pre))
+                                if pause_pre_ms > 0:
+                                    final_items.append(TTS_Item(length=pause_pre_ms))
 
                                 # print(f'Close')
                         elif c in ['.', ',', ';', ':']:
                             if pos == idx:
                                 if len(final_items) > 0:
                                     final_items[-1].text += c
-                                    pos += lenght
+                                    pos += length
 
                     if add_item:
                         # Add item resulting from breaking
                         if new_item.text:
                             # if len(final_items) > 0:
                             #     if pause_pre > 0:
                             #         final_items.append(TTS_Item(length=pause_pre))
@@ -453,16 +463,16 @@
                             #     if pause_post > 0:
                             #         final_items.append(TTS_Item(length=pause_post))
                             # print(f'Adding item after breaking: {new_item.text} / {new_item.speaker}')
                         pos = idx + 1
                         found = add_item
 
                 if found:
-                    if pause_post > 0:
-                        final_items.append(TTS_Item(length=pause_post))
+                    if pause_post_ms > 0:
+                        final_items.append(TTS_Item(length=pause_post_ms))
 
                 # Add rest / regular item
                 new_item = copy.copy(tts_item)
                 new_item.text = tts_item.text[pos:].strip()
                 new_item.speaker = current_speaker
                 new_item.speaker_idx = current_speaker_idx
                 new_item.length = tts_item.length
@@ -471,27 +481,39 @@
                     # print(f'Adding regular item: {new_item.text} / {new_item.speaker}')
                     final_items.append(new_item)
 
         return final_items
 
     def preprocess_items(self, tts_items: list[TTS_Item]) -> list[TTS_Item]:
         """
-        Preprocess items
+        Preprocesses a list of TTS items.
+
+        :param tts_items: A list of TTS items to be preprocessed.
+        :type tts_items: list[TTS_Item]
+
+        :return: A new list of preprocessed TTS items.
+        :rtype: list[TTS_Item]
         """
         final_items = []
         merged_items = self._merge_similar_items(tts_items)
 
         for tts_item in merged_items:
             final_items += self._prepare_item(tts_item)
 
         return final_items
 
     def _merge_similar_items(self, items=[]) -> list:
         """
         Merge similar items for smoother synthesizing and avoiding unwanted pauses
+
+        :param items: A list of TTS items to merge
+        :type items: list
+
+        :return: A list of merged TTS items
+        :rtype: list
         """
         final_items: list[TTS_Item] = []
 
         if items:
             start_item = -1
             merged_item = TTS_Item()
 
@@ -527,18 +549,25 @@
 
         return final_items
 
     def synthesize_and_write(self, tts_items: list[TTS_Item], output_filename: str, callback: Callable[[int, int], None] | None = None):
         """
         Synthesize and write list of items as an audio file
 
-        Args:
-            tts_items (list[TTS_Item]): List of items to be synthesized
-            output_filename (str): Absolute path and filename of output audio file including file type extension (for example mp3, ogg)
-            callback (function): Reference to function to be called after synthesizing of an item if finished, parameters: index (int), total number of items (int)
+        :param tts_items: List of TTS items to be synthesized
+        :type tts_items: list
+
+        :param output_filename: Absolute path and filename of output audio file including file type extension (for example mp3, ogg)
+        :type output_filename: str
+
+        :param callback: Reference to function to be called after synthesizing of an item is finished
+        :type callback: function
+
+        :return: None
+        :rtype: None
         """
         time_total = 0.0
         time_needed = 0.0
 
         characters_sum = 0
         characters_total = 0
 
@@ -582,44 +611,42 @@
                 log(LOG_TYPE.ERROR, f'Error synthesizing "{output_filename}": {e}')
                 sys.exit()
 
         self.write(segments, output_filename)
 
     def synthesize_tts_item(self, tts_item: TTS_Item) -> AudioSegment:
         """
-        Synthesize a single item and return a pydub AudioSegment
+        Synthesize a single item and return a PyDub AudioSegment object
+
+        :param tts_item: TTS item to be synthesized
+        :type tts_item: TTS_Item
+
+        :return: AudioSegment object of synthesized audio
+        :rtype: AudioSegment
         """
         segment = AudioSegment.empty()
 
         if tts_item.text:
             try:
                 speaker = ''
 
-                if self.synthesizer.tts_model:
-                    if self.synthesizer.tts_model.num_speakers > 1:
-                        speaker = tts_item.speaker
-
-                        # Use index if no explicit speaker name is given, wrap around speakers to avoid undefined indexes
-                        if not speaker:
-                            speaker = self.speakers[tts_item.speaker_idx % len(self.speakers)]
-
-                            if self.preferred_speakers:
-                                if self.preferred_speakers[tts_item.speaker_idx % len(self.preferred_speakers)] in self.speakers:
-                                    speaker = self.preferred_speakers[tts_item.speaker_idx % len(self.preferred_speakers)]
+                if self.synthesizer.tts_model and self.synthesizer.tts_model.num_speakers > 1:
+                    speaker = tts_item.speaker or self.speakers[tts_item.speaker_idx % len(self.speakers)]
+                    speaker = self.preferred_speakers[tts_item.speaker_idx % len(self.preferred_speakers)] if self.preferred_speakers and speaker in self.speakers else speaker
 
                 # Suppress tts output
                 with contextlib.redirect_stdout(None):
                     wav = self.synthesizer.tts(
                         text=tts_item.text,
                         speaker_name=speaker,
                     )
             except Exception as e:
                 raise Exception(f'Error synthesizing "{tts_item.text}: {e}"')
             else:
-                speech_segment = numpy_to_segment(wav, int(self.synthesizer.output_sample_rate))
+                speech_segment = numpy_to_segment(np.array(wav), int(self.synthesizer.output_sample_rate))
 
                 # If length is predefined, add padding if necessary
                 if int(speech_segment.duration_seconds * 1000) < tts_item.length:
                     speech_segment += AudioSegment.silent(int(tts_item.length - speech_segment.duration_seconds * 1000), int(self.synthesizer.output_sample_rate))
                 else:
                     # Strip some silence away to make pauses easier to control
                     silence = detect_silence(speech_segment, min_silence_len=self.silence_length, silence_thresh=self.silence_threshold)
@@ -634,14 +661,23 @@
                 segment += AudioSegment.silent(tts_item.length, int(self.synthesizer.output_sample_rate))
 
         return segment
 
     def write(self, segment: AudioSegment, output_filename: str) -> None:
         """
         Compress, convert and write AudioSegment as a given output file path and name
+
+        :param segment: AudioSegment to be written
+        :type segment: AudioSegment
+
+        :param output_filename: Absolute path and filename of output audio file including file type extension (for example mp3, ogg)
+        :type output_filename: str
+
+        :return: None
+        :rtype: None
         """
         # Clean up to free up some memory
         # self.synthesizer = None
         # gc.collect()
 
         # Set default format to mp3
         format = os.path.splitext(output_filename)[1][1:] or 'mp3'
```

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/__future__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/__future__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ast.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_csv.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_csv.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_thread.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_thread.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/abc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/abc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/array.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/array.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ast.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ast.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ast.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ast.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/builtins.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/codecs.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/copy.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/copy.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/copy.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/copy.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/csv.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/csv.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/csv.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/csv.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/datetime.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/enum.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/enum.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/io.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/io.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/math.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/math.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/math.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/math.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/mmap.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pickle.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/re.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/re.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/string.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/string.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/string.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/string.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sys.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/sys.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/threading.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/threading.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/threading.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/threading.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/time.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/time.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/types.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/types.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/warnings.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/warnings.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/header.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/message.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/path.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json` & `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/tests/tts_arranger_test.py` & `tts_arranger-0.0.5/tests/tts_arranger_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,134 +1,134 @@
 import unittest
 
-from tts_arranger import TTS_Arranger, TTS_Item
+from tts_arranger import TTS_Processor, TTS_Item
 
 
 class Test(unittest.TestCase):
     def test_break1(self):
-        t = TTS_Arranger(multi=True)
+        t = TTS_Processor()
 
         tts_item = TTS_Item('This. Is: A t:est!', 'p330')
 
         tts_items = t._prepare_item(tts_item)
 
         self.assertEqual(tts_items[0].text, 'This. Is')
         self.assertEqual(tts_items[1].length, 150)
         self.assertEqual(tts_items[2].text, 'A t:est!')
         self.assertEqual(tts_items[3].length, 1000)
 
     # def test_break2(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_item = TTS_Item('This “Is” a test, right?', 'test', 10, 10, True)
 
     #     tts_items = t._prepare_item(tts_item)
 
     #     self.assertEqual(tts_items[0].text, 'This')
     #     self.assertEqual(tts_items[1].text, 'Is')
     #     self.assertEqual(tts_items[2].text, 'a test, right?')
 
     # def test_break3(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     text = '''In this rough theatre of teeming peoples and conflicting cultures were developed the agriculture and commerce, the horse and wagon, the coinage and letters of credit, the crafts and industries, the law and government, the mathematics and medicine, the enemas and drainage systems, the geometry and astronomy, the calendar and clock and zodiac, the alphabet and writing, the paper and ink, the books and libraries and schools, the literature and music, the sculpture and architecture, the glazed pottery and fine furniture, the monotheism and monogamy, the cosmetics and jewelry, the checkers and dice, the ten-pins and income tax, the wet-nurses and beer, from which our own European and American culture derive by a continuous succession through the mediation of Crete and Greece and Rome.'''
 
     #     tts_item = TTS_Item(text, 'test', 10, 10, True)
 
     #     tts_items = t.prepare_item(tts_item)
 
     #     self.assertEqual(tts_items[0].text, 'In this rough theatre of teeming peoples and conflicting cultures were developed the agriculture and commerce, the horse and wagon, the coinage and letters of credit, the crafts and industries, the law and government, the mathematics and medicine, the enemas and drainage systems, the geometry and astronomy')
     #     self.assertEqual(tts_items[1].text, 'the calendar and clock and zodiac, the alphabet and writing, the paper and ink, the books and libraries and schools, the literature and music, the sculpture and architecture, the glazed pottery and fine furniture, the monotheism and monogamy, the cosmetics and jewelry, the checkers and dice')
     #     self.assertEqual(
     #         tts_items[2].text, 'the ten-pins and income tax, the wet-nurses and beer, from which our own European and American culture derive by a continuous succession through the mediation of Crete and Greece and Rome.')
 
     # def test_break4(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_item = TTS_Item('LoremipsumdolorsitametconsecteturadipiscingelitseddoeiusmodtemporincididuntutlaboreetdoloremagnaaliquaUtenimadminimveniamquisnostrudexercitationullamcolaborisnisiutaliquipexeacommodoconsequatduisauteiruredolorinreprehenderitinvoluptatevelitessecillumdoloreeufugiatnullapariaturexcepteursintoccaecatcupidatatnonproidentsuntinculpaquiofficiadeseruntmollitanimidestlaborum.', 'test', 10, 10, True)
 
     #     tts_items = t.prepare_item(tts_item)
 
     #     self.assertEqual(tts_items[0].text, 'LoremipsumdolorsitametconsecteturadipiscingelitseddoeiusmodtemporincididuntutlaboreetdoloremagnaaliquaUtenimadminimveniamquisnostrudexercitationullamcolaborisnisiutaliquipexeacommodoconsequatduisauteiruredolorinreprehenderitinvoluptatevelitessecillumdoloreeufugiatnullapariaturexcepteursintoccaecatcupidatatnonproidentsu')
     #     self.assertEqual(
     #         tts_items[1].text, 'ntinculpaquiofficiadeseruntmollitanimidestlaborum.')
 
     def test_url(self):
-        t = TTS_Arranger()
+        t = TTS_Processor()
 
         tts_item = TTS_Item('https://stackoverflow.com/questions/17730788/search-and-replace-with-whole-word-only-option', '')
 
         tts_items = t._prepare_item(tts_item)
         self.assertEqual(tts_items[0].text, 'stackoverflow.com')
 
     def test_endings(self):
-        t = TTS_Arranger()
+        t = TTS_Processor()
 
         tts_item = TTS_Item('''Lovely story!
 Do you mean pidgin Danish, perhaps? :''', '')
 
         tts_items = t._prepare_item(tts_item)
         self.assertEqual(tts_items[0].text, 'Lovely story!')
         self.assertEqual(tts_items[1].length, 1000)
         self.assertEqual(tts_items[2].length, 250)
         self.assertEqual(tts_items[3].text, 'Do you mean pidgin Danish, perhaps?')
         self.assertEqual(tts_items[4].length, 1000)
 
     # def test_punctuation1(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_item = TTS_Item('Sure, these were all hoary old tropes even by the late ’70s/early ’80s, but this particular combination of them, at this exact date…? Even the “silly but kind of grim” atmosphere that you correctly mention the game possessing is the exact way I would describe “Night Horrors”.', '')
 
     #     tts_items = t._prepare_item(tts_item)
     #     self.assertEqual(tts_items[0].text, 'Sure, these were all hoary old tropes even by the late \'70s/early \'80s, but this particular combination of them, at this exact date?')
     #     self.assertEqual(tts_items[1].text, 'Even the')
     #     self.assertEqual(tts_items[2].text, 'silly but kind of grim')
     #     self.assertEqual(tts_items[3].text, 'atmosphere that you correctly mention the game possessing is the exact way I would describe')
     #     self.assertEqual(tts_items[4].text, 'Night Horrors.')
 
     def test_punctuation2(self):
-        t = TTS_Arranger(multi=True)
+        t = TTS_Processor()
 
         tts_item = TTS_Item('Specifically, he wanted to bring FORTRAN, as it happens the implementation language of the original Adventure (not that Ken likely knew this or cared), to the little Apple II.', '')
 
         tts_items = t._prepare_item(tts_item)
         self.assertEqual(tts_items[0].text, 'Specifically, he wanted to bring FORTRAN, as it happens the implementation language of the original Adventure')
         self.assertEqual(tts_items[1].length, 300)
         self.assertEqual(tts_items[2].text, 'not that Ken likely knew this or cared,')
         self.assertEqual(tts_items[3].length, 300)
         self.assertEqual(tts_items[4].text, 'to the little Apple 2.')
         self.assertEqual(tts_items[5].length, 750)
 
     def test_punctuation3(self):
-        t = TTS_Arranger(multi=True)
+        t = TTS_Processor()
 
         tts_item = TTS_Item('a — b.', '')
 
         tts_items = t._prepare_item(tts_item)
         self.assertEqual(tts_items[0].text, 'a')
         self.assertEqual(tts_items[1].length, 300)
         self.assertEqual(tts_items[2].text, 'b.')
         self.assertEqual(tts_items[3].length, 750)
 
     # def test_punctuation3(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_item = TTS_Item('Much of what led to designs like The Wizard and the Princess — the lack of understood “best practices” for game design, primitive technology, the simple inexperience of the designers themselves — I’ve already mentioned here and elsewhere. Certainly, as I’ve particularly harped, it was difficult with a Scott Adams- or Hi-Res-Adventures-level parser and world model to find a ground for challenging puzzles that were not unfair; the leap from trivial to impossible being made in one seemingly innocuous hop, as it were.', '')
 
     #     tts_items = t._prepare_item(tts_item)
     #     self.assertEqual(tts_items[0].text, 'Much of what led to designs like The Wizard and the Princess')
     #     self.assertEqual(tts_items[1].text, 'the lack of understood')
     #     self.assertEqual(tts_items[2].text, 'best practices')
     #     self.assertEqual(tts_items[3].text, 'for game design, primitive technology, the simple inexperience of the designers themselves')
     #     self.assertEqual(tts_items[4].text, 'I\'ve already mentioned here and elsewhere.')
     #     self.assertEqual(tts_items[5].text, 'Certainly, as I\'ve particularly harped, it was difficult with a Scott Adams- or Hi-Res-Adventures-level parser and world model to find a ground for challenging puzzles that were not unfair')
     #     self.assertEqual(tts_items[6].text, 'the leap from trivial to impossible being made in one seemingly innocuous hop, as it were.')
 
     # def test_start_end(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_item = TTS_Item(
     #         '“In ASCII “A” numerically follows “B” which follows “C,” etc.”.')
 
     #     # tts_items = t.break_start_end([tts_item], ('“', '”'), True)
     #     tts_items = t.break_speakers([tts_item], ('“', '”'), True)
 
@@ -146,29 +146,29 @@
     #     # self.assertEqual(tts_items[5].speaker, t.default_speakers[2])
     #     self.assertEqual(tts_items[6].text, 'etc..')
     #     # self.assertEqual(tts_items[6].speaker, t.default_speakers[1])
     #     # self.assertEqual(tts_items[7].text, '.')
     #     # self.assertEqual(tts_items[7].speaker, t.default_speakers[0])
 
     # def test_quotes2(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_item = TTS_Item('"This" is a "test".')
 
     #     tts_items = t.break_speakers([tts_item], ('"', '"'), True)
 
     #     self.assertEqual(tts_items[0].text, 'This')
     #     # self.assertEqual(tts_items[0].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[1].text, 'is a')
     #     # self.assertEqual(tts_items[1].speaker, t.default_speakers[0])
     #     self.assertEqual(tts_items[2].text, 'test.')
     #     # self.assertEqual(tts_items[2].speaker, t.default_speakers[1])
 
     # def test_new_break(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_items = [TTS_Item('Hello, “This” is a “test”.', t.default_speakers[0]),
     #                  TTS_Item('“And this is another test.”', t.default_speakers[0])]
 
     #     tts_items = t.break_speakers(tts_items, ('“', '”'), True)
 
     #     self.assertEqual(tts_items[0].text, 'Hello,')
@@ -179,15 +179,15 @@
     #     # self.assertEqual(tts_items[2].speaker, t.default_speakers[0])
     #     self.assertEqual(tts_items[3].text, 'test.')
     #     # self.assertEqual(tts_items[3].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[4].text, 'And this is another test.')
     #     # self.assertEqual(tts_items[4].speaker, t.default_speakers[1])
 
     # def test_start_end2(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_items = []
 
     #     tts_items.append(TTS_Item('Test abc “hallo test', ''))
     #     tts_items.append(TTS_Item('continued test” something.', ''))
 
     #     # tts_items = t.break_start_end([tts_item], ('“', '”'), True)
@@ -199,15 +199,15 @@
     #     # self.assertEqual(tts_items[1].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[2].text, 'continued test')
     #     # self.assertEqual(tts_items[2].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[3].text, 'something.')
     #     # self.assertEqual(tts_items[3].speaker, t.default_speakers[0])
 
     # def test_new_break2(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_items = [TTS_Item('Hello, "This" is a "test".', t.default_speakers[0]),
     #                  TTS_Item('"And this is another test."', t.default_speakers[0])]
 
     #     tts_items = t.break_speakers(tts_items, ('"', '"'), True)
 
     #     self.assertEqual(tts_items[0].text, 'Hello,')
@@ -218,69 +218,69 @@
     #     # self.assertEqual(tts_items[2].speaker, t.default_speakers[0])
     #     self.assertEqual(tts_items[3].text, 'test.')
     #     # self.assertEqual(tts_items[3].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[4].text, 'And this is another test.')
     #     # self.assertEqual(tts_items[4].speaker, t.default_speakers[1])
 
     # def test_new_break3(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_items = [TTS_Item('"I’m a “test. ‘This as well’”."', t.default_speakers[0])]
 
     #     tts_items = t._prepare_item(tts_items[0])
 
     #     self.assertEqual(tts_items[0].text, 'I\'m a')
     #     # self.assertEqual(tts_items[0].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[1].text, 'test.')
     #     # self.assertEqual(tts_items[1].speaker, t.default_speakers[2])
     #     self.assertEqual(tts_items[2].text, 'This as well.')
     #     # self.assertEqual(tts_items[2].speaker, t.default_speakers[3])
 
     # def test_new_break_a1(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_items = [TTS_Item('a', t.default_speakers[0]), TTS_Item('"b"', t.default_speakers[0]), TTS_Item('"c"', t.default_speakers[0])]
 
     #     tts_items = t.break_speakers(tts_items, ('"', '"'), True)
 
     #     self.assertEqual(tts_items[0].text, 'a')
     #     # self.assertEqual(tts_items[0].speaker, t.default_speakers[0])
     #     self.assertEqual(tts_items[1].text, 'b')
     #     # self.assertEqual(tts_items[1].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[2].text, 'c')
     #     # self.assertEqual(tts_items[2].speaker, t.default_speakers[1])
 
     # def test_new_break_a2(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_items = [TTS_Item('a', t.default_speakers[1]), TTS_Item('"b"', t.default_speakers[1]), TTS_Item('"c"', t.default_speakers[1])]
 
     #     tts_items = t.break_speakers(tts_items, ('"', '"'), True)
 
     #     self.assertEqual(tts_items[0].text, 'a')
     #     # self.assertEqual(tts_items[0].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[1].text, 'b')
     #     # self.assertEqual(tts_items[1].speaker, t.default_speakers[2])
     #     self.assertEqual(tts_items[2].text, 'c')
     #     # self.assertEqual(tts_items[2].speaker, t.default_speakers[2])
 
     # def test_new_break_a3(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_items = [TTS_Item('“‘"Test1."’”')]
 
     #     tts_items = t.break_speakers(tts_items, ('“', '”'), True)
     #     tts_items = t.break_speakers(tts_items, ('‘', '’'), True)
     #     tts_items = t.break_speakers(tts_items, ('"', '"'), True)
 
     #     self.assertEqual(tts_items[0].text, 'Test1.')
     #     # self.assertEqual(tts_items[0].speaker, t.default_speakers[3])
 
     # def test_new_break_a4(self):
-    #     t = TTS_Arranger(multi=True)
+    #     t = TTS_Arranger()
 
     #     tts_items = [TTS_Item('a'),
     #                  TTS_Item('“b'),
     #                  TTS_Item('c”')]
 
     #     tts_items = t.break_speakers(tts_items, ('“', '”'), True)
     #     # tts_items = t.break_speakers(tts_items, ('‘', '’'), True)
@@ -290,26 +290,26 @@
     #     # self.assertEqual(tts_items[0].speaker, t.default_speakers[0])
     #     self.assertEqual(tts_items[1].text, 'b')
     #     # self.assertEqual(tts_items[1].speaker, t.default_speakers[1])
     #     self.assertEqual(tts_items[2].text, 'c')
     #     # self.assertEqual(tts_items[2].speaker, t.default_speakers[1])
 
     def test_new_break_a5(self):
-        t = TTS_Arranger(multi=True)
+        t = TTS_Processor()
 
         tts_item = TTS_Item('sic!].')
 
         tts_items = t._prepare_item(tts_item)
         # tts_items = t.break_speakers(tts_items, ('‘', '’'), True)
         # tts_items = t.break_speakers(tts_items, ('"', '"'), True)
 
         self.assertEqual(tts_items[0].text, 'sic!')
 
     def test_new_break_a6(self):
-        t = TTS_Arranger(multi=True)
+        t = TTS_Processor()
 
         tts_item = TTS_Item('candle- ?, ?')
 
         tts_items = t._prepare_item(tts_item)
         # tts_items = t.break_speakers(tts_items, ('‘', '’'), True)
         # tts_items = t.break_speakers(tts_items, ('"', '"'), True)
```

### Comparing `tts_arranger-0.0.4/LICENSE` & `tts_arranger-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/README.md` & `tts_arranger-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.4/pyproject.toml` & `tts_arranger-0.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.0.4"
+version = "0.0.5"
 
 dependencies = [
   "numpy>=1.22.4",
   "pydub>=0.25.1",
   "scipy>=1.9.0",
-  "TTS>=0.10.2",
-  "num2words>=0.5.11"
+  "TTS>=0.13.0",
+  "num2words>=0.5.11",
 ]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
```

### Comparing `tts_arranger-0.0.4/PKG-INFO` & `tts_arranger-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: num2words>=0.5.11
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: pydub>=0.25.1
 Requires-Dist: scipy>=1.9.0
-Requires-Dist: tts>=0.10.2
+Requires-Dist: tts>=0.13.0
 Description-Content-Type: text/markdown
 
 # TTS Arranger
 
 Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS.
 
 # Example
```

