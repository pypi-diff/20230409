# Comparing `tmp/bintropy-1.3.7.tar.gz` & `tmp/bintropy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bintropy-1.3.7.tar", last modified: Sun Apr  9 10:37:51 2023, max compression
+gzip compressed data, was "bintropy-1.4.0.tar", last modified: Sun Apr  9 20:54:01 2023, max compression
```

## Comparing `bintropy-1.3.7.tar` & `bintropy-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.410348 bintropy-1.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.406348 bintropy-1.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.406348 bintropy-1.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-09 10:37:43.000000 bintropy-1.3.7/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-09 10:37:43.000000 bintropy-1.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 10:37:43.000000 bintropy-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-09 10:37:51.410348 bintropy-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-09 10:37:43.000000 bintropy-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.406348 bintropy-1.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-09 10:37:43.000000 bintropy-1.3.7/docs/example-not-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-09 10:37:43.000000 bintropy-1.3.7/docs/example-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-09 10:37:43.000000 bintropy-1.3.7/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-09 10:37:43.000000 bintropy-1.3.7/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-04-09 10:37:43.000000 bintropy-1.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 10:37:51.410348 bintropy-1.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.406348 bintropy-1.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.410348 bintropy-1.3.7/src/bintropy/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 10:37:43.000000 bintropy-1.3.7/src/bintropy/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 10:37:43.000000 bintropy-1.3.7/src/bintropy/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-04-09 10:37:43.000000 bintropy-1.3.7/src/bintropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-09 10:37:43.000000 bintropy-1.3.7/src/bintropy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.410348 bintropy-1.3.7/src/bintropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.181283 bintropy-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-09 20:53:53.000000 bintropy-1.4.0/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-09 20:53:53.000000 bintropy-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 20:53:53.000000 bintropy-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-09 20:54:01.185284 bintropy-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-09 20:53:53.000000 bintropy-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-09 20:53:53.000000 bintropy-1.4.0/docs/example-not-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-09 20:53:53.000000 bintropy-1.4.0/docs/example-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-09 20:53:53.000000 bintropy-1.4.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-09 20:53:53.000000 bintropy-1.4.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-04-09 20:53:53.000000 bintropy-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 20:54:01.185284 bintropy-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.181283 bintropy-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/src/bintropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 20:53:53.000000 bintropy-1.4.0/src/bintropy/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 20:53:53.000000 bintropy-1.4.0/src/bintropy/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23879 2023-04-09 20:53:53.000000 bintropy-1.4.0/src/bintropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-09 20:53:53.000000 bintropy-1.4.0/src/bintropy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/src/bintropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/top_level.txt
```

### Comparing `bintropy-1.3.7/.github/workflows/python-package.yml` & `bintropy-1.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/.gitignore` & `bintropy-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/LICENSE` & `bintropy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/PKG-INFO` & `bintropy-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.3.7
+Version: 1.4.0
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bintropy-1.3.7/README.md` & `bintropy-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/docs/example-not-packed.png` & `bintropy-1.4.0/docs/example-not-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/docs/example-packed.png` & `bintropy-1.4.0/docs/example-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/docs/logo.png` & `bintropy-1.4.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/pyproject.toml` & `bintropy-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/src/bintropy/__info__.py` & `bintropy-1.4.0/src/bintropy/__info__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.7/src/bintropy/__init__.py` & `bintropy-1.4.0/src/bintropy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import statistics
 
 
 __all__ = ["bintropy", "characteristics", "entropy", "is_packed", "plot", "THRESHOLDS"]
 
 
 __log = lambda l, m, lvl="debug": getattr(l, lvl)(m) if l else None
