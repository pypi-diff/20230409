# Comparing `tmp/borg_space-0.4.0.tar.gz` & `tmp/borg_space-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borg_space-0.4.0.tar", last modified: Sun Oct 23 02:46:34 2022, max compression
+gzip compressed data, was "borg_space-1.0.tar", last modified: Sun Apr  9 05:02:50 2023, max compression
```

## Comparing `borg_space-0.4.0.tar` & `borg_space-1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2022-10-22 21:26:19.370225 borg_space-0.4.0/LICENSE
--rw-r--r--   0        0        0     4203 2022-10-23 02:39:49.068396 borg_space-0.4.0/README.rst
--rwxr-xr-x   0        0        0     6500 2022-10-23 02:39:49.066397 borg_space-0.4.0/borg_space.py
--rw-r--r--   0        0        0     1195 2022-10-23 02:39:49.064396 borg_space-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5269 1970-01-01 00:00:00.000000 borg_space-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-22 21:26:19.370225 borg_space-1.0/LICENSE
+-rw-r--r--   0        0        0     3693 2023-04-09 04:39:15.072813 borg_space-1.0/README.rst
+-rwxr-xr-x   0        0        0     6651 2023-04-09 04:38:00.405766 borg_space-1.0/borg_space.py
+-rw-r--r--   0        0        0     1362 2023-04-09 04:47:40.123167 borg_space-1.0/pyproject.toml
+-rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 borg_space-1.0/PKG-INFO
```

### Comparing `borg_space-0.4.0/LICENSE` & `borg_space-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `borg_space-0.4.0/README.rst` & `borg_space-1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 .. image:: https://img.shields.io/pypi/v/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space
 
 .. image:: https://img.shields.io/pypi/pyversions/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space/
 
 :Author: Ken Kundert
-:Version: 0.4.0
-:Released: 2022-10-22
+:Version: 1.0
+:Released: 2023-04-08
 
 *Borg-Space* is an accessory for `Emborg <https://emborg.readthedocs.io>`_.  It
 reports on the space consumed by your *BorgBackup* repositories.  You can get
 this information using the ``emborg info`` command, but there are several
 reasons to prefer *Borg-Space*.  First, the *info* command gives a great deal of
 information, whereas *Borg-Space* only reports the space consumed by the
 repository, so is much more compact.  Second, the output message is user
@@ -101,41 +101,7 @@
 
 Installation
 ------------
 
 Install with::
 
     > pip3 install --user borg-space
-
-
-Releases
---------
-
-Latest development release
-..........................
-| Version: 0.4.0
-| Released: 2022-10-22
-
-
-0.4.0 (2022-10-22)
-..................
-- Tweak graph axes labels.
-
-
-0.3.0 (2022-03-21)
-..................
-- Upgrade required to support *Emborg* version 1.31.
-
-
-0.2.0 (2021-10-01)
-..................
-- Fixed incompatibility with *Emborg* version 1.26.
-
-
-0.1.0 (2021-09-30)
-..................
-- Added ability to save graph as SVG file.
-
-
-0.0.0 (2021-09-25)
-..................
-- Initial release
```

### Comparing `borg_space-0.4.0/borg_space.py` & `borg_space-1.0/borg_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,42 +12,43 @@
 Options:
     -r, --record                save the result
     -q, --quiet                 do not output the size message
     -m <msg>, --message <msg>   the size message
     -g, --graph                 graph the previously recorded sizes over time
     -l, --log-y                 use a logarithmic Y-axis when graphing
     -s <file>, --svg <file>     produce plot as SVG file rather than display it
