# Comparing `tmp/PyComplexHeatmap-1.3.8.tar.gz` & `tmp/PyComplexHeatmap-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.3.8.tar", last modified: Mon Mar 27 20:36:17 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.3.9.tar", last modified: Sun Apr  9 03:54:05 2023, max compression
```

## Comparing `PyComplexHeatmap-1.3.8.tar` & `PyComplexHeatmap-1.3.9.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-03-27 20:36:17.556600 PyComplexHeatmap-1.3.8/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       31 2023-02-03 20:34:47.000000 PyComplexHeatmap-1.3.8/.gitattributes
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       13 2023-02-03 20:32:48.000000 PyComplexHeatmap-1.3.8/.gitignore
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1067 2022-05-10 00:26:58.000000 PyComplexHeatmap-1.3.8/LICENSE
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       89 2023-02-08 04:06:17.000000 PyComplexHeatmap-1.3.8/MANIFEST.in
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     7795 2023-03-27 20:36:17.556161 PyComplexHeatmap-1.3.8/PKG-INFO
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-03-27 20:36:17.552972 PyComplexHeatmap-1.3.8/PyComplexHeatmap/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      325 2023-03-27 20:35:22.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap/__init__.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    65517 2023-03-27 20:13:28.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap/annotations.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    69978 2023-03-27 20:32:00.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     5495 2023-03-27 15:50:37.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap/colors.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    30427 2023-03-27 20:32:59.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6766 2023-02-27 16:02:10.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap/example.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     6753 2023-02-24 22:42:08.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap/tools.py
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)    25810 2023-03-15 21:08:42.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        0 2023-03-27 20:36:17.555617 PyComplexHeatmap-1.3.8/PyComplexHeatmap.egg-info/
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     7795 2023-03-27 20:36:16.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      469 2023-03-27 20:36:17.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)        1 2023-03-27 20:36:16.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       17 2023-03-27 20:36:16.000000 PyComplexHeatmap-1.3.8/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     7186 2023-03-27 20:02:47.000000 PyComplexHeatmap-1.3.8/README.md
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)      672 2023-03-27 20:35:15.000000 PyComplexHeatmap-1.3.8/pyproject.toml
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)       38 2023-03-27 20:36:17.556678 PyComplexHeatmap-1.3.8/setup.cfg
--rw-r--r--   0 dingw1   (1300322987) CHOP-EDU\Domain Users (1768498755)     1044 2023-03-27 20:35:04.000000 PyComplexHeatmap-1.3.8/setup.py
+drwxr-xr-x   0 dingw1   (1300322987) 1768498755        0 2023-04-09 03:54:05.699920 PyComplexHeatmap-1.3.9/
+-rw-r--r--   0 dingw1   (1300322987) 1768498755       31 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/.gitattributes
+drwxr-xr-x   0 dingw1   (1300322987) 1768498755        0 2023-04-09 03:54:05.676953 PyComplexHeatmap-1.3.9/.github/
+-rw-r--r--   0 dingw1   (1300322987) 1768498755      810 2023-03-30 00:58:12.000000 PyComplexHeatmap-1.3.9/.github/FUNDING.yml
+-rw-r--r--   0 dingw1   (1300322987) 1768498755       13 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/.gitignore
+-rw-r--r--   0 dingw1   (1300322987) 1768498755     1067 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/LICENSE
+-rw-r--r--   0 dingw1   (1300322987) 1768498755       89 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/MANIFEST.in
+-rw-r--r--   0 dingw1   (1300322987) 1768498755     7981 2023-04-09 03:54:05.699393 PyComplexHeatmap-1.3.9/PKG-INFO
+drwxr-xr-x   0 dingw1   (1300322987) 1768498755        0 2023-04-09 03:54:05.688483 PyComplexHeatmap-1.3.9/PyComplexHeatmap/
+-rw-r--r--   0 dingw1   (1300322987) 1768498755      375 2023-04-09 03:51:12.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 dingw1   (1300322987) 1768498755    65705 2023-04-08 23:51:07.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 dingw1   (1300322987) 1768498755    70043 2023-04-09 02:17:50.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 dingw1   (1300322987) 1768498755     5495 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/colors.py
+-rw-r--r--   0 dingw1   (1300322987) 1768498755    21247 2023-04-08 14:53:33.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 dingw1   (1300322987) 1768498755     6766 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/example.py
+-rw-r--r--   0 dingw1   (1300322987) 1768498755    17624 2023-04-09 03:11:44.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 dingw1   (1300322987) 1768498755     6753 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/tools.py
+-rw-r--r--   0 dingw1   (1300322987) 1768498755    25810 2023-03-29 20:43:55.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 dingw1   (1300322987) 1768498755        0 2023-04-09 03:54:05.698369 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 dingw1   (1300322987) 1768498755     7981 2023-04-09 03:54:04.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 dingw1   (1300322987) 1768498755      519 2023-04-09 03:54:05.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 dingw1   (1300322987) 1768498755        1 2023-04-09 03:54:04.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 dingw1   (1300322987) 1768498755       17 2023-04-09 03:54:04.000000 PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 dingw1   (1300322987) 1768498755     7372 2023-04-09 03:50:27.000000 PyComplexHeatmap-1.3.9/README.md
+-rw-r--r--   0 dingw1   (1300322987) 1768498755      672 2023-04-09 03:51:24.000000 PyComplexHeatmap-1.3.9/pyproject.toml
+-rw-r--r--   0 dingw1   (1300322987) 1768498755       38 2023-04-09 03:54:05.700000 PyComplexHeatmap-1.3.9/setup.cfg
+-rw-r--r--   0 dingw1   (1300322987) 1768498755     1044 2023-04-09 03:51:35.000000 PyComplexHeatmap-1.3.9/setup.py
```

### Comparing `PyComplexHeatmap-1.3.8/LICENSE` & `PyComplexHeatmap-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.8/PKG-INFO` & `PyComplexHeatmap-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.3.8
+Version: 1.3.9
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -49,31 +49,31 @@
 pip install PyComplexHeatmap
 
 #upgrade from older version
 pip install --upgrade PyComplexHeatmap
 ```
 
 2. **Install the developmental version directly from github**:
-```
+```shell
 pip install git+https://github.com/DingWB/PyComplexHeatmap
 ```
 if you have installed it previously and want to update it, please run 
 `pip uninstall PyComplexHeatmap`
 and install from github again
 OR