-__secname = lambda s: s.strip("\x00") or s or"<empty>"
+__secname = lambda s: s.strip("\x00") or s or "<empty>"
 
 # https://matplotlib.org/2.0.2/examples/color/named_colors.html
 COLORS = {
     None:       ["salmon", "gold", "plum", "darkkhaki", "orchid", "sandybrown", "purple", "khaki", "peru", "thistle"],
     'headers':  "black",
     'overlay':  "lightgray",
     '<undef>':  "lightgray",
@@ -42,15 +42,15 @@
     # Mach-O
     'cstring':  "navy",           # string table
     'const':    "cornflowerblue", # read-only data
     'literal4': "blue",           # 4-byte literal values
     'literal4': "mediumblue",     # 8-byte literal values
     'common':   "royalblue",      # uninitialized imported symbol definitions
 }
-MIN_ZONE_WIDTH = 5  # minimum number of samples on the entropy plot for a section (so that it can still be visible even
+MIN_ZONE_WIDTH = 3  # minimum number of samples on the entropy plot for a section (so that it can still be visible even
                     #  if it is far smaller than the other sections)
 N_SAMPLES = 2048
 SUBLABELS = {
     'ep':          lambda d: "EP at 0x%.8x in %s" % d['entrypoint'][1:],
     'size':        lambda d: "Size = %s" % _human_readable_size(d['size'], 1),
     'size-ep':     lambda d: "Size = %s\nEP at 0x%.8x in %s" % \
                              (_human_readable_size(d['size'], 1), d['entrypoint'][1], d['entrypoint'][2]),
@@ -66,14 +66,34 @@
     #TODO: get average and highest entropy values for lief.EXE_FORMATS.ELF
     #TODO: get average and highest entropy values for lief.EXE_FORMATS.MACHO
 }
 
 plt.rcParams['font.family'] = "serif"
 
 
+def _get_ep_and_section(binary):
+    """ Helper for computing the entry point and finding its section for each supported format.
+    :param binary: LIEF-parsed binary object
+    :return:       (ep_file_offset, name_of_ep_section)
+    """
+    btype = str(type(binary)).split(".")[1]
+    try:
+        if btype in ["ELF", "MachO"]:
+            ep = binary.virtual_address_to_offset(binary.entrypoint)
+            ep_section = binary.section_from_offset(ep)
+        elif btype == "PE":
+            ep = binary.rva_to_offset(binary.optional_header.addressof_entrypoint)
+            ep_section = binary.section_from_rva(binary.optional_header.addressof_entrypoint)
+        else:
+            raise OSError("Unknown format")
+        return ep, ep_section.name
+    except (AttributeError, lief.not_found, lief.conversion_error):
+        return None, None
+
+
 def _human_readable_size(size, precision=0):
     """ Convert size in bytes to a more readable form. """
     i, units = 0, ["B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"]
     while size > 1024 and i < len(units):
         i += 1
         size /= 1024.0
     return "%.*f%s" % (precision, size, units[i])
@@ -205,45 +225,52 @@
     tmp_fd, null_fd = os.dup(2), os.open(os.devnull, os.O_RDWR)
     os.dup2(null_fd, 2)
     binary = lief.parse(str(executable))
     os.dup2(tmp_fd, 2)  # restore stderr
     os.close(null_fd)
     if binary is None:
         raise TypeError("Not an executable")
-    data['type'] = "ELF" if type(binary) is lief.ELF.Binary else \
-                   "Mach-O" if type(binary) is lief.MachO.Binary else \
-                   "PE" if type(binary) is lief.PE.Binary else None
-    if data['type'] is None:
-        raise TypeError("Unsupported executable format")
+    data['type'] = str(type(binary)).split(".")[1]
     # entry point (EP)
