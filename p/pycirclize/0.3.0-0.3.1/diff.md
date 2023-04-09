# Comparing `tmp/pycirclize-0.3.0.tar.gz` & `tmp/pycirclize-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycirclize-0.3.0.tar", max compression
+gzip compressed data, was "pycirclize-0.3.1.tar", max compression
```

## Comparing `pycirclize-0.3.0.tar` & `pycirclize-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,41 @@
--rw-r--r--   0        0        0     1062 2023-04-01 07:16:59.637385 pycirclize-0.3.0/LICENSE
--rw-r--r--   0        0        0     4721 2023-04-01 07:16:59.637385 pycirclize-0.3.0/README.md
--rw-r--r--   0        0        0     1210 2023-04-01 07:16:59.785391 pycirclize-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       89 2023-04-01 07:16:59.785391 pycirclize-0.3.0/src/pycirclize/__init__.py
--rw-r--r--   0        0        0    29042 2023-04-01 07:16:59.785391 pycirclize-0.3.0/src/pycirclize/circos.py
--rw-r--r--   0        0        0     2867 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/config.py
--rw-r--r--   0        0        0      232 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/parser/__init__.py
--rw-r--r--   0        0        0     1684 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/parser/bed.py
--rw-r--r--   0        0        0    14435 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/parser/genbank.py
--rw-r--r--   0        0        0    13398 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/parser/gff.py
--rw-r--r--   0        0        0     7996 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/parser/matrix.py
--rw-r--r--   0        0        0    11565 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/patches.py
--rw-r--r--   0        0        0    14932 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/sector.py
--rw-r--r--   0        0        0    45252 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/track.py
--rw-r--r--   0        0        0      534 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/utils/__init__.py
--rw-r--r--   0        0        0     6888 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/utils/dataset.py
--rw-r--r--   0        0        0     3774 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/utils/helper.py
--rw-r--r--   0        0        0     9955 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/utils/images/python_logo.png
--rw-r--r--   0        0        0     2314 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/utils/plot.py
--rw-r--r--   0        0        0     4991 2023-04-01 07:16:59.789391 pycirclize-0.3.0/src/pycirclize/utils/tree.py
--rw-r--r--   0        0        0        0 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1514 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/parser/__init__.py
--rw-r--r--   0        0        0     2090 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/parser/test_matrix.py
--rw-r--r--   0        0        0     2751 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/test_circos.py
--rw-r--r--   0        0        0    20975 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/test_plot.py
--rw-r--r--   0        0        0     2811 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/test_sector.py
--rw-r--r--   0        0        0      925 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/test_track.py
--rw-r--r--   0        0        0      755 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/testdata/eukaryote/hg38/hg38_chr.bed
--rw-r--r--   0        0        0    30808 2023-04-01 07:16:59.789391 pycirclize-0.3.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
--rw-r--r--   0        0        0   283582 2023-04-01 07:16:59.793391 pycirclize-0.3.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
--rw-r--r--   0        0        0   148834 2023-04-01 07:16:59.793391 pycirclize-0.3.0/tests/testdata/prokaryote/enterobacteria_phage.gbk
--rw-r--r--   0        0        0    36204 2023-04-01 07:16:59.793391 pycirclize-0.3.0/tests/testdata/prokaryote/enterobacteria_phage.gff
--rw-r--r--   0        0        0        0 2023-04-01 07:16:59.793391 pycirclize-0.3.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1983 2023-04-01 07:16:59.793391 pycirclize-0.3.0/tests/utils/test_dataset.py
--rw-r--r--   0        0        0     1839 2023-04-01 07:16:59.793391 pycirclize-0.3.0/tests/utils/test_helper.py
--rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 pycirclize-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-09 08:06:37.002844 pycirclize-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4783 2023-04-09 08:06:37.002844 pycirclize-0.3.1/README.md
+-rw-r--r--   0        0        0     1216 2023-04-09 08:06:37.158843 pycirclize-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/__init__.py
+-rw-r--r--   0        0        0    29406 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/circos.py
+-rw-r--r--   0        0        0     2921 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/config.py
+-rw-r--r--   0        0        0      232 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/__init__.py
+-rw-r--r--   0        0        0     1684 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/bed.py
+-rw-r--r--   0        0        0    18161 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/genbank.py
+-rw-r--r--   0        0        0    15424 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/gff.py
+-rw-r--r--   0        0        0     7996 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/parser/matrix.py
+-rw-r--r--   0        0        0    12582 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/patches.py
+-rw-r--r--   0        0        0    15864 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/sector.py
+-rw-r--r--   0        0        0    45503 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/track.py
+-rw-r--r--   0        0        0      534 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/__init__.py
+-rw-r--r--   0        0        0     6869 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/dataset.py
+-rw-r--r--   0        0        0     3774 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/helper.py
+-rw-r--r--   0        0        0     9955 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/images/python_logo.png
+-rw-r--r--   0        0        0     2314 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/plot.py
+-rw-r--r--   0        0        0     4991 2023-04-09 08:06:37.158843 pycirclize-0.3.1/src/pycirclize/utils/tree.py
+-rw-r--r--   0        0        0        0 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1941 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/parser/__init__.py
+-rw-r--r--   0        0        0     1752 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/parser/test_genbank.py
+-rw-r--r--   0        0        0     1839 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/parser/test_gff.py
+-rw-r--r--   0        0        0     2090 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/parser/test_matrix.py
+-rw-r--r--   0        0        0     2751 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/test_circos.py
+-rw-r--r--   0        0        0    20534 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/test_plot.py
+-rw-r--r--   0        0        0     2811 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/test_sector.py
+-rw-r--r--   0        0        0      925 2023-04-09 08:06:37.158843 pycirclize-0.3.1/tests/test_track.py
+-rw-r--r--   0        0        0      755 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_chr.bed
+-rw-r--r--   0        0        0    30808 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv
+-rw-r--r--   0        0        0   283582 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv
+-rw-r--r--   0        0        0   148834 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/prokaryote/enterobacteria_phage.gbk
+-rw-r--r--   0        0        0    36204 2023-04-09 08:06:37.162843 pycirclize-0.3.1/tests/testdata/prokaryote/enterobacteria_phage.gff
+-rw-r--r--   0        0        0   580710 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/testdata/prokaryote/mycoplasma_alvi.gbk.gz
+-rw-r--r--   0        0        0    58530 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/testdata/prokaryote/mycoplasma_alvi.gff.gz
+-rw-r--r--   0        0        0        0 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1983 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/utils/test_dataset.py
+-rw-r--r--   0        0        0     1839 2023-04-09 08:06:37.166843 pycirclize-0.3.1/tests/utils/test_helper.py
+-rw-r--r--   0        0        0     5743 1970-01-01 00:00:00.000000 pycirclize-0.3.1/PKG-INFO
```

### Comparing `pycirclize-0.3.0/LICENSE` & `pycirclize-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/README.md` & `pycirclize-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 API usage is described in each of the following sections in the [document](https://moshi4.github.io/pyCirclize/).
 
 - [Getting Started](https://moshi4.github.io/pyCirclize/getting_started/)
 - [Plot API Example](https://moshi4.github.io/pyCirclize/plot_api_example/)
 - [Chord Diagram](https://moshi4.github.io/pyCirclize/chord_diagram/)
 - [Circos Plot (Genomics)](https://moshi4.github.io/pyCirclize/circos_plot/)
 - [Phylogenetic Tree](https://moshi4.github.io/pyCirclize/phylogenetic_tree/)
+- [Plot Tips](https://moshi4.github.io/pyCirclize/plot_tips/)
 
 ## Code Example
 
 ### 1. Circos Plot
 
 ```python
 from pycirclize import Circos
```

### Comparing `pycirclize-0.3.0/pyproject.toml` & `pycirclize-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyCirclize"
-version = "0.3.0"
+version = "0.3.1"
 description = "Circular visualization in Python"
 authors = ["moshi4"]
 license = "MIT"
 homepage = "https://moshi4.github.io/pyCirclize/"
 repository = "https://github.com/moshi4/pyCirclize/"
 readme = "README.md"
 keywords = [
@@ -31,15 +31,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 matplotlib = ">=3.5.2"
 biopython = ">=1.79"
 numpy = ">=1.21.1"
 pandas = ">=1.3.5"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = ">=7.1.2"
 black = ">=22.10.0"
 flake8 = ">=4.0.1"
 pydocstyle = ">=6.1.1"
 pytest-cov = ">=4.0.0"
 ipykernel = ">=6.13.0"
 mkdocs = ">=1.2"
```

### Comparing `pycirclize-0.3.0/src/pycirclize/circos.py` & `pycirclize-0.3.1/src/pycirclize/circos.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from matplotlib.colors import Colormap, Normalize
 from matplotlib.figure import Figure
 from matplotlib.patches import Patch
 from matplotlib.projections.polar import PolarAxes
 
 from pycirclize import config, utils
 from pycirclize.parser import Bed, Matrix
-from pycirclize.patches import ArcLine, ArcRectangle, BezierCurve
+from pycirclize.patches import ArcLine, ArcRectangle, BezierCurve, Line
 from pycirclize.sector import Sector
 from pycirclize.track import Track
 
 
 class Circos:
     """Circos Visualization Class"""
 
@@ -449,33 +449,39 @@
             ax.text(math.radians(deg), r, text, **kwargs)
 
         self._plot_funcs.append(plot_text)
 
     def line(
         self,
         *,
-        r: float,
+        r: float | tuple[float, float],
         deg_lim: tuple[float, float] | None = None,
+        arc: bool = True,
         **kwargs,
     ) -> None:
         """Plot line
 
         Parameters
         ----------
-        r : float
-            Radius position (0 - 100)
+        r : float, tuple[float, float]
+            Line radius position (0 - 100). If r is float, (r, r) is set.
         deg_lim : tuple[float, float]
             Degree limit region (-360 - 360). If None, `circos.deg_lim` is set.
+        arc : bool, optional
+            If True, plot arc style line for polar projection.
+            If False, simply plot linear style line.
         **kwargs : dict, optional
             Patch properties (e.g. `color="red", lw=3, ...`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
         """
         deg_lim = self.deg_lim if deg_lim is None else deg_lim
         rad_lim = (math.radians(min(deg_lim)), math.radians(max(deg_lim)))
-        self._patches.append(ArcLine(rad_lim, (r, r), **kwargs))
+        r_lim = r if isinstance(r, (tuple, list)) else (r, r)
+        LinePatch = ArcLine if arc else Line
+        self._patches.append(LinePatch(rad_lim, r_lim, **kwargs))
 
     def rect(
         self,
         r_lim: tuple[float, float] = (0, 100),
         deg_lim: tuple[float, float] | None = None,
         **kwargs,
     ) -> None:
```

### Comparing `pycirclize-0.3.0/src/pycirclize/config.py` & `pycirclize-0.3.1/src/pycirclize/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,10 +95,12 @@
         "mm10_genomic_link.tsv",
     ],
 }
 
 PROKARYOTE_FILES = [
     "enterobacteria_phage.gbk",
     "enterobacteria_phage.gff",
+    "mycoplasma_alvi.gbk",
+    "mycoplasma_alvi.gff",
     "escherichia_coli.gbk.gz",
     "escherichia_coli.gff.gz",
 ]
```

### Comparing `pycirclize-0.3.0/src/pycirclize/parser/bed.py` & `pycirclize-0.3.1/src/pycirclize/parser/bed.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/src/pycirclize/parser/genbank.py` & `pycirclize-0.3.1/src/pycirclize/parser/genbank.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import bz2
 import gzip
 import zipfile
+from collections import defaultdict
 from functools import lru_cache
 from io import TextIOWrapper
 from pathlib import Path
 from typing import Any
 
 import numpy as np
 from Bio import SeqIO, SeqUtils
@@ -132,37 +133,46 @@
         """Range genome sequence"""
         seq = "".join(str(r.seq) for r in self.records)
         return seq[self.min_range : self.max_range]
 
     @lru_cache(maxsize=None)
     def calc_genome_gc_content(self) -> float:
         """Calculate genome GC content"""
-        return SeqUtils.gc_fraction(self.genome_seq) * 100
+        try:
+            gc_content = SeqUtils.gc_fraction(self.genome_seq) * 100
+        except AttributeError:
+            # For backward compatibility, biopython <= 1.79
+            gc_content = SeqUtils.GC(self.genome_seq)
+        return gc_content
 
     def calc_gc_skew(
         self,
         window_size: int | None = None,
         step_size: int | None = None,
+        *,
+        seq: str | None = None,
     ) -> tuple[np.ndarray, np.ndarray]:
         """Calculate GC skew in sliding window
 
         Parameters
         ----------
         window_size : int | None, optional
             Window size (Default: `genome_size / 500`)
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
+        seq : str | None, optional
+            Sequence for GCskew calculation (Default: `self.genome_seq`)
 
         Returns
         -------
         gc_skew_result_tuple : tuple[np.ndarray, np.ndarray]
             Position list & GC skew list
         """
         pos_list, gc_skew_list = [], []
-        seq = self.genome_seq
+        seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
             step_size = int(len(seq) / 1000)
         pos_list = list(range(0, len(seq), step_size)) + [len(seq)]
         for pos in pos_list:
             window_start_pos = pos - int(window_size / 2)
@@ -181,47 +191,132 @@
 
         return (np.array(pos_list), np.array(gc_skew_list))
 
     def calc_gc_content(
         self,
         window_size: int | None = None,
         step_size: int | None = None,
+        *,
+        seq: str | None = None,
     ) -> tuple[np.ndarray, np.ndarray]:
         """Calculate GC content in sliding window
 
         Parameters
         ----------
         window_size : int | None, optional
             Window size (Default: `genome_size / 500`)
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
+        seq : str | None, optional
+            Sequence for GCskew calculation (Default: `self.genome_seq`)
 
         Returns
         -------
         gc_content_result_tuple : tuple[np.ndarray, np.ndarray]
             Position list & GC content list
         """
         pos_list, gc_content_list = [], []
-        seq = self.genome_seq
+        seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
             step_size = int(len(seq) / 1000)
         pos_list = list(range(0, len(seq), step_size)) + [len(seq)]
         for pos in pos_list:
             window_start_pos = pos - int(window_size / 2)
             window_end_pos = pos + int(window_size / 2)
             window_start_pos = 0 if window_start_pos < 0 else window_start_pos
             window_end_pos = len(seq) if window_end_pos > len(seq) else window_end_pos
 
             subseq = seq[window_start_pos:window_end_pos]
-            gc_content_list.append(SeqUtils.gc_fraction(subseq) * 100)
+            try:
+                gc_content = SeqUtils.gc_fraction(subseq) * 100
+            except AttributeError:
+                # For backward compatibility, biopython <= 1.79
+                gc_content = SeqUtils.GC(subseq)
+            gc_content_list.append(gc_content)
 
         return (np.array(pos_list), np.array(gc_content_list))
 
+    def get_seqid2seq(self) -> dict[str, str]:
+        """Get seqid & complete/contig/scaffold genome sequence dict
+
+        Returns
+        -------
+        seqid2seq : dict[str, int]
+            seqid & genome sequence dict
+        """
+        return {rec.id: rec.seq for rec in self.records}
+
+    def get_seqid2size(self) -> dict[str, int]:
+        """Get seqid & complete/contig/scaffold genome size dict
+
+        Returns
+        -------
+        seqid2size : dict[str, int]
+            seqid & genome size dict
+        """
+        return {seqid: len(seq) for seqid, seq in self.get_seqid2seq().items()}
+
+    def get_seqid2features(
+        self,
+        feature_type: str | None = "CDS",
+        target_strand: int | None = None,
+        pseudogene: bool | None = False,
+    ) -> dict[str, list[SeqFeature]]:
+        """Get seqid & features in target seqid genome dict
+
+        Parameters
+        ----------
+        feature_type : str | None, optional
+            Feature type (`CDS`, `gene`, `mRNA`, etc...)
+            If None, extract regardless of feature type.
+        target_strand : int | None, optional
+            Extract target strand. If None, extract regardless of strand.
+        pseudogene : bool | None, optional
+            If True, `pseudo=`, `pseudogene=` tagged record only extract.
+            If False, `pseudo=`, `pseudogene=` not tagged record only extract.
+            If None, extract regardless of pseudogene tag.
+
+        Returns
+        -------
+        seqid2features : dict[str, list[SeqFeature]]
+            seqid & features dict
+        """
+        seqid2features = defaultdict(list)
+        for rec in self.records:
+            feat: SeqFeature
+            for feat in rec.features:
+                if feature_type is not None and feat.type != feature_type:
+                    continue
+                if target_strand is not None and feat.strand != target_strand:
+                    continue
+                if feat.strand == -1:
+                    start = self._to_int(feat.location.parts[-1].start)
+                    end = self._to_int(feat.location.parts[0].end)
+                else:
+                    start = self._to_int(feat.location.parts[0].start)
+                    end = self._to_int(feat.location.parts[-1].end)
+
+                qual = feat.qualifiers
+                has_pseudo_qual = "pseudo" in qual or "pseudogene" in qual
+                if (
+                    pseudogene is None
+                    or (pseudogene is True and has_pseudo_qual)
+                    or (pseudogene is False and not has_pseudo_qual)
+                ):
+                    seqid2features[rec.id].append(
+                        SeqFeature(
+                            location=FeatureLocation(start, end, feat.strand),
+                            type=feat.type,
+                            qualifiers=feat.qualifiers,
+                        ),
+                    )
+        return seqid2features
+
     def extract_features(
         self,
         feature_type: str = "CDS",
         target_strand: int | None = None,
         fix_position: bool = False,
         allow_partial: bool = False,
         pseudogene: bool = False,
```

### Comparing `pycirclize-0.3.0/src/pycirclize/parser/gff.py` & `pycirclize-0.3.1/src/pycirclize/parser/gff.py`

 * *Files 8% similar despite different names*

```diff
@@ -183,48 +183,99 @@
         return self._target_seqid
 
     @property
     def seqid_list(self) -> list[str]:
         """seqid list"""
         return self._seqid_list
 
+    def get_seqid2size(self) -> dict[str, int]:
+        """Get seqid & complete/contig/scaffold genome size dict
+
+        Returns
+        -------
+        seqid2size : dict[str, int]
+            seqid & genome size dict
+        """
+        seqid2size: dict[str, int] = {}
+        for seqid in self.seqid_list:
+            gff = Gff(self._gff_file, target_seqid=seqid)
+            seqid2size[seqid] = gff.range_size
+        return seqid2size
+
+    def get_seqid2features(
+        self,
+        feature_type: str | None = "CDS",
+        target_strand: int | None = None,
+        pseudogene: bool | None = False,
+    ) -> dict[str, list[SeqFeature]]:
+        """Get seqid & features in target seqid genome dict
+
+        Parameters
+        ----------
+        feature_type : str | None, optional
+            Feature type (`CDS`, `gene`, `mRNA`, etc...)
+            If None, extract regardless of feature type.
+        target_strand : int | None, optional
+            Extract target strand. If None, extract regardless of strand.
+        pseudogene : bool | None, optional
+            If True, `pseudo=`, `pseudogene=` tagged record only extract.
+            If False, `pseudo=`, `pseudogene=` not tagged record only extract.
+            If None, extract regardless of pseudogene tag.
+
+        Returns
+        -------
+        seqid2features : dict[str, list[SeqFeature]]
+            seqid & features dict
+        """
+        seqid2features = {}
+        for seqid in self.seqid_list:
+            gff = Gff(self._gff_file, target_seqid=seqid)
+            seqid2features[seqid] = gff.extract_features(
+                feature_type, target_strand, pseudogene
+            )
+        return seqid2features
+
     def extract_features(
         self,
-        feature_type: str = "CDS",
+        feature_type: str | None = "CDS",
         target_strand: int | None = None,
-        pseudogene: bool = False,
+        pseudogene: bool | None = False,
     ) -> list[SeqFeature]:
         """Extract features within min-max range
 
         Parameters
         ----------
-        feature_type : str, optional
+        feature_type : str | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
+            If None, extract regardless of feature type.
         target_strand : int | None, optional
-            Extract target strand
-        pseudogene : bool, optional
-            If True, `pseudo=`, `pseudogne=` tagged record only extract.
+            Extract target strand. If None, extract regardless of strand.
+        pseudogene : bool | None, optional
+            If True, `pseudo=`, `pseudogene=` tagged record only extract.
             If False, `pseudo=`, `pseudogene=` not tagged record only extract.
+            If None, extract all regardless of pseudogene tag.
 
         Returns
         -------
         features : list[SeqFeature]
             Feature list
         """
         features: list[SeqFeature] = []
         for rec in self.records_within_range:
-            if rec.type != feature_type:
+            if feature_type is not None and rec.type != feature_type:
                 continue
             if target_strand is not None and rec.strand != target_strand:
                 continue
-            if pseudogene and ("pseudo" in rec.attrs or "pseudogene" in rec.attrs):
+            has_pseudo_attr = "pseudo" in rec.attrs or "pseudogene" in rec.attrs
+            if (
+                pseudogene is None
+                or (pseudogene is True and has_pseudo_attr)
+                or (pseudogene is False and not has_pseudo_attr)
+            ):
                 features.append(rec.to_seq_feature())
-            else:
-                features.append(rec.to_seq_feature())
-
         return features
 
     def extract_exon_features(self, feature_type: str = "mRNA") -> list[SeqFeature]:
         """Extract exon structure features within min-max range
 
         Extract exons based on `parent feature` and `exon` ID-Parent relation
```

### Comparing `pycirclize-0.3.0/src/pycirclize/parser/matrix.py` & `pycirclize-0.3.1/src/pycirclize/parser/matrix.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/src/pycirclize/patches.py` & `pycirclize-0.3.1/src/pycirclize/patches.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,46 @@
 import numpy as np
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
 
 from pycirclize import config
 
 
+class Line(PathPatch):
+    """Linear Line Patch"""
+
+    def __init__(
+        self,
+        rad_lim: tuple[float, float],
+        r_lim: tuple[float, float],
+        **kwargs,
+    ):
+        """
+        Parameters
+        ----------
+        rad_lim : tuple[float, float]
+            Radian limit region
+        r_lim : tuple[float, float]
+            Radius limit region
+        **kwargs : dict, optional
+            Patch properties (e.g. `ec="red", lw=1.0, ...`)
+            <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
+        """
+        # Default params: fc='none', color='black', linewidth=0.5
+        kwargs.update(dict(fc="none"))
+        if "ec" not in kwargs and "edgecolor" not in kwargs and "color" not in kwargs:
+            kwargs.update(dict(ec="black"))
+        if "lw" not in kwargs and "linewidth" not in kwargs:
+            kwargs.update(dict(lw=0.5))
+
+        # Set line path
+        verts = list(zip(rad_lim, r_lim))
+        super().__init__(Path(verts), **kwargs)
+
+
 class ArcLine(PathPatch):
     """Arc Line Patch"""
 
     def __init__(
         self,
         rad_lim: tuple[float, float],
         r_lim: tuple[float, float],
```

### Comparing `pycirclize-0.3.0/src/pycirclize/sector.py` & `pycirclize-0.3.1/src/pycirclize/sector.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 from matplotlib.patches import Patch
 from matplotlib.projections.polar import PolarAxes
 from PIL import Image, ImageOps
 
 from pycirclize import config, utils
-from pycirclize.patches import ArcLine, ArcRectangle
+from pycirclize.patches import ArcLine, ArcRectangle, Line
 from pycirclize.track import Track
 from pycirclize.utils.plot import get_label_params_by_rad
 
 
 class Sector:
     """Circos Sector Class"""
 
@@ -220,75 +220,91 @@
 
     def text(
         self,
         text: str,
         x: float | None = None,
         r: float = 105,
         *,
+        adjust_rotation: bool = True,
         orientation: str = "horizontal",
+        ignore_range_error: bool = False,
         **kwargs,
     ) -> None:
         """Plot text
 
         Parameters
         ----------
         text : str
             Text content
         x: float, optional
             X position. If None, sector center x is set.
         r : float, optional
             Radius position. By default, outer position `r=105` is set.
+        adjust_rotation : bool, optional
+            If True, text rotation is auto set based on `x` and `orientation` params.
         orientation : str, optional
             Text orientation (`horizontal` or `vertical`)
+        ignore_range_error : bool, optional
+            If True, ignore x position range error
+            (ErrorCase: `not track.start <= x <= track.end`)
         **kwargs : dict, optional
             Text properties (e.g. `size=12, color="red", va="center", ...`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         """
-        if x is None:
-            # Get sector center radian position
-            center_x = (self.start + self.end) / 2
-            rad = self.x_to_rad(center_x)
-        else:
-            rad = self.x_to_rad(x)
-
-        # Set label proper alignment, rotation parameters by radian
-        params = utils.plot.get_label_params_by_rad(rad, orientation, outer=True)
-        kwargs.update(params)
+        # If value is None, center position is set.
+        x = (self.start + self.end) / 2 if x is None else x
+        rad = self.x_to_rad(x, ignore_range_error)
+
+        if adjust_rotation:
+            # Set label proper alignment, rotation parameters by radian
+            params = utils.plot.get_label_params_by_rad(rad, orientation)
+            kwargs.update(params)
+
+        if "ha" not in kwargs and "horizontalalignment" not in kwargs:
+            kwargs.update(dict(ha="center"))
+        if "va" not in kwargs and "verticalalignment" not in kwargs:
+            kwargs.update(dict(va="center"))
 
         def plot_text(ax: PolarAxes) -> None:
             ax.text(rad, r, text, **kwargs)
 
         self._plot_funcs.append(plot_text)
 
     def line(
         self,
         *,
-        r: float,
+        r: float | tuple[float, float],
         start: float | None = None,
         end: float | None = None,
+        arc: bool = True,
         **kwargs,
     ) -> None:
         """Plot line
 
         Parameters
         ----------
-        r : float
-            Line radius position (0 - 100)
+        r : float, tuple[float, float]
+            Line radius position (0 - 100). If r is float, (r, r) is set.
         start : float, optional
             Start position (x coordinate). If None, `sector.start` is set.
         end : float, optional
             End position (x coordinate). If None, `sector.end` is set.
+        arc : bool, optional
+            If True, plot arc style line for polar projection.
+            If False, simply plot linear style line.
         **kwargs : dict, optional
             Patch properties (e.g. `color="red", lw=3, ...`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
         """
         start = self.start if start is None else start
         end = self.end if end is None else end
         rad_lim = (self.x_to_rad(start), self.x_to_rad(end))
-        self._patches.append(ArcLine(rad_lim, (r, r), **kwargs))
+        r_lim = r if isinstance(r, (tuple, list)) else (r, r)
+        LinePatch = ArcLine if arc else Line
+        self._patches.append(LinePatch(rad_lim, r_lim, **kwargs))
 
     def rect(
         self,
         start: float | None = None,
         end: float | None = None,
         r_lim: tuple[float, float] | None = None,
         **kwargs,
```

### Comparing `pycirclize-0.3.0/src/pycirclize/track.py` & `pycirclize-0.3.1/src/pycirclize/track.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,28 +615,32 @@
     def line(
         self,
         x: list[float] | np.ndarray,
         y: list[float] | np.ndarray,
         *,
         vmin: float = 0,
         vmax: float | None = None,
+        arc: bool = True,
         **kwargs,
     ) -> None:
         """Plot line
 
         Parameters
         ----------
         x : list[float] | np.ndarray
             X coordinates
         y : list[float] | np.ndarray
             Y coordinates
         vmin : float, optional
             Y min value
         vmax : float | None, optional
             Y max value. If None, `max(y)` is set.
+        arc : bool, optional
+            If True, plot arc style line for polar projection.
+            If False, simply plot linear style line.
         **kwargs : dict, optional
             Axes.plot properties (e.g. `color="red", lw=0.5, ls="--", ...`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.plot.html>
         """
         # Check x, y list length
         if len(x) != len(y):
             err_msg = f"List length is not match ({len(x)=}, {len(y)=})"
@@ -644,19 +648,22 @@
 
         # Convert (x, y) to (rad, r)
         rad = list(map(self.x_to_rad, x))
         vmax = max(y) if vmax is None else vmax
         self._check_value_min_max(y, vmin, vmax)
         r = [self._y_to_r(v, vmin, vmax) for v in y]
 
-        # Convert normal line to arc line (rad, r) points
-        arc_rad, arc_r = self._to_arc_radr(rad, r)
+        if arc:
+            # Convert linear line to arc line (rad, r) points
+            plot_rad, plot_r = self._to_arc_radr(rad, r)
+        else:
+            plot_rad, plot_r = rad, r
 
         def plot_line(ax: PolarAxes) -> None:
-            ax.plot(arc_rad, arc_r, **kwargs)
+            ax.plot(plot_rad, plot_r, **kwargs)
 
         self._plot_funcs.append(plot_line)
 
     def scatter(
         self,
         x: list[float] | np.ndarray,
         y: list[float] | np.ndarray,
```

### Comparing `pycirclize-0.3.0/src/pycirclize/utils/__init__.py` & `pycirclize-0.3.1/src/pycirclize/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/src/pycirclize/utils/dataset.py` & `pycirclize-0.3.1/src/pycirclize/utils/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,17 @@
     """Load pycirclize example Genbank or GFF file
 
     Load example file from <https://github.com/moshi4/pycirclize-data/>
     and cache file in local directory (Default: `~/.cache/pycirclize/`).
 
     List of example Genbank or GFF filename
 
-    - `enterobacteria_phage.gbk`
-    - `enterobacteria_phage.gff`
-    - `escherichia_coli.gbk.gz`
-    - `escherichia_coli.gff.gz`
+    - `enterobacteria_phage.[gbk|gff]`
+    - `mycoplasma_alvi.[gbk|gff]`
+    - `escherichia_coli.[gbk|gff].gz`
 
     Parameters
     ----------
     filename : str
         Genbank or GFF filename (e.g. `enterobacteria_phage.gff`)
     cache_dir : str | Path | None, optional
         Output cache directory (Default: `~/.cache/pycirclize/`)
```

### Comparing `pycirclize-0.3.0/src/pycirclize/utils/helper.py` & `pycirclize-0.3.1/src/pycirclize/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/src/pycirclize/utils/images/python_logo.png` & `pycirclize-0.3.1/src/pycirclize/utils/images/python_logo.png`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/src/pycirclize/utils/plot.py` & `pycirclize-0.3.1/src/pycirclize/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/src/pycirclize/utils/tree.py` & `pycirclize-0.3.1/src/pycirclize/utils/tree.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/parser/test_matrix.py` & `pycirclize-0.3.1/tests/parser/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/test_circos.py` & `pycirclize-0.3.1/tests/test_circos.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/test_plot.py` & `pycirclize-0.3.1/tests/test_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,27 @@
 import random
 from io import StringIO
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
-import pytest
 from Bio import Phylo
 
 from pycirclize import Circos
 from pycirclize.parser import Genbank, Gff
 from pycirclize.utils import (
     ColorCycler,
     load_eukaryote_example_dataset,
     load_prokaryote_example_file,
 )
 
 np.random.seed(0)
 random.seed(0)
 
 
-@pytest.fixture
-def fig_outfile(tmp_path: Path) -> Path:
-    """Figure output file fixture"""
-    return tmp_path / "figure.png"
-
-
-@pytest.fixture
-def hg38_testdata_dir(testdata_dir: Path):
-    """hg38 dataset directory fixture"""
-    return testdata_dir / "eukaryote" / "hg38"
-
-
-@pytest.fixture
-def prokaryote_testdata_dir(testdata_dir: Path):
-    """Prokaryote test file directory"""
-    return testdata_dir / "prokaryote"
-
-
 ###########################################################
 # Circos Class Plot
 ###########################################################
 
 
 def test_circos_axis_plot(fig_outfile: Path):
     """Test `circos.axis()`"""
```

### Comparing `pycirclize-0.3.0/tests/test_sector.py` & `pycirclize-0.3.1/tests/test_sector.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/test_track.py` & `pycirclize-0.3.1/tests/test_track.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/testdata/eukaryote/hg38/hg38_chr.bed` & `pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_chr.bed`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv` & `pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_cytoband.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv` & `pycirclize-0.3.1/tests/testdata/eukaryote/hg38/hg38_genomic_link.tsv`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/testdata/prokaryote/enterobacteria_phage.gbk` & `pycirclize-0.3.1/tests/testdata/prokaryote/enterobacteria_phage.gbk`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/testdata/prokaryote/enterobacteria_phage.gff` & `pycirclize-0.3.1/tests/testdata/prokaryote/enterobacteria_phage.gff`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/utils/test_dataset.py` & `pycirclize-0.3.1/tests/utils/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/tests/utils/test_helper.py` & `pycirclize-0.3.1/tests/utils/test_helper.py`

 * *Files identical despite different names*

### Comparing `pycirclize-0.3.0/PKG-INFO` & `pycirclize-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycirclize
-Version: 0.3.0
+Version: 0.3.1
 Summary: Circular visualization in Python
 Home-page: https://moshi4.github.io/pyCirclize/
 License: MIT
 Keywords: matplotlib,visualization,bioinformatics,circos,chord-diagram
 Author: moshi4
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Matplotlib
@@ -68,14 +68,15 @@
 API usage is described in each of the following sections in the [document](https://moshi4.github.io/pyCirclize/).
 
 - [Getting Started](https://moshi4.github.io/pyCirclize/getting_started/)
 - [Plot API Example](https://moshi4.github.io/pyCirclize/plot_api_example/)
 - [Chord Diagram](https://moshi4.github.io/pyCirclize/chord_diagram/)
 - [Circos Plot (Genomics)](https://moshi4.github.io/pyCirclize/circos_plot/)
 - [Phylogenetic Tree](https://moshi4.github.io/pyCirclize/phylogenetic_tree/)
+- [Plot Tips](https://moshi4.github.io/pyCirclize/plot_tips/)
 
 ## Code Example
 
 ### 1. Circos Plot
 
 ```python
 from pycirclize import Circos
```