-```
+```shell
 git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap
 python setup.py install
 ```
 
 ## **Usage**
 ----------------------
 ### **1. Simple Guide To Get started.**
-```
+```py
 from PyComplexHeatmap import *
 
 #Generate example dataset (random)
 df = pd.DataFrame(['GroupA'] * 5 + ['GroupB'] * 5, columns=['AB'])
 df['CD'] = ['C'] * 3 + ['D'] * 3 + ['G'] * 4
 df['EF'] = ['E'] * 6 + ['F'] * 2 + ['H'] * 2
 df['F'] = np.random.normal(0, 1, 10)
@@ -150,14 +150,20 @@
 
 <p align="center">
 <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
 <img src="docs/images/5.jpg" width=500 align="middle">
 </a>
 </p>
 
+<p align="center">
+<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
+<img src="docs/images/6.png" width=600 align="middle">
+</a>
+</p>
+
 ## **More Examples**
 [https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html](https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html)
 
 
 ## Call for Contributions
 ----------------------
```

### Comparing `PyComplexHeatmap-1.3.8/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.3.9/PyComplexHeatmap/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,17 +535,20 @@
         if len(hs) == 0:
             return 0
         else:
             return max(hs)
 # =============================================================================
 class anno_boxplot(AnnotationBase):
     """
-    annotate boxplots, all arguments are included in AnnotationBase,
-    plot_kws for anno_boxplot include showfliers, edgecolor, grid, medianlinecolor
+        annotate boxplots, all arguments are included in AnnotationBase,
+        plot_kws for anno_boxplot include showfliers, edgecolor, grid, medianlinecolor
         width and other arguments passed to plt.boxplot.
+
+    Parameters
+    ----------
     """
 
     def _height(self, height):
         return 8 if height is None else height
 
     def _set_default_plot_kws(self, plot_kws):
         self.plot_kws = plot_kws if plot_kws is not None else {}
