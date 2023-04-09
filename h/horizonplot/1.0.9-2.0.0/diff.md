# Comparing `tmp/horizonplot-1.0.9.tar.gz` & `tmp/horizonplot-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/horizonplot-1.0.9.tar", last modified: Fri Dec  4 10:42:02 2020, max compression
+gzip compressed data, was "horizonplot-2.0.0.tar", last modified: Sun Apr  9 13:00:00 2023, max compression
```

## Comparing `horizonplot-1.0.9.tar` & `horizonplot-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2020-12-04 10:42:02.000000 horizonplot-1.0.9/
--rw-r--r--   0 kmt        (501) staff       (20)      283 2020-12-04 10:42:02.000000 horizonplot-1.0.9/PKG-INFO
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2020-12-04 10:42:02.000000 horizonplot-1.0.9/horizonplot/
--rw-r--r--   0 kmt        (501) staff       (20)     7536 2020-12-04 10:38:12.000000 horizonplot-1.0.9/horizonplot/__init__.py
--rw-r--r--   0 kmt        (501) staff       (20)      169 2020-12-03 12:58:39.000000 horizonplot-1.0.9/README.md
-drwxr-xr-x   0 kmt        (501) staff       (20)        0 2020-12-04 10:42:02.000000 horizonplot-1.0.9/horizonplot.egg-info/
--rw-r--r--   0 kmt        (501) staff       (20)      283 2020-12-04 10:42:02.000000 horizonplot-1.0.9/horizonplot.egg-info/PKG-INFO
--rw-r--r--   0 kmt        (501) staff       (20)      216 2020-12-04 10:42:02.000000 horizonplot-1.0.9/horizonplot.egg-info/SOURCES.txt
--rw-r--r--   0 kmt        (501) staff       (20)       52 2020-12-04 10:42:02.000000 horizonplot-1.0.9/horizonplot.egg-info/requires.txt
--rw-r--r--   0 kmt        (501) staff       (20)       12 2020-12-04 10:42:02.000000 horizonplot-1.0.9/horizonplot.egg-info/top_level.txt
--rw-r--r--   0 kmt        (501) staff       (20)        1 2020-12-04 10:42:02.000000 horizonplot-1.0.9/horizonplot.egg-info/dependency_links.txt
--rw-r--r--   0 kmt        (501) staff       (20)      503 2020-12-04 10:40:12.000000 horizonplot-1.0.9/setup.py
--rw-r--r--   0 kmt        (501) staff       (20)       38 2020-12-04 10:42:02.000000 horizonplot-1.0.9/setup.cfg
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-09 13:00:00.666257 horizonplot-2.0.0/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)    35141 2023-04-09 12:57:40.000000 horizonplot-2.0.0/LICENSE
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      249 2023-04-09 13:00:00.655257 horizonplot-2.0.0/PKG-INFO
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      169 2023-04-09 12:57:40.000000 horizonplot-2.0.0/README.md
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-09 12:59:59.844242 horizonplot-2.0.0/horizonplot/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)     8032 2023-04-09 12:57:40.000000 horizonplot-2.0.0/horizonplot/__init__.py
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-09 13:00:00.583256 horizonplot-2.0.0/horizonplot.egg-info/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      249 2023-04-09 12:59:58.000000 horizonplot-2.0.0/horizonplot.egg-info/PKG-INFO
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      224 2023-04-09 12:59:58.000000 horizonplot-2.0.0/horizonplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)        1 2023-04-09 12:59:58.000000 horizonplot-2.0.0/horizonplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       52 2023-04-09 12:59:58.000000 horizonplot-2.0.0/horizonplot.egg-info/requires.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       12 2023-04-09 12:59:58.000000 horizonplot-2.0.0/horizonplot.egg-info/top_level.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       38 2023-04-09 13:00:00.682257 horizonplot-2.0.0/setup.cfg
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      503 2023-04-09 12:57:40.000000 horizonplot-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `horizonplot-1.0.9/horizonplot/__init__.py` & `horizonplot-2.0.0/horizonplot/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,46 +59,53 @@
 
 def round_to_1_signif(x):
     """
     Rounds to first significant digit.
     """
     return round(x, -int(floor(log10(abs(x)))))
     
-def horizonplot(df, key, width, cut='fixed', start='start', col='chrom', row='pop',
+def horizonplot(df, key, width, 
+                cut=None, # float, takes precedence over quantile_span
+                quantile_span = None, # tuple: (0.05, 0.95)
+                start='start', col='chrom', row='pop',
                 beginzero=False, pop_sorting=None, size=0.5, aspect=40,
-                colours = sns.color_palette("Blues", 3) + ['midnightblue'] + \
-                          sns.color_palette("Reds", 3) + ['darkred'] + ['lightgrey']):
+                colors = ['#CCE2DF', '#59A9A8', '#374E9B', 'midnightblue',
+                          '#F2DE9A', '#DA8630', '#972428', 'darkred',
+                          '#D3D3D3']):
+                # colours = ['#314E9F', '#36AAA8', '#D7E2D4'] + ['midnightblue'] + \
+                #           ['#F5DE90', '#F5DE90', '#A51023'] + ['darkred'] + ['whitesmoke']):
+                # colors = sns.color_palette("Blues", 3) + ['midnightblue'] + \
+                #           sns.color_palette("Reds", 3) + ['darkred'] + ['lightgrey']):
+
     """
     Horizon bar plot made allowing multiple chromosomes and multiple samples.
     """
 
     pop, chrom = row, col
         
     # set cut if not set
-    if cut is 'fixed':
+    if cut is not None:
         cut = np.max([np.max(df[key]), np.max(-df[key])]) / 3
-
-    # TODO: cut should be either:
-    # value applied to all
-    # 'fixed' (default) computing a shared cutoff for all rows
-    # 'adaptive' computing a cutoff that fits each row.
+    elif quantile_span:
+        cut=max(np.abs(np.nanquantile(df[col], quantile_span[0])), 
+                np.abs(np.nanquantile(df[col], quantile_span[1]))) / 3,
 
     # make the data frame to plot
     row_iter = df.itertuples()
     col_iterators = zip(*(horizon(row, key, cut) for row in row_iter))
     col_names = ['yp1', 'yp2', 'yp3', 'yp4', 
                  'yn1', 'yn2', 'yn3', 'yn4', 'nan']
 
     df2 = (df[[key, start, chrom, pop]]
            .assign(**dict(zip(col_names, col_iterators)))
           )
 
     df3 = pd.DataFrame(dict((col, list(chain.from_iterable(zip(df2[col].values, df2[col].values)))) for col in df2))
     #df3[start] = list(df3[start].values[1:]) + [df3[start].values[-1] + width]
-    df3[start] = df3.groupby(row).start.apply(lambda sr: pd.concat([sr.iloc[1:], pd.Series([df3[start].iloc[-1] + width])])).values
+    df3[start] = df3.groupby(row, sort=False).start.apply(lambda sr: pd.concat([sr.iloc[1:], pd.Series([df3[start].iloc[-1] + width])])).values
 
     df2 = df3
 
     # chromosome names
     chrom_names = list(df.groupby(chrom).groups.keys())
     sorted_chrom_names = sorted(chrom_names, key=chrom_sort)
     
@@ -136,22 +143,22 @@
                             row_order=pop_sorting,                      
                             gridspec_kws={'hspace':0.0, 'width_ratios': facet_widths_ratios}
                             )
 
             # first y tick
             ytic1 = round_to_1_signif(cut / 3)
 
-            for col_name, colour in zip(col_names, colours):
+            for col_name, color in zip(col_names, colors):
                 plt.setp(g.fig.texts, text="") # hack to make y facet labels align...
                 # map barplots to each facet
                 g.map(plt.fill_between, 
                     start, 
                     col_name, 
                     y2=0,
-                    color=colour,
+                    color=color,
                     linewidth=0,
                     capstyle='butt')
 
             # g.set_ylabels('')
 
             def add_pop_labels(pop_label, **kwargs):
                 # only rightmosts facets:
```

