# Comparing `tmp/tts_arranger-0.0.5.tar.gz` & `tmp/tts_arranger-0.0.6.tar.gz`

## Comparing `tts_arranger-0.0.5.tar` & `tts_arranger-0.0.6.tar`

### file list

```diff
@@ -1,681 +1,681 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/requirements.txt
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    30020 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0    12453 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/tts_writer_example.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_csv.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/csv.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/csv.meta.json
--rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json
--rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json
--rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
--rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json
--rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
--rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json
--rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
--rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json
--rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json
--rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json
--rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json
--rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json
--rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/data/replace
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/data/replace_de
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/data/replace_en
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json
--rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json
--rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json
--rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
--rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json
--rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
--rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json
--rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
--rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json
--rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json
--rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json
--rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json
--rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json
--rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json
--rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/LICENSE
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/README.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 tts_arranger-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    30020 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0    12507 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/tts_writer_example.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_csv.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/csv.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/csv.meta.json
+-rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
+-rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json
+-rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json
+-rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
+-rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/data/replace
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/data/replace_de
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/data/replace_en
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json
+-rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
+-rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json
+-rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
+-rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json
+-rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
+-rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0    16954 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/LICENSE
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 tts_arranger-0.0.6/PKG-INFO
```

### Comparing `tts_arranger-0.0.5/src/tts_arranger/tts_processor.py` & `tts_arranger-0.0.6/src/tts_arranger/tts_processor.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.0.6/src/tts_arranger/tts_processor_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/tts_writer.py` & `tts_arranger-0.0.6/src/tts_arranger/tts_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from typing import Callable
 
 import ffmpeg  # type: ignore
 from pathvalidate._filename import sanitize_filename
 from PIL import Image
 from pydub import AudioSegment  # type: ignore
 
-from tts_arranger import TTS_Item, TTS_Processor  # type: ignore
-from tts_arranger.utils.log import LOG_TYPE, bcolors, log  # type: ignore
-
-from .items.tts_chapter import TTS_Chapter
-from .items.tts_project import TTS_Project
+from .items.tts_chapter import TTS_Chapter  # type: ignore
+from .items.tts_item import TTS_Item  # type: ignore
+from .items.tts_project import TTS_Project  # type: ignore
+from .tts_processor import TTS_Processor
+from .utils.log import LOG_TYPE, bcolors, log  # type: ignore
 
 
 class TTS_Writer():
     """
     Class to process TTS projects (containing of chapters each containing a number of items) and to finally write an audio file including chapter metadata and chapter info
     """
 
@@ -100,39 +100,39 @@
             total_items += len(chapter.tts_items)
 
         current_total_items = 0
 
         cumulative_time = 0
 
         for i, chapter in enumerate(chapters):
-            print(f'for {i}, {chapter.title} in enumerate(chapters):')
+            # print(f'for {i}, {chapter.title} in enumerate(chapters):')
             audio = AudioSegment.empty()
 
             temp_format = 'mp4'
 
             if self.output_format != 'm4b':
                 temp_format = 'wav'
 
             filename = temp_dir + '/' + f'tts_part_{i}.{temp_format}'
 
             log(LOG_TYPE.INFO, f'Synthesizing chapter {i + 1} of {len(chapters)}')
 
             for j, tts_item in enumerate(chapter.tts_items):
-                print(f'for {j}, tts_item in enumerate(chapter.tts_items):')
+                # print(f'for {j}, tts_item in enumerate(chapter.tts_items):')
                 if tts_item.text:
                     log(LOG_TYPE.INFO, f'Synthesizing item {j + 1} of {len(chapter.tts_items)} ("{tts_item.speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
                 else:
                     log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC} {tts_item.text}')
 
                 audio += tts_arranger.synthesize_tts_item(tts_item)
 
                 if callback is not None:
                     # callback(i + 1, len(chapters), j + 1, len(chapter.tts_items), chapter.title, current_total_items, total_items)
                     # callback((i * len(chapter.tts_items) + j + 1) / (len(chapters) * len(chapter.tts_items)) * 100)