@@ -635,14 +638,16 @@
     """
 
     def _set_default_plot_kws(self, plot_kws):
         self.plot_kws = plot_kws if plot_kws is not None else {}
         self.plot_kws.setdefault('edgecolor', 'black')
         self.plot_kws.setdefault('grid', True)
         self.plot_kws.setdefault('zorder', 10)
+        # self.plot_kws.setdefault('width', 0.7)
+        self.plot_kws.setdefault('align', 'center')
 
     def _check_cmap(self, cmap):
         if cmap == 'auto':
             if self.ncols == 1:
                 self.cmap = 'jet'
             else:
                 self.cmap = 'Set1'
@@ -1253,29 +1258,29 @@
             idxs = [self.annotations[0].plot_data.index.tolist()]
         if self.axis == 1:
             nrows = len(self.heights)
             ncols = len(idxs)
             height_ratios = self.heights
             width_ratios = [len(idx) for idx in idxs]
             wspace = gap * mm2inch * self.ax.figure.dpi / (
-                    self.ax.get_window_extent().width / nrows) if wspace is None else wspace  # 1mm=mm2inch inch
+                    self.ax.get_window_extent().width / ncols) if wspace is None else wspace  # 1mm=mm2inch inch
             hspace = 0 if hspace is None else hspace  # fraction of height
         else:
             nrows = len(idxs)
             ncols = len(self.heights)
             width_ratios = self.heights
             height_ratios = [len(idx) for idx in idxs]
             hspace = gap * mm2inch * self.ax.figure.dpi / (
-                    self.ax.get_window_extent().height / ncols) if hspace is None else hspace
+                    self.ax.get_window_extent().height / nrows) if hspace is None else hspace
             wspace = 0 if wspace is None else wspace  # The amount of width reserved for space between subplots, expressed as a fraction of the average axis width
         if subplot_spec is None:
             self.gs = self.ax.figure.add_gridspec(nrows, ncols, hspace=hspace, wspace=wspace,
                                                   height_ratios=height_ratios,
                                                   width_ratios=width_ratios)
-        else:
+        else: #this ax is a subplot of another bigger figure.
             self.gs = matplotlib.gridspec.GridSpecFromSubplotSpec(nrows, ncols, hspace=hspace, wspace=wspace,
                                                                   subplot_spec=subplot_spec,
                                                                   height_ratios=height_ratios,
                                                                   width_ratios=width_ratios)
         self.axes = np.empty(shape=(nrows, ncols), dtype=object)
         self.fig = self.ax.figure
         self.ax.set_axis_off()
```

### Comparing `PyComplexHeatmap-1.3.8/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.3.9/PyComplexHeatmap/clustermap.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,20 +638,22 @@
         mask the data in heatmap, the cell with missing values of infinite values will be masked automatically.
     subplot_gap :float
         the gap between subplots, default is 1mm.
     legend :bool
         True or False, whether to plot heatmap legend, determined by cmap.
     legend_kws :dict
         kws passed to plot legend. If one want to change the outline color and linewidth of cbar:
+        ```
         for cbar in cm.cbars:
             if isinstance(cbar,matplotlib.colorbar.Colorbar):
                 cbar.outline.set_color('white')
                 cbar.outline.set_linewidth(2)
                 cbar.dividers.set_color('red')
                 cbar.dividers.set_linewidth(2)
+        ```
     plot :bool
         whether to plot or not.
     plot_legend :bool
         True or False, whether to plot legend, if False, legends can be plot with
         ClusterMapPlotter.plot_legends()
     legend_anchor :str
         ax_heatmap or ax, the ax to which legend anchor.
@@ -689,22 +691,21 @@
                  top_annotation=None, bottom_annotation=None, left_annotation=None, right_annotation=None,
                  row_cluster=True, col_cluster=True, row_cluster_method='average', row_cluster_metric='correlation',
                  col_cluster_method='average', col_cluster_metric='correlation',
                  show_rownames=False, show_colnames=False, row_names_side='right', col_names_side='bottom',
                  row_dendrogram=False, col_dendrogram=False, row_dendrogram_size=10, col_dendrogram_size=10,
                  row_split=None, col_split=None, dendrogram_kws=None, tree_kws=None,
                  row_split_order=None, col_split_order=None, row_split_gap=0.5, col_split_gap=0.2, mask=None,
-                 subplot_gap=1, legend=True, legend_kws=None, plot=True, plot_legend=True,
+                 subplot_gap=3, legend=True, legend_kws=None, plot=True, plot_legend=True,
                  legend_anchor='auto', legend_gap=5, legend_width=4.5, legend_hpad=2, legend_vpad=5,
                  legend_side='right', cmap='jet', label=None, xticklabels_kws=None, yticklabels_kws=None,
                  rasterized=False, legend_delta_x=None, verbose=1, **kwargs):
         self.kwargs = kwargs if not kwargs is None else {}
-        self.data2d = self.format_data(data, z_score, standard_scale)
+        self.data2d = self.format_data(data, mask, z_score, standard_scale)
         self.verbose=verbose
-        self.mask = _check_mask(self.data2d, mask)
         self._define_kws(xticklabels_kws, yticklabels_kws)
         self.top_annotation = top_annotation
         self.bottom_annotation = bottom_annotation
         self.left_annotation = left_annotation
         self.right_annotation = right_annotation
         self.row_dendrogram_size = row_dendrogram_size
         self.col_dendrogram_size = col_dendrogram_size
@@ -758,24 +759,25 @@
 
     def _define_kws(self, xticklabels_kws, yticklabels_kws):
         self.yticklabels_kws = {} if yticklabels_kws is None else yticklabels_kws
         # self.yticklabels_kws.setdefault('labelrotation', 0)
         self.xticklabels_kws = {} if xticklabels_kws is None else xticklabels_kws
         # self.xticklabels_kws.setdefault('labelrotation', 90)
 
-    def format_data(self, data, z_score=None, standard_scale=None):
+    def format_data(self, data, mask=None, z_score=None, standard_scale=None):
         data2d = data.copy()
         self.kwargs.setdefault('vmin', np.nanmin(data.values))
         self.kwargs.setdefault('vmax', np.nanmax(data.values))
         if z_score is not None and standard_scale is not None:
             raise ValueError('Cannot perform both z-scoring and standard-scaling on data')
         if z_score is not None:
             data2d = self.z_score(data, z_score)
         if standard_scale is not None:
             data2d = self.standard_scale(data, standard_scale)
+        self.mask = _check_mask(data2d, mask)
         return data2d
 
     def _define_gs_ratio(self):
         self.top_heights = []
         self.bottom_heights = []
         self.left_widths = []
         self.right_widths = []
@@ -1134,17 +1136,17 @@
 
     def plot_matrix(self, row_order, col_order):
         if self.verbose >= 1:
             print("Plotting matrix..")
         nrows = len(row_order)
         ncols = len(col_order)
         self.wspace = self.col_split_gap * mm2inch * self.ax.figure.dpi / (
-                self.ax_heatmap.get_window_extent().width / nrows)  # 1mm=mm2inch inch
+                self.ax_heatmap.get_window_extent().width / ncols)  # 1mm=mm2inch inch
         self.hspace = self.row_split_gap * mm2inch * self.ax.figure.dpi / (
-                self.ax_heatmap.get_window_extent().height / ncols)
+                self.ax_heatmap.get_window_extent().height / nrows) #height
         self.heatmap_gs = matplotlib.gridspec.GridSpecFromSubplotSpec(nrows, ncols, hspace=self.hspace,
                                                                       wspace=self.wspace,
                                                                       subplot_spec=self.gs[1, 1],
                                                                       height_ratios=[len(rows) for rows in row_order],
                                                                       width_ratios=[len(cols) for cols in col_order])
 
         annot = self.kwargs.pop("annot", None)
@@ -1374,15 +1376,16 @@
     legend_side: str
         right,left [right].
     legend_gap: float
         row gap between two legends, unit is mm.
 
     Returns
     -------
-    legend_axes
+    tuple:
+        ax,legend_axes
 
     """
     if ax is None:
         ax = plt.gca()
     n = len(cmlist)
     wspace, hspace = 0, 0
     if axis == 1:  # horizontally