-    ep = binary.rva_to_offset(binary.optional_header.addressof_entrypoint)
+    ep, ep_section = _get_ep_and_section(binary)
+    # convert to 3-tuple (EP offset on plot, EP file offset, section name containing EP)
+    data['entrypoint'] = None if ep is None else (int(ep // data['chunksize']), ep, __secname(ep_section))
     # sections
-    __d = lambda s, e, n: (s, e, n, statistics.mean(data['entropy'][s:e+1]))
-    data['sections'] = [__d(0, int(max(MIN_ZONE_WIDTH, binary.sizeof_headers // chunksize)), "Headers")]
-    data['entrypoint'] = int(ep // data['chunksize'])
-    ep_section = binary.section_from_rva(binary.optional_header.addressof_entrypoint).name.rstrip("\x00")
-    # convert to 3-tuple (real EP, EP, section of real EP)
-    data['entrypoint'] = (data['entrypoint'], ep, __secname(ep_section))
-    for section in sorted(binary.sections, key=lambda x: x.offset):
+    __d = lambda s, e, n: (int(s), int(e), n, statistics.mean(data['entropy'][int(s):int(e)+1]))
+    data['sections'] = [__d(0, int(max(MIN_ZONE_WIDTH, binary.sections[0].offset // chunksize)), "Headers")] \
+                       if len(binary.sections) > 0 else []
+    for section in binary.sections:
         name = __secname(section.name)
         start = max(data['sections'][-1][1] if len(data['sections']) > 0 else 0, int(section.offset // chunksize))
         max_end = min(max(start + MIN_ZONE_WIDTH, int((section.offset + section.size) // chunksize)),
                       len(data['entropy']) - 1)
         data['sections'].append(__d(int(min(start, max_end - MIN_ZONE_WIDTH)), int(max_end), name))
+    # adjust the entry point (be sure that its position on the plot is within the EP section)
+    if ep:
+        ep_pos, _, ep_sec_name = data['entrypoint']
+        for s, e, name, m in data['sections']:
+            if name == ep_sec_name:
+                data['entrypoint'] = (min(max(ep_pos, s), e), ep, ep_sec_name)
     # fill in undefined sections
     prev_end = None
     for i, t in enumerate(data['sections'][:]):
         start, end, name, _ = t
         if prev_end and prev_end < start:
             data['sections'].insert(i, __d(prev_end, start, "<undef>"))
         prev_end = end
-    # add overlay
-    last = data['sections'][-1][1]
-    if last + 1 < n_samples:
-        data['sections'].append(__d(int(last), int(n_samples), "Overlay"))
+    if len(binary.sections) > 0:
+        last = data['sections'][-1][1]
+        if data['type'] == "ELF":
+            # add section header table
+            sh_size = binary.header.section_header_size * binary.header.numberof_sections
+            data['sections'].append(__d(int(last), int(last) + sh_size // chunksize, "Header"))
+        elif data['type'] == "PE":
+            # add overlay
+            if last + 1 < n_samples:
+                data['sections'].append(__d(int(last), int(n_samples), "Overlay"))
     return data
 
 
 def entropy(something, blocksize=0, ignore_half_block_zeros=False):
     """ Shannon entropy, with the possibility to compute the entropy per block with a given size, possibly ignoring
          blocks in which at least half of the characters or bytes are zeros.
     
@@ -349,15 +376,15 @@
         try:
             label = labels[i]
             if isinstance(label, type(lambda: 0)):
                 label = label(data)
         except:
             pass
         ref_point = .65
-        if sublabel:
+        if sublabel and not (isinstance(sublabel, str) and "ep" in sublabel and data['entrypoint'] is None):
             if isinstance(sublabel, str):
                 sublabel = SUBLABELS.get(sublabel)
             sl = sublabel(data) if isinstance(sublabel, type(lambda: 0)) else None
             if sl:
                 nl, y_pos, f_color = len(sl.split("\n")), ref_point, "black"
                 if label:
                     f_size, f_color = "x-small" if nl <= 2 else "xx-small", "gray"
@@ -368,17 +395,18 @@
         if label:
             y_pos = ref_point
             if sublabel:
                 nl = len(sl.split("\n"))
                 y_pos = min(1., ref_point + nl * [.16, .12, .09, .08][min(4, nl)-1])
             obj.text(s=label, x=-420., y=y_pos, fontsize="large", ha="left", va="center")
         # display the entry point
-        obj.vlines(x=data['entrypoint'][0], ymin=0, ymax=1, color="r", zorder=11).set_label("Entry point")
-        obj.text(data['entrypoint'][0], -.15, "______", c="r", ha="center", rotation=90, size=.8,
-                 bbox={'boxstyle': "rarrow", 'fc': "r", 'ec': "r", 'lw': 1})
+        if data['entrypoint']:
+            obj.vlines(x=data['entrypoint'][0], ymin=0, ymax=1, color="r", zorder=11).set_label("Entry point")
+            obj.text(data['entrypoint'][0], -.15, "______", c="r", ha="center", rotation=90, size=.8,
+                     bbox={'boxstyle': "rarrow", 'fc': "r", 'ec': "r", 'lw': 1})
         color_cursor, last = 0, None
         for start, end, name, avg_ent in data['sections']:
             x = range(start, min(n, end + 1))
             # select the right color first
             try:
                 c = COLORS[name.lower().lstrip("._").strip("\x00\n ")]
             except KeyError:
@@ -400,19 +428,23 @@
                 obj.text(s=name, x=start + (end - start) // 2, y=pos_y, zorder=12, color=c, ha="center", va="center")
                 last = (start, end, last[0] if last else None, last[1] if last else None)
             # draw entropy
             obj.plot(x, data['entropy'][start:end+1], c=c, zorder=10, lw=.1)
             obj.fill_between(x, [0] * len(x), data['entropy'][start:end+1], facecolor=c)
             l = obj.hlines(y=statistics.mean(data['entropy'][start:end+1]), xmin=x[0], xmax=x[-1], color="black",
                            linestyle=(0, (5, 5)), linewidth=.5)
-        l.set_label("Average entropy of section")
+        if len(data['sections']) > 0:
+            l.set_label("Average entropy of section")
+        else:
+            obj.text(.5, ref_point, "Could not parse sections", fontsize=16, color="red", ha="center", va="center")
     plt.subplots_adjust(left=[.15, .02][labels is None and sublabel is None], right=[1.02, .82][lloc_side],
                         bottom=.5/max(1.75, nf))
     h, l = (objs[[0, 1][title]] if nf+[0, 1][title] > 1 else objs).get_legend_handles_labels()
-    plt.figlegend(h, l, loc=lloc, ncol=1 if lloc_side else 2, prop={'size': 7})
+    if len(h) > 0:
+        plt.figlegend(h, l, loc=lloc, ncol=1 if lloc_side else 2, prop={'size': 7})
     img_name = img_name or os.path.splitext(os.path.basename(filenames[0]))[0]
     # appending the extension to img_name is necessary for avoiding an error when the filename contains a ".[...]" ;
     #  e.g. "PortableWinCDEmu-4.0" => this fails with "ValueError: Format '0' is not supported"
     try:
         plt.savefig(img_name + "." + img_format, img_format=img_format, dpi=dpi, bbox_inches="tight")
     except:  # format argument renamed in further versions of pyplot
         plt.savefig(img_name + "." + img_format, format=img_format, dpi=dpi, bbox_inches="tight")
```

### Comparing `bintropy-1.3.7/src/bintropy/__main__.py` & `bintropy-1.4.0/src/bintropy/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,103 @@
-# -*- coding: UTF-8 -*-
-import logging
-from argparse import ArgumentParser, RawTextHelpFormatter
-from ast import literal_eval
-from os.path import exists
-from time import perf_counter
-
-from .__info__ import __author__, __copyright__, __email__, __license__, __reference__, __source__, __version__
-from .__init__ import bintropy, plot, THRESHOLDS
-
-
-lieflog = logging.getLogger("lief")
-lieflog.setLevel(logging.CRITICAL)
-
-
-def valid_file(path):
-    if not exists(path):
-        raise ValueError("input file does not exist")
-    return path
-
-
-class Positive:
-    def __init__(self, *types):
-        self._types = types
-    
-    def __call__(self, string):
-        try:
-            n = literal_eval(string)
-        except ValueError:
-            raise ValueError(string)
-        if not isinstance(n, self._types) or n < 0.:
-            raise ValueError(string)
-        return self._types[0](n)
-    
-    def __repr__(self):
-        return "positive %s" % "|".join(map(lambda x: x.__name__, self._types))
-
-
-def main():
-    """ Tool's main function """
-    descr = "Bintropy {}\n\nAuthor   : {} ({})\nCopyright: {}\nLicense  : {}\nReference: {}\nSource   : {}\n" \
-            "\nThis tool returns whether a binary contains compressed/encrypted bytes or not.\n" \
-            "It supports both modes from the reference paper and adds a third mode of operation (based on segments)." \
-            "\nAs decision criteria, it considers the highest block entropy (%.3f) and average entropy (%.3f) values" \
-            " from the paper.\nIt is also able to generate a plot of the entropy of an input binary.\n\n" % \
-            THRESHOLDS['default'][::-1]
-    descr = descr.format(__version__, __author__, __email__, __copyright__, __license__, __reference__, __source__)
-    examples = "usage examples:\n- " + "\n- ".join([
-        "bintropy elf",
-        "bintropy program.exe -b",
-        "bintropy elf --blocksize 512 --mode 1",
-        "bintropy program.exe -m 2 --do-not-decide",
-        "bintropy program.exe --all-blocks --threshold-average-entropy 6.5",
-        "bintropy program.exe --plot",
-    ])
-    parser = ArgumentParser(description=descr, epilog=examples, formatter_class=RawTextHelpFormatter)
-    parser.add_argument("path", type=valid_file, help="path to executable")
-    parser.add_argument("-b", "--benchmark", action="store_true",
-                        help="enable benchmarking, output in seconds (default: False)")
-    parser.add_argument("-m", "--mode", choices=[0, 1, 2], type=int, default=0,
-                        help="mode of operation (default: 0)\n - 0: full binary\n - 1: per section\n - 2: per segment")
-    parser.add_argument("-p", "--plot", action="store_true", help="plot the entropy and sections (default: False)")
-    parser.add_argument("-v", "--verbose", action="store_true", help="display debug information (default: False)")
-    parser.add_argument("--all-blocks", action="store_true", help="consider all blocks, even those in which more than "
-                                                                  "the half are zeros (default: False)")
-    parser.add_argument("--blocksize", type=Positive(int), default=256,
-                        help="block size to be considered (default: 256)")
-    parser.add_argument("--do-not-decide", dest="decide", action="store_false",
-                        help="do not decide if packed, return entropy values (default: decide)")
-    parser.add_argument("--threshold-average-entropy", type=Positive(float, int),
-                        help="threshold for the average entropy")
-    parser.add_argument("--threshold-highest-entropy", type=Positive(float, int),
-                        help="threshold for the highest entropy")
-    args = parser.parse_args()
-    logging.basicConfig()
-    args.logger = logging.getLogger("bintropy")
-    args.logger.setLevel([logging.INFO, logging.DEBUG][args.verbose])
-    args.ignore_half_block_zeros = not args.all_blocks
-    code = 0
-    # execute the tool
-    if args.benchmark:
-        t1 = perf_counter()
-    try:
-        r = bintropy(args.path, **vars(args))
-        if r is None:
-            raise Exception("no result")
-        dt = str(perf_counter() - t1) if args.benchmark else ""
-        if not isinstance(r, (tuple, list)):
-            r = [r]
-        r = list(map(str, r))
-        if dt != "":
-            r.append(dt)
-        print(" ".join(r))
-        if args.plot:
-            plot(args.path, **vars(args))
-    except Exception as e:
-        if str(e) != "no result":
-            args.logger.exception(e)
-        code = 1
-    return code
-
+# -*- coding: UTF-8 -*-
+import logging
+from argparse import ArgumentParser, RawTextHelpFormatter
+from ast import literal_eval
+from os.path import exists, isfile
+from time import perf_counter
+
+from .__info__ import __author__, __copyright__, __email__, __license__, __reference__, __source__, __version__
+from .__init__ import bintropy, plot, THRESHOLDS
+
+
+lieflog = logging.getLogger("lief")
+lieflog.setLevel(logging.CRITICAL)
+
+
+def valid_file(path):
+    if not exists(path):
+        raise ValueError("input file does not exist")
+    if not isfile(path):
+        raise ValueError("input is not a file")
+    return path
+
+
+class Positive:
+    def __init__(self, *types):
+        self._types = types
+    
+    def __call__(self, string):
+        try:
+            n = literal_eval(string)
+        except ValueError:
+            raise ValueError(string)
+        if not isinstance(n, self._types) or n < 0.:
+            raise ValueError(string)
+        return self._types[0](n)
+    
+    def __repr__(self):
+        return "positive %s" % "|".join(map(lambda x: x.__name__, self._types))
+
+
+def main():
+    """ Tool's main function """
+    descr = "Bintropy {}\n\nAuthor   : {} ({})\nCopyright: {}\nLicense  : {}\nReference: {}\nSource   : {}\n" \
+            "\nThis tool returns whether a binary contains compressed/encrypted bytes or not.\n" \
+            "It supports both modes from the reference paper and adds a third mode of operation (based on segments)." \
+            "\nAs decision criteria, it considers the highest block entropy (%.3f) and average entropy (%.3f) values" \
+            " from the paper.\nIt is also able to generate a plot of the entropy of an input binary.\n\n" % \
+            THRESHOLDS['default'][::-1]
+    descr = descr.format(__version__, __author__, __email__, __copyright__, __license__, __reference__, __source__)
+    examples = "usage examples:\n- " + "\n- ".join([
+        "bintropy elf",
+        "bintropy program.exe -b",
+        "bintropy elf --blocksize 512 --mode 1",
+        "bintropy program.exe -m 2 --do-not-decide",
+        "bintropy program.exe --all-blocks --threshold-average-entropy 6.5",
+        "bintropy program.exe --plot",
+    ])
+    parser = ArgumentParser(description=descr, epilog=examples, formatter_class=RawTextHelpFormatter)
+    parser.add_argument("path", type=valid_file, help="path to executable")
+    parser.add_argument("-b", "--benchmark", action="store_true",
+                        help="enable benchmarking, output in seconds (default: False)")
+    parser.add_argument("-m", "--mode", choices=[0, 1, 2], type=int, default=0,
+                        help="mode of operation (default: 0)\n - 0: full binary\n - 1: per section\n - 2: per segment")
+    parser.add_argument("-p", "--plot", action="store_true", help="plot the entropy and sections (default: False)")
+    parser.add_argument("-v", "--verbose", action="store_true", help="display debug information (default: False)")
+    parser.add_argument("--all-blocks", action="store_true", help="consider all blocks, even those in which more than "
+                                                                  "the half are zeros (default: False)")
+    parser.add_argument("--blocksize", type=Positive(int), default=256,
+                        help="block size to be considered (default: 256)")
+    parser.add_argument("--do-not-decide", dest="decide", action="store_false",
+                        help="do not decide if packed, return entropy values (default: decide)")
+    parser.add_argument("--threshold-average-entropy", type=Positive(float, int),
+                        help="threshold for the average entropy")
+    parser.add_argument("--threshold-highest-entropy", type=Positive(float, int),
+                        help="threshold for the highest entropy")
+    args = parser.parse_args()
+    logging.basicConfig()
+    args.logger = logging.getLogger("bintropy")
+    args.logger.setLevel([logging.INFO, logging.DEBUG][args.verbose])
+    args.ignore_half_block_zeros = not args.all_blocks
+    code = 0
+    # execute the tool
+    if args.benchmark:
+        t1 = perf_counter()
+    try:
+        r = bintropy(args.path, **vars(args))
+        if r is None:
+            raise Exception("no result")
+        dt = str(perf_counter() - t1) if args.benchmark else ""
+        if not isinstance(r, (tuple, list)):
+            r = [r]
+        r = list(map(str, r))
+        if dt != "":
+            r.append(dt)
+        print(" ".join(r))
+        if args.plot:
+            plot(args.path, **vars(args))
+    except Exception as e:
+        if str(e) != "no result":
+            args.logger.exception(e)
+        code = 1
+    return code
+
```

### Comparing `bintropy-1.3.7/src/bintropy.egg-info/PKG-INFO` & `bintropy-1.4.0/src/bintropy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.3.7
+Version: 1.4.0
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