-                    print(f'callback(100/({len(chapters)} * {len(chapter.tts_items)} * ({i} + {j}), tts_item)')
+                    # print(f'callback(100/({len(chapters)} * {len(chapter.tts_items)} * ({i} + {j}), tts_item)')
                     callback(100/(len(chapters) * len(chapter.tts_items)) * (i + j), tts_item)
 
             current_total_items += len(chapter.tts_items)
 
             tts_arranger.write(audio, filename)
 
             num_zeros = len(str(len(self.temp_files)))
```

### Comparing `tts_arranger-0.0.5/src/tts_arranger/tts_writer_example.py` & `tts_arranger-0.0.6/src/tts_arranger/tts_writer_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from tts_writer import TTS_Writer  # type: ignore
 
 from tts_arranger import TTS_Item  # type: ignore
 
-from .items.tts_chapter import TTS_Chapter
-from .items.tts_project import TTS_Project
+from items.tts_chapter import TTS_Chapter  # type: ignore
+from items.tts_project import TTS_Project  # type: ignore
 
 items1 = []
 items1.append(TTS_Item('This is a test:', speaker_idx=0))
 items1.append(TTS_Item('This is another test:',  speaker_idx=1))
 
 items2 = []
 items2.append(TTS_Item('Another test',  speaker_idx=0))
```

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/__future__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/__future__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ast.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_csv.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_csv.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_thread.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_thread.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/abc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/abc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/array.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/array.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ast.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/ast.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ast.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/ast.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/builtins.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/codecs.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/copy.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/copy.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/copy.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/copy.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/csv.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/csv.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/csv.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/csv.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/datetime.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/enum.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/enum.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/io.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/io.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/math.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/math.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/math.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/math.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/mmap.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pickle.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/re.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/re.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/string.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/string.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/string.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/string.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sys.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/sys.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/threading.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/threading.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/threading.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/threading.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/time.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/time.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/types.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/types.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/warnings.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/warnings.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/header.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/message.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/path.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.0.6/src/tts_arranger/items/tts_chapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass, field
 
 from pydub import AudioSegment  # type: ignore
-from tts_item import TTS_Item  # type: ignore
+
+from .tts_item import TTS_Item  # type: ignore
 
 
 @dataclass
 class TTS_Chapter():
     """
     A data class representing a TTS chapter.
```

### Comparing `tts_arranger-0.0.5/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.0.6/src/tts_arranger/items/tts_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 
 
 @dataclass
-class TTS_Item:
+class TTS_Item():
     """
     Represents a TTS item containing various information.
 
     :param text: The text to be synthesized. Can be left empty in combination with length > 0 to create a pause.
     :type text: str
 
     :param speaker: The name of the speaker to be used.
```

### Comparing `tts_arranger-0.0.5/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.0.6/src/tts_arranger/items/tts_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import datetime
 import pickle
 from dataclasses import dataclass, field
 
-from tts_chapter import TTS_Chapter  # type: ignore
-from tts_item import TTS_Item  # type: ignore
-
 from ..utils.log import LOG_TYPE, log
+from .tts_chapter import TTS_Chapter  # type: ignore
+from .tts_item import TTS_Item  # type: ignore
 
 
 @dataclass
 class TTS_Project():
     """
     A data class representing a text-to-speech project.
```

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/audio.py` & `tts_arranger-0.0.6/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/log.py` & `tts_arranger-0.0.6/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json` & `tts_arranger-0.0.6/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/tests/tts_arranger_test.py` & `tts_arranger-0.0.6/tests/tts_arranger_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 
-from tts_arranger import TTS_Processor, TTS_Item
+from tts_arranger import TTS_Processor
+from tts_arranger.items.tts_item import TTS_Item
 
 
 class Test(unittest.TestCase):
     def test_break1(self):
         t = TTS_Processor()
 
         tts_item = TTS_Item('This. Is: A t:est!', 'p330')
```

### Comparing `tts_arranger-0.0.5/LICENSE` & `tts_arranger-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/README.md` & `tts_arranger-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.5/pyproject.toml` & `tts_arranger-0.0.6/pyproject.toml`

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
-version = "0.0.5"
+version = "0.0.6"
 
 dependencies = [
   "numpy>=1.22.4",
   "pydub>=0.25.1",
   "scipy>=1.9.0",
   "TTS>=0.13.0",
   "num2words>=0.5.11",
```

### Comparing `tts_arranger-0.0.5/PKG-INFO` & `tts_arranger-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