@@ -1437,11 +1440,11 @@
     legend_axes, cbars,boundry = \
         plot_legend_list(legend_list, ax=ax, space=space,
                         legend_side=legend_side, gap=legend_gap,
                          y0=legend_y,legend_width=legend_width)
     ax.set_axis_off()
     # import pdb;
     # pdb.set_trace()
-    return legend_axes
+    return ax,legend_axes
 # =============================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `PyComplexHeatmap-1.3.8/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.3.9/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.8/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.3.9/PyComplexHeatmap/dotHeatmap.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     delta=vmax - vmin
     return [(j - vmin) / delta for j in values]
 # =============================================================================
 def dotHeatmap2d(data, hue=None, vmin=None, vmax=None, ax=None,
                  colors=None, cmap=None, ratio=None,spines=False, **kwargs):
     """
     Plot dot heatmap using a dataframe matrix as input.
+
     Parameters
     ----------
     data : pd.DataFrame
         input matrix (pandas.DataFrame)
     hue : pd.DataFrame
         hue to control the colors and cmap of the dot.
     vmin : float
@@ -192,198 +193,18 @@
     ax.set_xticklabels(col_labels)
     if not spines:
         despine(ax=ax, left=True, bottom=True, right=True, top=True)
         # for side in ["top", "right", "left", "bottom"]:
         #     ax.spines[side].set_visible(False)
     return ax
 # =============================================================================
-def dotHeatmap(data=None, x=None, y=None, value=None, hue=None,
-               row_order=None,col_order=None,
-               colors=None, cmap=None, ax=None,
-               show_rownames=True, show_colnames=True,alpha=1,
-               plot_legend=True,legend_side='right',label_side='left',
-               legend_hpad=3,legend_width=4.5,legend_vpad=5,
-               legend_gap=5,color_legend_kws={},
-               dot_legend_kws={},cmap_legend_kws={},**kwargs):
-    """
-    Plot dot heatmap using different columns of dataframe `data`.
-
-    Parameters
-    ----------
-    data : DataFrame
-        a dataframe containing multiple columns.
-    x : str
-        column name in data.columns, used to show on the xaxis of dot heatmap.
-    y : str
-        column name in data.columns, used to show on the yaxis of dot heatmap.
-    value : str
-        column name in data.columns, used to control the color and size of dot.
-    hue : str
-        column name in data.columns, used to control the color and cmap of dot.
-    row_order : list
-        row order should be the order of values in data[y].values
-    col_order : list
-        col order should be the order of values in data[x].values
-    colors : str or dict
-        a string or dict do control the colors of dot, could be used with hue, default is None.
-    cmap : string or dict
-        cmap to control the color of dot, could be used together with hue and colors.
-    ax : matplotlib.axes
-        ax
-    show_rownames : bool
-        whether to show row names, default is True.
-    show_colnames : bool
-        whether to show col names, default is True.
-    alpha: float [0,1]
-        coefficient to scale the size of dot in figure legend, valid for marker and dot in legend.
-    plot_legend : bool
-        whether to plot legend, default is True.
-    legend_side : str
-        legend side, default is right.
-    label_side : str
-        label side of y tick labels, default is left.
-    legend_hpad : float
-        horizonal pad between legend and main figure.
-    legend_width : float
-        width of legend.
-    legend_vpad : float
-        vertical pad between legend and the top of main figure.
-    legend_gap : float
-        vertical gap between two legends.
-    color_legend_kws : dict
-        legend_kws passed to `plot_color_dict_legend`.
-    dot_legend_kws : dict
-        legend_kws passed to `plot_marker_legend`.
-    cmap_legend_kws : dict
-        legend_kws passed to `plot_cmap_legend`.
-    kwargs : dict
-        others kwargs passed to plt.scatter, such as linewidths, edgecolor, alphia and so on.
-
-    Returns
-    -------
-
-    ax
-    """
-    marker = kwargs.get('marker', 'o')  # https://matplotlib.org/stable/api/markers_api.html#module-matplotlib.markers
-    color_dict=None
-
-    # fig, ax = plt.subplots(figsize=(6,6))
-    if ax is None:
-        ax = plt.gca()
-    col_order = data[x].unique().tolist() if col_order is None else col_order
-    row_order = data[y].unique().tolist() if row_order is None else row_order
-    df = data[x].apply(lambda j: col_order.index(j) + 1).to_frame(name='X')
-    df['Y'] = data[y].apply(lambda j: row_order.index(j) + 1)
-    # df=data.pivot_table(index=x,columns=y,values=value,aggfunc=np.mean)
-
-    w, h = ax.get_window_extent().width / ax.figure.dpi, ax.get_window_extent().height / ax.figure.dpi
-    r = min(w * 72 / len(col_order), h * 72 / len(row_order))
-
-    df['S'] = kwargs.pop('s', scale(data[value].values))
-
-    # print(kwargs)
-    if type(cmap) != dict and type(marker) == str:
-        if not colors is None and type(colors)==str:
-            kwargs['c']=colors
-        if 'c' in kwargs:
-            df['C'] = kwargs.pop('c')
-        elif not hue is None:
-            if colors is None:  #
-                color_dict = {}
-                col_list = data[hue].value_counts().index.tolist()
-                for c in col_list:
-                    color_dict[c] = matplotlib.colors.to_hex(plt.get_cmap(cmap)(col_list.index(c)))
-            elif type(colors) == dict:
-                color_dict = colors
-            elif type(colors) == str:
-                col_list = data[hue].value_counts().index.tolist()
-                for c in col_list:
-                    color_dict[c] = colors
-            else:
-                raise ValueError('colors must be string or dict')
-
-            df['C'] = data[hue].map(color_dict)
-        else:
-            df['C'] = scale(data[value].values)
-            # kwargs.setdefault('norm',matplotlib.colors.Normalize(vmin=vmin, vmax=vmax))
-            kwargs.setdefault('cmap', cmap)
-        ax.scatter(x=df.X.values, y=df.Y.values, s=df.S * (r ** 2),
-                   c=df.C.values, **kwargs)  #
-    elif type(cmap) == dict and not hue is None:
-        for h in cmap:  # key are hue, values are cmap
-            df1 = df.loc[data[hue] == h]
-            # df1['C']=kwargs.pop('c',scale(df1.S.values))
-            df1.insert(0, 'C', kwargs.pop('c', scale(df1.S.values)))
-            kwargs['cmap'] = cmap[h]
-            if type(marker) == dict:
-                kwargs['marker'] = marker[h]
-            ax.scatter(x=df1.X.values, y=df1.Y.values, s=df1.S * (r ** 2),
-                       c=df1.C.values, **kwargs)  #
-    else:
-        raise ValueError('cmap must be string or dict')
-
-    ax.set_ylim([0.5, len(row_order) + 0.5])
-    ax.set_xlim(0.5, len(col_order) + 0.5)
-    y_locater = list(range(1, len(row_order) + 1))
-    x_locater = list(range(1, len(col_order) + 1))
-    ax.yaxis.set_major_locator(plt.FixedLocator(y_locater))
-    ax.yaxis.set_minor_locator(plt.FixedLocator(np.array(y_locater) - 0.5))
-    ax.xaxis.set_major_locator(plt.FixedLocator(x_locater))
-    ax.xaxis.set_minor_locator(plt.FixedLocator(np.array(x_locater) - 0.5))
-    #    ax.yaxis.set_major_formatter(plt.FixedFormatter(df.index.values))
-    #    majorLocator = MultipleLocator(1)
-    #    ax.yaxis.set_major_locator(majorLocator)
-    if show_colnames:
-        ax.set_yticklabels(row_order)
-    if show_rownames:
-        ax.set_xticklabels(col_order, rotation=-90)
-    # ax.grid(which='minor',color='white',linestyle='-',alpha=0.6)
-    ax.tick_params(axis='both', which='both',
-                   left=False, right=False, labelleft=True, labelright=False,
-                   top=False, bottom=False, labeltop=False, labelbottom=True)
-    if plot_legend:
-        legend_list=[]
-        if not color_dict is None and not hue is None:
-            legend_list.append([color_dict, hue, color_legend_kws, len(color_dict), 'color_dict'])
-        if type(cmap)==str and colors is None:
-            legend_list.append([cmap, value, cmap_legend_kws, 4, 'cmap'])
-        if type(cmap)==dict:
-            for k in cmap:
-                legend_list.append([cmap[k], k, cmap_legend_kws, 4, 'cmap'])
-        if type(marker)==dict and not hue is None:
-            legend_list.append([(marker,colors,r*alpha), hue, dot_legend_kws, len(marker), 'markers']) #markersize is r*0.8
-        # dot size legend:
-        if 's' not in kwargs:
-            max_s=np.nanmax(data[value].values)
-            markers1={}
-            ms={}
-            for f in [1,0.8,0.6,0.4,0.2]:
-                k=str(round(f*max_s,2))
-                markers1[k]='o'
-                ms[k]=f * r * alpha
-            legend_list.append([(markers1, colors, ms), value, dot_legend_kws, len(markers1), 'markers'])
-        label_width=ax.yaxis.label.get_window_extent(renderer=ax.figure.canvas.get_renderer()).width
-        yticklabels = ax.yaxis.get_ticklabels()
-        if len(yticklabels) == 0:
-            ticklabel_width=0
-        else:
-            ticklabel_width=max([label.get_window_extent(renderer=ax.figure.canvas.get_renderer()).width
-                 for label in ax.yaxis.get_ticklabels()])
-        if len(legend_list) > 0:
-            space = max([label_width,ticklabel_width]) if (legend_side == 'right' and label_side == 'right') else 0
-            legend_hpad = legend_hpad * mm2inch * ax.figure.dpi  # mm to inch to pixel
-            legend_axes, cbars, boundry = plot_legend_list(legend_list, ax=ax, space=space + legend_hpad,
-                                 legend_side='right', gap=legend_gap,
-                                 legend_width=legend_width, legend_vpad=legend_vpad)
-    return ax
-# =============================================================================
 class DotClustermapPlotter(ClusterMapPlotter):
     """
     DotClustermap (Heatmap) plotter, inherited from ClusterMapPlotter.