+    -n, --narrate               narrate the run
 
 Results are saved to ~/.local/share/emborg/<config>-sizes.nt.
 <msg> may contain {size}, which is replaced with the measured size, and 
 {config}, which is replaced by the config name.
 If no replacements are made, size is appended to the end of the message.
 """
 
 # imports {{{1
 import arrow
 from appdirs import user_data_dir
 from docopt import docopt
 from emborg import Emborg
-from inform import Error, display, error, os_error
+from inform import Inform, Error, display, error, os_error
 from pathlib import Path
 from quantiphy import Quantity
 import json
 import nestedtext as nt
 import matplotlib
 import matplotlib.pyplot as plt
-from matplotlib.dates import DateFormatter
+from matplotlib.dates import AutoDateFormatter, AutoDateLocator
 from matplotlib.ticker import FuncFormatter
 
 # globals {{{1
 data_dir = Path(user_data_dir('emborg'))
 now = str(arrow.now())
 Quantity.set_prefs(prec=2)
-__version__ = "0.4.0"
-__released__ = "2022-10-22"
+__version__ = "1.0"
+__released__ = "2023-04-08"
 
 # generate_graph() {{{1
 def generate_graph(requests, svg_file, log_scale):
     configs = []
     if svg_file:
         matplotlib.use('SVG')
 
@@ -72,15 +73,17 @@
     # create and configure the canvas {{{3
     fig = plt.figure()
     ax = fig.add_subplot(111)
     if log_scale:
         ax.set_yscale('log')
 
     # configure the axis labeling {{{3
-    ax.xaxis.set_major_formatter(DateFormatter('%b %g'))
+    locator = AutoDateLocator()
+    ax.xaxis.set_major_locator(locator)
+    ax.xaxis.set_major_formatter(AutoDateFormatter(locator))
 
     # add traces in order of last size, largest to smallest {{{3
     largest = 0
     smallest = 1e100
     for entry in sorted(traces, key=lambda d: d[1], reverse=True):
         name, last_size, dates, sizes = entry
         largest = max(largest, *sizes)
```

### Comparing `borg_space-0.4.0/pyproject.toml` & `borg_space-1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "borg_space"
 dist-name = "borg-space"
-version = "0.4.0"
+version = "1.0"
 description = "Accessory for Emborg used to report and track the size of your Borg repositories"
 readme = "README.rst"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 keywords = ["emborg", "borg", "backups"]
 authors = [{name = "Ken Kundert", email = "emborg@nurdletech.com"}]
 classifiers = [
@@ -27,16 +27,18 @@
     "inform>=1.26",
     "matplotlib",
     "nestedtext",
     "quantiphy",
 ]
 
 [project.urls]
-homepage = "https://emborg.readthedocs.io"
+homepage = "https://github.com/kenkundert/borg-space"
 repository = "https://github.com/kenkundert/borg-space"
+documentation = "https://github.com/KenKundert/borg-space/blob/master/README.rst"
+changelog = "https://github.com/KenKundert/ntlog/blob/master/CHANGELOG.rst"
 
 [project.scripts]
 borg-space = "borg_space:main"
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `borg_space-0.4.0/PKG-INFO` & `borg_space-1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borg_space
-Version: 0.4.0
+Version: 1.0
 Summary: Accessory for Emborg used to report and track the size of your Borg repositories
 Keywords: emborg,borg,backups
 Author-email: Ken Kundert <emborg@nurdletech.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -19,15 +19,17 @@
 Requires-Dist: arrow>=0.15
 Requires-Dist: docopt
 Requires-Dist: emborg>=1.31
 Requires-Dist: inform>=1.26
 Requires-Dist: matplotlib
 Requires-Dist: nestedtext
 Requires-Dist: quantiphy
-Project-URL: homepage, https://emborg.readthedocs.io
+Project-URL: changelog, https://github.com/KenKundert/ntlog/blob/master/CHANGELOG.rst
+Project-URL: documentation, https://github.com/KenKundert/borg-space/blob/master/README.rst
+Project-URL: homepage, https://github.com/kenkundert/borg-space
 Project-URL: repository, https://github.com/kenkundert/borg-space
 
 Borg-Space — Report and track the size of your Borg repositories
 ================================================================
 
 .. image:: https://pepy.tech/badge/borg-space/month
     :target: https://pepy.tech/project/borg-space
@@ -35,16 +37,16 @@
 .. image:: https://img.shields.io/pypi/v/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space
 
 .. image:: https://img.shields.io/pypi/pyversions/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space/
 
 :Author: Ken Kundert
-:Version: 0.4.0
-:Released: 2022-10-22
+:Version: 1.0
+:Released: 2023-04-08
 
 *Borg-Space* is an accessory for `Emborg <https://emborg.readthedocs.io>`_.  It
 reports on the space consumed by your *BorgBackup* repositories.  You can get
 this information using the ``emborg info`` command, but there are several
 reasons to prefer *Borg-Space*.  First, the *info* command gives a great deal of
 information, whereas *Borg-Space* only reports the space consumed by the
 repository, so is much more compact.  Second, the output message is user
@@ -130,41 +132,7 @@
 Installation
 ------------
 
 Install with::
 
     > pip3 install --user borg-space
 
-
-Releases
---------
-
-Latest development release
-..........................
-| Version: 0.4.0
-| Released: 2022-10-22
-
-
-0.4.0 (2022-10-22)
-..................
-- Tweak graph axes labels.
-
-
-0.3.0 (2022-03-21)
-..................
-- Upgrade required to support *Emborg* version 1.31.
-
-
-0.2.0 (2021-10-01)
-..................
-- Fixed incompatibility with *Emborg* version 1.26.
-
-
-0.1.0 (2021-09-30)
-..................
-- Added ability to save graph as SVG file.
-
-
-0.0.0 (2021-09-25)
-..................
-- Initial release
-
```