-    Plot dot heatmap / clustermap with annotation and legends.
+    Plot dot heatmap (clustermap) with annotation and legends.
 
     Parameters
     ----------
     data : dataframe
         pandas dataframe or numpy array.
     x: str
         The column name in data.columns to be shown on the columns of heatmap / clustermap.
@@ -435,16 +256,17 @@
         when there are multiple values for the same x and y, using aggfunc (default is np.mean) to aggregate them.
         aggfunc will be called in data.pivot(index=y,columns=x,values=value,aggfunc=aggfunc)
     kwargs :dict
         Other kwargs passed to ClusterMapPlotter.
 
     Returns
     -------
-    Class DotClustermapPlotter.
+    DotClustermapPlotter.
     """
+
     def __init__(self, data=None, x=None, y=None, value=None, hue=None,
                  s=None,c=None,marker='o',alpha=0.8,
                  color_legend_kws={},cmap_legend_kws={},
                  dot_legend_kws={},aggfunc=np.mean,
                  value_na=0,hue_na='NA',s_na=0,c_na=0,
                  spines=False,**kwargs):
         kwargs['data']=data
@@ -464,15 +286,15 @@
         self.color_legend_kws=color_legend_kws
         self.cmap_legend_kws=cmap_legend_kws
         self.spines=spines
         self.dot_legend_kws=dot_legend_kws
 
         super().__init__(**kwargs)
 
-    def format_data(self, data, z_score=None, standard_scale=None):
+    def format_data(self, data, mask=None,z_score=None, standard_scale=None):
         # self.data=data
         data2d = data.pivot_table(index=self.y,columns=self.x,values=self.value,aggfunc=self.aggfunc).fillna(self.value_na)
         # hue
         if not self.hue is None:
             self.kwargs['hue']=data.pivot(index=self.y,columns=self.x,values=self.hue).fillna(self.hue_na)
         # s
         if not self.s is None:
@@ -530,32 +352,32 @@
 
     def plot_matrix(self, row_order, col_order):
         if self.verbose >= 1:
             print("Plotting matrix..")
         nrows = len(row_order)
         ncols = len(col_order)
         self.wspace = self.col_split_gap * mm2inch * self.ax.figure.dpi / (
-                self.ax_heatmap.get_window_extent().width / nrows)  # 1mm=mm2inch inch
+                self.ax_heatmap.get_window_extent().width / ncols)  # 1mm=mm2inch inch
         self.hspace = self.row_split_gap * mm2inch * self.ax.figure.dpi / (
-                self.ax_heatmap.get_window_extent().height / ncols)
+                self.ax_heatmap.get_window_extent().height / nrows) #height
         self.heatmap_gs = matplotlib.gridspec.GridSpecFromSubplotSpec(nrows, ncols, hspace=self.hspace,
                                                                       wspace=self.wspace,
                                                                       subplot_spec=self.gs[1, 1],
                                                                       height_ratios=[len(rows) for rows in row_order],
                                                                       width_ratios=[len(cols) for cols in col_order])
         self.heatmap_axes = np.empty(shape=(nrows, ncols), dtype=object)
         # if nrows > 1 or ncols > 1:
         self.ax_heatmap.set_axis_off()
         for i, rows in enumerate(row_order):
             for j, cols in enumerate(col_order):
                 ax1 = self.ax_heatmap.figure.add_subplot(self.heatmap_gs[i, j],
                                                         sharex=self.heatmap_axes[0, j],
                                                         sharey=self.heatmap_axes[i, 0])
-                ax1.set_xlim([0, len(rows)])
-                ax1.set_ylim([0, len(cols)])
+                # ax1.set_xlim([0, len(rows)])
+                # ax1.set_ylim([0, len(cols)])
                 kwargs=self.kwargs.copy()
                 # print(kwargs)
                 dotHeatmap2d(self.data2d.loc[rows, cols],
                              cmap=kwargs.pop('cmap',self.cmap),ax=ax1,
                              spines=self.spines,**kwargs)
                 self.heatmap_axes[i, j] = ax1
                 ax1.yaxis.label.set_visible(False)
@@ -619,32 +441,14 @@
             heatmap_label_max_width = max([label.get_window_extent().width for label in self.yticklabels]) if len(
                 self.yticklabels) > 0 else 0
             if heatmap_label_max_width >= self.label_max_width or self.legend_anchor == 'ax_heatmap':
                 self.label_max_width = heatmap_label_max_width * 1.1
             if len(self.legend_list) > 1:
                 self.legend_list = sorted(self.legend_list, key=lambda x: x[3])
 
-    def plot_legends(self, ax=None):
-        if self.verbose >= 1:
-            print("Plotting legends..")
-        if len(self.legend_list) > 0:
-            if self.legend_side == 'right' and not self.right_annotation is None:
-                space = self.label_max_width
-            elif self.legend_side == 'right' and self.show_rownames and self.row_names_side=='right':
-                space = self.label_max_width
-            else:
-                space=0
-
-            legend_hpad = self.legend_hpad * mm2inch * self.ax.figure.dpi
-            self.legend_axes, self.cbars,self.boundry = \
-                plot_legend_list(self.legend_list, ax=ax, space=space + legend_hpad,
-                                  legend_side=self.legend_side, gap=self.legend_gap,
-                                  delta_x=self.legend_delta_x,legend_width=self.legend_width,
-                                 legend_vpad=self.legend_vpad)
-
     def post_processing(self):
         if not self.spines:
             for ax in self.heatmap_axes.ravel():
                 despine(ax=ax, left=True, bottom=True, right=True, top=True)
 
 if __name__ == "__main__":
     pass
```

### Comparing `PyComplexHeatmap-1.3.8/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.3.9/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.8/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.3.9/PyComplexHeatmap/tools.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.8/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.3.9/PyComplexHeatmap/utils.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.3.8/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.3.9/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.3.8
+Version: 1.3.9
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -49,31 +49,31 @@
 pip install PyComplexHeatmap
 
 #upgrade from older version
 pip install --upgrade PyComplexHeatmap
 ```
 
 2. **Install the developmental version directly from github**:
-```
+```shell
 pip install git+https://github.com/DingWB/PyComplexHeatmap
 ```
 if you have installed it previously and want to update it, please run 
 `pip uninstall PyComplexHeatmap`
 and install from github again
 OR
-```
+```shell
 git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap
 python setup.py install
 ```
 
 ## **Usage**
 ----------------------
 ### **1. Simple Guide To Get started.**
-```
+```py
 from PyComplexHeatmap import *
 
 #Generate example dataset (random)
 df = pd.DataFrame(['GroupA'] * 5 + ['GroupB'] * 5, columns=['AB'])
 df['CD'] = ['C'] * 3 + ['D'] * 3 + ['G'] * 4
 df['EF'] = ['E'] * 6 + ['F'] * 2 + ['H'] * 2
 df['F'] = np.random.normal(0, 1, 10)
@@ -150,14 +150,20 @@
 
 <p align="center">
 <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
 <img src="docs/images/5.jpg" width=500 align="middle">
 </a>
 </p>
 
+<p align="center">
+<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
+<img src="docs/images/6.png" width=600 align="middle">
+</a>
+</p>
+
 ## **More Examples**
 [https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html](https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html)
 
 
 ## Call for Contributions
 ----------------------
```

### Comparing `PyComplexHeatmap-1.3.8/README.md` & `PyComplexHeatmap-1.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,31 +33,31 @@
 pip install PyComplexHeatmap
 
 #upgrade from older version
 pip install --upgrade PyComplexHeatmap
 ```
 
 2. **Install the developmental version directly from github**:
-```
+```shell
 pip install git+https://github.com/DingWB/PyComplexHeatmap
 ```
 if you have installed it previously and want to update it, please run 
 `pip uninstall PyComplexHeatmap`
 and install from github again
 OR
-```
+```shell
 git clone https://github.com/DingWB/PyComplexHeatmap
 cd PyComplexHeatmap
 python setup.py install
 ```
 
 ## **Usage**
 ----------------------
 ### **1. Simple Guide To Get started.**
-```
+```py
 from PyComplexHeatmap import *
 
 #Generate example dataset (random)
 df = pd.DataFrame(['GroupA'] * 5 + ['GroupB'] * 5, columns=['AB'])
 df['CD'] = ['C'] * 3 + ['D'] * 3 + ['G'] * 4
 df['EF'] = ['E'] * 6 + ['F'] * 2 + ['H'] * 2
 df['F'] = np.random.normal(0, 1, 10)
@@ -134,14 +134,20 @@
 
 <p align="center">
 <a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/composite_heatmaps.html#Composite-two-heatmaps-horizontally-for-mouse-DNA-methylation-array-dataset">
 <img src="docs/images/5.jpg" width=500 align="middle">
 </a>
 </p>
 
+<p align="center">
+<a href="https://dingwb.github.io/PyComplexHeatmap/build/html/notebooks/oncoPrint.html">
+<img src="docs/images/6.png" width=600 align="middle">
+</a>
+</p>
+
 ## **More Examples**
 [https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html](https://dingwb.github.io/PyComplexHeatmap/build/html/more_examples.html)
 
 
 ## Call for Contributions
 ----------------------
```

### Comparing `PyComplexHeatmap-1.3.8/pyproject.toml` & `PyComplexHeatmap-1.3.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `PyComplexHeatmap-1.3.8/setup.py` & `PyComplexHeatmap-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.3.8',
+   version='1.3.9',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

