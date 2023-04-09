# Comparing `tmp/cellsnake-0.2.0.dev7.tar.gz` & `tmp/cellsnake-0.2.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellsnake-0.2.0.dev7.tar", last modified: Tue Apr  4 10:07:25 2023, max compression
+gzip compressed data, was "cellsnake-0.2.0.dev8.tar", last modified: Sun Apr  9 00:36:01 2023, max compression
```

## Comparing `cellsnake-0.2.0.dev7.tar` & `cellsnake-0.2.0.dev8.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.028516 cellsnake-0.2.0.dev7/
--rw-r--r--   0 sium       (501) staff       (20)     1072 2022-12-02 21:30:51.000000 cellsnake-0.2.0.dev7/LICENSE
--rw-r--r--   0 sium       (501) staff       (20)      300 2023-02-22 13:59:41.000000 cellsnake-0.2.0.dev7/MANIFEST.in
--rw-r--r--   0 sium       (501) staff       (20)     4907 2023-04-04 10:07:25.028214 cellsnake-0.2.0.dev7/PKG-INFO
--rw-r--r--   0 sium       (501) staff       (20)     4459 2023-03-03 23:32:18.000000 cellsnake-0.2.0.dev7/README.md
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:24.999123 cellsnake-0.2.0.dev7/cellsnake/
--rw-r--r--   0 sium       (501) staff       (20)        0 2022-12-02 21:33:29.000000 cellsnake-0.2.0.dev7/cellsnake/__init__.py
--rw-r--r--   0 sium       (501) staff       (20)        0 2023-02-01 12:33:26.000000 cellsnake-0.2.0.dev7/cellsnake/cellsnake_functions.py
--rwxr-xr-x   0 sium       (501) staff       (20)    13703 2023-04-04 10:02:45.000000 cellsnake-0.2.0.dev7/cellsnake/command_line.py
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.001026 cellsnake-0.2.0.dev7/cellsnake/scrna/
--rw-r--r--   0 sium       (501) staff       (20)     2362 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/config.yaml
--rwxr-xr-x   0 sium       (501) staff       (20)       55 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/install_r_packages.sh
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.001619 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/
--rw-r--r--   0 sium       (501) staff       (20)    22087 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/Snakefile
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.002179 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/bundle/
--rw-r--r--   0 sium       (501) staff       (20)  2786711 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:24.993888 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.007032 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.007286 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/
--rw-r--r--   0 sium       (501) staff       (20)     8522 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4148 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py
--rwxr-xr-x   0 sium       (501) staff       (20)     8607 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/k2sc.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4158 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.010091 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/
--rw-r--r--   0 sium       (501) staff       (20)     2179 2023-02-08 21:49:02.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/extra_functions.smk
--rw-r--r--   0 sium       (501) staff       (20)      351 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/integration.smk
--rw-r--r--   0 sium       (501) staff       (20)     5712 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/microbiome.smk
--rw-r--r--   0 sium       (501) staff       (20)     1050 2022-12-02 22:51:49.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/params_detect.smk
--rw-r--r--   0 sium       (501) staff       (20)      181 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/params_write.smk
--rw-r--r--   0 sium       (501) staff       (20)    19533 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/seurat.smk
--rw-r--r--   0 sium       (501) staff       (20)     1337 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/test.smk
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.027623 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/
--rwxr-xr-x   0 sium       (501) staff       (20)     3016 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-cellchat.R
--rwxr-xr-x   0 sium       (501) staff       (20)    17388 2023-02-27 13:17:03.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3319 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-celltypist.R
--rwxr-xr-x   0 sium       (501) staff       (20)      761 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-celltypist.py
--rwxr-xr-x   0 sium       (501) staff       (20)     4459 2023-02-28 14:02:58.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1132 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1108 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3449 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-dimplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1828 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-dotplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1716 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-find-markers.R
--rwxr-xr-x   0 sium       (501) staff       (20)     6918 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-functions.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3205 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2212 2023-02-20 22:44:59.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-gsea.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2945 2022-12-03 20:20:58.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-harmony.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2648 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-install-packages.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4595 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-kegg.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4464 2023-01-31 11:27:53.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py
--rwxr-xr-x   0 sium       (501) staff       (20)     2937 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1952 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3289 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1253 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2461 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-metrics.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2835 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     3375 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2497 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-monocle3.R
--rwxr-xr-x   0 sium       (501) staff       (20)        0 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-music-decon.R
--rwxr-xr-x   0 sium       (501) staff       (20)     6558 2023-03-22 10:39:26.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R
--rwxr-xr-x   0 sium       (501) staff       (20)     6894 2023-03-22 10:39:26.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-read-qc.R
--rwxr-xr-x   0 sium       (501) staff       (20)     4568 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2068 2023-04-04 09:59:25.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R
--rwxr-xr-x   0 sium       (501) staff       (20)     2636 2023-03-22 10:39:26.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1305 2023-03-22 10:39:26.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1363 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-technicals.R
--rwxr-xr-x   0 sium       (501) staff       (20)     1703 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R
-drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-04 10:07:25.000411 cellsnake-0.2.0.dev7/cellsnake.egg-info/
--rw-r--r--   0 sium       (501) staff       (20)     4907 2023-04-04 10:07:24.000000 cellsnake-0.2.0.dev7/cellsnake.egg-info/PKG-INFO
--rw-r--r--   0 sium       (501) staff       (20)     2969 2023-04-04 10:07:24.000000 cellsnake-0.2.0.dev7/cellsnake.egg-info/SOURCES.txt
--rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-04 10:07:24.000000 cellsnake-0.2.0.dev7/cellsnake.egg-info/dependency_links.txt
--rw-r--r--   0 sium       (501) staff       (20)       58 2023-04-04 10:07:24.000000 cellsnake-0.2.0.dev7/cellsnake.egg-info/entry_points.txt
--rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-04 10:07:24.000000 cellsnake-0.2.0.dev7/cellsnake.egg-info/not-zip-safe
--rw-r--r--   0 sium       (501) staff       (20)      159 2023-04-04 10:07:24.000000 cellsnake-0.2.0.dev7/cellsnake.egg-info/requires.txt
--rw-r--r--   0 sium       (501) staff       (20)       10 2023-04-04 10:07:24.000000 cellsnake-0.2.0.dev7/cellsnake.egg-info/top_level.txt
--rw-r--r--   0 sium       (501) staff       (20)      152 2023-03-28 08:51:31.000000 cellsnake-0.2.0.dev7/reqs.txt
--rw-r--r--   0 sium       (501) staff       (20)      159 2023-03-28 12:37:22.000000 cellsnake-0.2.0.dev7/requirements.txt
--rw-r--r--   0 sium       (501) staff       (20)       38 2023-04-04 10:07:25.028592 cellsnake-0.2.0.dev7/setup.cfg
--rw-r--r--   0 sium       (501) staff       (20)     1674 2023-04-04 08:32:32.000000 cellsnake-0.2.0.dev7/setup.py
--rw-r--r--   0 sium       (501) staff       (20)   953080 2023-02-27 13:02:47.000000 cellsnake-0.2.0.dev7/test_counts.txt
--rw-r--r--   0 sium       (501) staff       (20)      340 2023-02-27 13:02:48.000000 cellsnake-0.2.0.dev7/test_meta.txt
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.573568 cellsnake-0.2.0.dev8/
+-rw-r--r--   0 sium       (501) staff       (20)     1072 2022-12-02 21:30:51.000000 cellsnake-0.2.0.dev8/LICENSE
+-rw-r--r--   0 sium       (501) staff       (20)      300 2023-02-22 13:59:41.000000 cellsnake-0.2.0.dev8/MANIFEST.in
+-rw-r--r--   0 sium       (501) staff       (20)     4906 2023-04-09 00:36:01.573360 cellsnake-0.2.0.dev8/PKG-INFO
+-rw-r--r--   0 sium       (501) staff       (20)     4458 2023-04-04 13:27:36.000000 cellsnake-0.2.0.dev8/README.md
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.562278 cellsnake-0.2.0.dev8/cellsnake/
+-rw-r--r--   0 sium       (501) staff       (20)        0 2022-12-02 21:33:29.000000 cellsnake-0.2.0.dev8/cellsnake/__init__.py
+-rw-r--r--   0 sium       (501) staff       (20)        0 2023-02-01 12:33:26.000000 cellsnake-0.2.0.dev8/cellsnake/cellsnake_functions.py
+-rwxr-xr-x   0 sium       (501) staff       (20)    13703 2023-04-07 13:12:53.000000 cellsnake-0.2.0.dev8/cellsnake/command_line.py
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.563704 cellsnake-0.2.0.dev8/cellsnake/scrna/
+-rw-r--r--   0 sium       (501) staff       (20)     2362 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/config.yaml
+-rwxr-xr-x   0 sium       (501) staff       (20)       55 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/install_r_packages.sh
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.563866 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/
+-rw-r--r--   0 sium       (501) staff       (20)    23558 2023-04-09 00:07:09.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/Snakefile
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.564062 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/bundle/
+-rw-r--r--   0 sium       (501) staff       (20)  2786711 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.559868 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.566297 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.566459 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/
+-rw-r--r--   0 sium       (501) staff       (20)     8522 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4148 2023-03-06 17:19:41.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     8607 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/k2sc.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4158 2023-03-29 12:07:58.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.567688 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/
+-rw-r--r--   0 sium       (501) staff       (20)     2179 2023-02-08 21:49:02.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/extra_functions.smk
+-rw-r--r--   0 sium       (501) staff       (20)      351 2023-04-04 08:31:54.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/integration.smk
+-rw-r--r--   0 sium       (501) staff       (20)     5712 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/microbiome.smk
+-rw-r--r--   0 sium       (501) staff       (20)     1050 2022-12-02 22:51:49.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/params_detect.smk
+-rw-r--r--   0 sium       (501) staff       (20)      181 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/params_write.smk
+-rw-r--r--   0 sium       (501) staff       (20)    20702 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/seurat.smk
+-rw-r--r--   0 sium       (501) staff       (20)      306 2023-04-09 00:07:09.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/subset.smk
+-rw-r--r--   0 sium       (501) staff       (20)     1337 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/test.smk
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.573109 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/
+-rwxr-xr-x   0 sium       (501) staff       (20)     3016 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-cellchat.R
+-rwxr-xr-x   0 sium       (501) staff       (20)    17388 2023-02-27 13:17:03.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3319 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-celltypist.R
+-rwxr-xr-x   0 sium       (501) staff       (20)      761 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-celltypist.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     4459 2023-02-28 14:02:58.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1132 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1241 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3449 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-dimplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1828 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-dotplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1714 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-find-markers.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3563 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     6918 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-functions.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3205 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2212 2023-02-20 22:44:59.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-gsea.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2945 2022-12-03 20:20:58.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-harmony.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2648 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-install-packages.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4595 2023-03-26 14:44:30.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kegg.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4464 2023-01-31 11:27:53.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py
+-rwxr-xr-x   0 sium       (501) staff       (20)     2937 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1952 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3289 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1253 2023-03-29 11:39:17.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2461 2023-03-10 09:17:10.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-metrics.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2835 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3375 2023-03-20 10:56:03.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2497 2023-04-03 19:18:34.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-monocle3.R
+-rwxr-xr-x   0 sium       (501) staff       (20)        0 2022-12-02 21:44:56.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-music-decon.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     6679 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     6898 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-read-qc.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     4568 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2068 2023-04-04 09:59:25.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     2636 2023-03-22 10:39:26.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     3548 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1363 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-technicals.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1703 2023-03-28 12:21:47.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R
+-rwxr-xr-x   0 sium       (501) staff       (20)     1217 2023-04-07 13:09:40.000000 cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-volcano.R
+drwxr-xr-x   0 sium       (501) staff       (20)        0 2023-04-09 00:36:01.563337 cellsnake-0.2.0.dev8/cellsnake.egg-info/
+-rw-r--r--   0 sium       (501) staff       (20)     4906 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/PKG-INFO
+-rw-r--r--   0 sium       (501) staff       (20)     3123 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 sium       (501) staff       (20)       58 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/entry_points.txt
+-rw-r--r--   0 sium       (501) staff       (20)        1 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/not-zip-safe
+-rw-r--r--   0 sium       (501) staff       (20)      159 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/requires.txt
+-rw-r--r--   0 sium       (501) staff       (20)       10 2023-04-09 00:36:01.000000 cellsnake-0.2.0.dev8/cellsnake.egg-info/top_level.txt
+-rw-r--r--   0 sium       (501) staff       (20)      152 2023-03-28 08:51:31.000000 cellsnake-0.2.0.dev8/reqs.txt
+-rw-r--r--   0 sium       (501) staff       (20)      159 2023-03-28 12:37:22.000000 cellsnake-0.2.0.dev8/requirements.txt
+-rw-r--r--   0 sium       (501) staff       (20)       38 2023-04-09 00:36:01.573615 cellsnake-0.2.0.dev8/setup.cfg
+-rw-r--r--   0 sium       (501) staff       (20)     1674 2023-04-07 13:10:17.000000 cellsnake-0.2.0.dev8/setup.py
+-rw-r--r--   0 sium       (501) staff       (20)   953080 2023-02-27 13:02:47.000000 cellsnake-0.2.0.dev8/test_counts.txt
+-rw-r--r--   0 sium       (501) staff       (20)      340 2023-02-27 13:02:48.000000 cellsnake-0.2.0.dev8/test_meta.txt
```

### Comparing `cellsnake-0.2.0.dev7/LICENSE` & `cellsnake-0.2.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/PKG-INFO` & `cellsnake-0.2.0.dev8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: cellsnake
-Version: 0.2.0.dev7
+Version: 0.2.0.dev8
 Summary: cellsnake
 Home-page: https://github.com/sinanugur/cellsnake
 Author: Sinan U. Umu
 Author-email: sinanugur@gmail.com
 Keywords: scRNA single-cell RNA analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cellsnake
 
-A command line tool for easy and scalable single cell analysis
-
-<img src="cellsnake-logo.png" width="80" height="80">
+A command line tool for easy and scalable single cell analysis  
+![Docker Pulls](https://img.shields.io/docker/pulls/sinanugur/cellsnake)
 
 Installation
 ------------
 
 Method for installing directly from the GitHub repo:
 ```
 git clone https://github.com/sinanugur/cellsnake.git
@@ -83,15 +82,14 @@
 Usage:
     cellsnake <INPUT> [--resolution <text>] [--percent_mt <text>] [--configfile <text>] [--gene <text>] [--jobs <integer>] [--option <text>]... [--release-the-kraken <text>] [--taxa <text>] [--unlock|--remove] [--dry]
     cellsnake <INPUT> [--unlock|--remove] [--dry]
     cellsnake --generate-template
     cellsnake --install-packages
     cellsnake (-h | --help)
     cellsnake --version
-    cellsnake --init
 
 Arguments:
     INPUT                                   Input directory or a file to process (if a directory given, batch mode is ON).
     -c <text>, --configfile <text>          Config file name (if not supplied, it will use default settings, you may generate a template, change it and use it in your runs).
     --resolution <text>                     Resolution for cluster detection, write "auto" for auto detection [default: 0.8].
     --percent_mt <text>                     Maximum mitochondrial gene percentage cutoff, for example, 5 or 10, write "auto" for auto detection [default: 10].
     --gene <text>                           Create publication ready plots for a gene or a list of genes from a text file.
```

### Comparing `cellsnake-0.2.0.dev7/README.md` & `cellsnake-0.2.0.dev8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # cellsnake
 
-A command line tool for easy and scalable single cell analysis
-
-<img src="cellsnake-logo.png" width="80" height="80">
+A command line tool for easy and scalable single cell analysis  
+![Docker Pulls](https://img.shields.io/docker/pulls/sinanugur/cellsnake)
 
 Installation
 ------------
 
 Method for installing directly from the GitHub repo:
 ```
 git clone https://github.com/sinanugur/cellsnake.git
@@ -69,15 +68,14 @@
 Usage:
     cellsnake <INPUT> [--resolution <text>] [--percent_mt <text>] [--configfile <text>] [--gene <text>] [--jobs <integer>] [--option <text>]... [--release-the-kraken <text>] [--taxa <text>] [--unlock|--remove] [--dry]
     cellsnake <INPUT> [--unlock|--remove] [--dry]
     cellsnake --generate-template
     cellsnake --install-packages
     cellsnake (-h | --help)
     cellsnake --version
-    cellsnake --init
 
 Arguments:
     INPUT                                   Input directory or a file to process (if a directory given, batch mode is ON).
     -c <text>, --configfile <text>          Config file name (if not supplied, it will use default settings, you may generate a template, change it and use it in your runs).
     --resolution <text>                     Resolution for cluster detection, write "auto" for auto detection [default: 0.8].
     --percent_mt <text>                     Maximum mitochondrial gene percentage cutoff, for example, 5 or 10, write "auto" for auto detection [default: 10].
     --gene <text>                           Create publication ready plots for a gene or a list of genes from a text file.
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake/command_line.py` & `cellsnake-0.2.0.dev8/cellsnake/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 import cellsnake
 cellsnake_path=os.path.dirname(cellsnake.__file__)
 options = ["clustree","clusteringTree","minimal","standard","advanced"] #and integration
 
 
 __author__ = 'Sinan U. Umu'
-__version__= '0.2.0.dev7'
+__version__= '0.2.0.dev8'
 __logo__="""
              _  _                     _           
             | || |                   | |          
   ___   ___ | || | ___  _ __    __ _ | | __  ___  
  / __| / _ \| || |/ __|| '_ \  / _` || |/ / / _ \ 
 | (__ |  __/| || |\__ \| | | || (_| ||   < |  __/ 
  \___| \___||_||_||___/|_| |_| \__,_||_|\_\ \___|
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/config.yaml` & `cellsnake-0.2.0.dev8/cellsnake/scrna/config.yaml`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/Snakefile` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/Snakefile`

 * *Files 4% similar despite different names*

```diff
@@ -28,32 +28,44 @@
 is_integrated_sample=config.get("is_integrated_sample",False)
 gene_to_plot=[] if config.get("gene_to_plot",None) is None else [config.get("gene_to_plot")]
 
 
 #configfile: "config.yaml"
 
 files=[]
+def file_capture(datafolder):
+    cellranger_new = cellsnake_glob_wildcards(datafolder +  "/{sample}/raw_feature_bc_matrix/matrix.mtx.gz").sample + cellsnake_glob_wildcards(datafolder + "/{sample}/outs/filtered_feature_bc_matrix/matrix.mtx.gz").sample + cellsnake_glob_wildcards(datafolder +  "/{sample}/matrix.mtx.gz").sample
+    cellranger_old = cellsnake_glob_wildcards(datafolder +  "/{sample}/raw_feature_bc_matrix/matrix.mtx").sample + cellsnake_glob_wildcards(datafolder + "/{sample}/outs/filtered_feature_bc_matrix/matrix.mtx").sample + cellsnake_glob_wildcards(datafolder +  "/{sample}/matrix.mtx").sample
+    h5files = cellsnake_glob_wildcards(datafolder + "/{sample}/filtered_feature_bc_matrix.h5").sample 
+    files=list(filter(lambda i: "/" not in i, cellranger_new + cellranger_old + h5files)) #do not capture subdirectories etc
+    return files
+
 try:
 
     if os.path.isdir(datafolder):
-        cellranger_new = cellsnake_glob_wildcards(datafolder +  "/{sample}/raw_feature_bc_matrix/matrix.mtx.gz").sample + cellsnake_glob_wildcards(datafolder + "/{sample}/outs/filtered_feature_bc_matrix/matrix.mtx.gz").sample + cellsnake_glob_wildcards(datafolder +  "/{sample}/matrix.mtx.gz").sample
-        cellranger_old = cellsnake_glob_wildcards(datafolder +  "/{sample}/raw_feature_bc_matrix/matrix.mtx").sample + cellsnake_glob_wildcards(datafolder + "/{sample}/outs/filtered_feature_bc_matrix/matrix.mtx").sample + cellsnake_glob_wildcards(datafolder +  "/{sample}/matrix.mtx").sample
-        h5files, = cellsnake_glob_wildcards(datafolder + "/{sample}/filtered_feature_bc_matrix.h5")
-        files=list(filter(lambda i: "/" not in i, cellranger_new + cellranger_old + h5files)) #do not capture subdirectories etc
+        files=file_capture(datafolder)
+        
+        if len(files)==0:
+            head,tail = os.path.split(datafolder.strip("/"))
+            files=file_capture(head) #probably capture a single file here
+            files=[x for x in files if tail in x]
+            if files:
+                datafolder=head
         print(files)
-    
     if os.path.isfile(datafolder):
         file_extension = pathlib.Path(datafolder)
         if (file_extension.suffix).lower() not in [".rds"]:
             files = [file_extension.stem]
             print(files)
         elif is_integrated_sample:
             analyses_folder="analyses_integrated"
             results_folder="results_integrated"
             files = [file_extension.stem]
+        elif (file_extension.suffix).lower() in [".rds"] and option in ["subset"]:
+            files = datafolder
 
 except:
     print("No samples detected")
 
 
 
 #basic paramaters
@@ -64,14 +76,19 @@
 min_molecules=config.get("min_molecules",0) #nCount_RNA
 percent_mt=str(config.get("percent_mt",10)) #if not automatic, this will be used for all samples
 percent_rp=config.get("percent_rp",0) #by default, no filtering on ribosomal genes percentage 
 highly_variable_features=config.get("highly_variable_features",2000)
 variable_selection_method=config.get("variable_selection_method","vst")
 doublet_filter= "--doublet.filter" if config.get("doublet_filter",True) in [True,"TRUE","True","T"] and is_integrated_sample is False else ""
 metadata_file=config.get("metadata_file","metadata.csv")
+metadata_column=config.get("metadata_column","condition")
+keywords=config.get("keywords",1)
+exact="--exact" if config.get("exact",True) in [True,"TRUE","True","T"] else ""
+subset_file=config.get("subset_file","subset")
+subset_column=config.get("subset_column","seurat_clusters")
 
 min_percentage_to_plot=config.get("min_percentage_to_plot",5) #only plot clusters with more than 5% of cells
 
 #automatic mt filtering
 grid_search=config.get("grid_search",False) #requires params file in tsv format
 
 
@@ -215,14 +232,21 @@
         outs += expand([results_folder + "/" + s + "/{params}/enrichment_analysis/table_GO-geneset_enrichment-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/enrichment_analysis/table_KEGG-enrichment-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/enrichment_analysis/table_KEGG-geneset_enrichment-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/enrichment_analysis/table_KEGG-module_enrichment-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/enrichment_analysis/table_KEGG-module_geneset_enrichment-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
     return outs
 
+def metadata_pairwise_deseq_analysis(paramspace,metadata_column):
+    outs=[]
+    if os.path.isfile(metadata_file) and is_integrated_sample:
+        outs += expand([results_folder + "/" + s + "/{params}/metaplot_volcano-" + metadata_column + ".pdf" for s in files],params=list(paramspace.instance_patterns))
+        outs += expand([results_folder + "/" + s + "/{params}/metatable_positive-markers-" + metadata_column + ".xlsx" for s in files],params=list(paramspace.instance_patterns))
+    return outs
+
 
 
 def kraken_predictions(paramspace,taxa,identity):
     #bamfiles=cellsnake_glob_wildcards(datafolder + "/{sample}/outs/possorted_genome_bam.bam").sample + cellsnake_glob_wildcards(datafolder + "/{sample}/possorted_genome_bam.bam").sample 
     outs=[]
     if kraken_db_folder is not None:
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/plot_microbiome_full-" + taxa + "-level.pdf" for s in files],params=list(paramspace.instance_patterns))
@@ -230,14 +254,15 @@
         outs = outs + ["analyses_integrated/seurat/" + integration_id + "-" + taxa + ".rds"]
     elif is_integrated_sample is True and os.path.isfile("analyses_integrated/seurat/" + integration_id + "-" + taxa + ".rds"):
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/plot_integrated_microbiome_dimplot-" + taxa + "-" + x + ".pdf" for x in ["umap","tsne"] for s in files],params=list(paramspace.instance_patterns))
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/plot_integrated_significance-" + taxa + "-" + x + ".pdf" for x in identity for s in files],params=list(paramspace.instance_patterns))
         outs = outs + expand([results_folder + "/" + s + "/{params}/microbiome/table_integrated_significance-" + taxa + "-" + x + ".xlsx" for x in identity for s in files],params=list(paramspace.instance_patterns))
     return outs
 
+
 def write_main_log(files):
 
     pathlib.Path("logs/").mkdir(parents=True, exist_ok=True)
     with open("logs/" + logname,"w") as f:
         f.write("Total number of samples processed : " + str(len(files)) + "\n")
         f.write("Sample names in this run : " + " ".join(files) + "\n")
         f.write("Run ID : " + str(runid) + "\n")
@@ -310,15 +335,16 @@
                 expand([results_folder + "/" + s + "/{params}/trajectory/plot_monocle-partition-plot.pdf" for s in files],params=list(paramspace.instance_patterns))
                 ]
     if option in ["minimal","standard","advanced"]:
         outs = outs + [
                 identity_dependent_dimplot(paramspace,identity_to_analysis),
                 identity_dependent_metrics(paramspace,[x for x in identity_to_analysis if x != "orig.ident"]),
                 kraken_predictions(paramspace,taxa,identity_to_analysis),
-                selected_gene_plot(paramspace,gene_to_plot,identity_to_analysis)
+                selected_gene_plot(paramspace,gene_to_plot,identity_to_analysis),
+                metadata_pairwise_deseq_analysis(paramspace,metadata_column)
                 ]
     if option in ["clustree","clusteringTree","minimal","standard","advanced"]:
         outs += expand([results_folder + "/" + s + "/{params}/technicals/plot_clustree.pdf" for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/technicals/plot_nFeature.pdf" for s in files],params=list(paramspace.instance_patterns))
         outs += expand([results_folder + "/" + s + "/{params}/technicals/plot_nCount.pdf" for s in files],params=list(paramspace.instance_patterns))
     if option in ["advanced"]:
         outs += cellchat_plot(paramspace,[x for x in identity_to_analysis if x != "orig.ident"])
@@ -368,10 +394,17 @@
 elif option in ["minimal","standard","clustree","clusteringTree","advanced"] and files:
     include: "rules/seurat.smk"
     include: "rules/microbiome.smk"
     rule all:
         input:
             sample_parameter(paramspace,files)
 
+elif option in ["subset"] and files:
+    include: "rules/subset.smk"
+    rule all:
+        input:
+            "dataoutput/" + subset_file + ".rds"
+
+
 else:
     print("Please select a correct option or no files detected...")
     pass
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/bundle/c2.cgp.v2022.1.Hs.symbols.gmt`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/collapse_taxonomy.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/k2sc.py` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/k2sc.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/mg2sc/src/scMeG-kraken.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/extra_functions.smk` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/extra_functions.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/microbiome.smk` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/microbiome.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/params_detect.smk` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/params_detect.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/seurat.smk` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/seurat.smk`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,43 @@
         rds=analyses_folder + "/go/" + f"{paramspace.wildcard_pattern}" + "/{sample}-{i}-go.rds",
         go=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/enrichment_analysis/table_GO-enrichment-{i}.xlsx",
         gse=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/enrichment_analysis/table_GO-geneset_enrichment-{i}.xlsx"
     shell:
         "{cellsnake_path}workflow/scripts/scrna-go_analysis.R --xlsx {input} --output.rds {output.rds} --mapping {mapping} --output.go {output.go} --output.gse {output.gse}"
 
 
+rule deseq_analysis_from_metadata_file:
+    input:
+        rds=analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds",
+        metadata=metadata_file
+    output:
+        rds=analyses_folder + "/markers/" + f"{paramspace.wildcard_pattern}" + "/deseq_{sample}-{i}.rds"
+    shell:
+        "{cellsnake_path}workflow/scripts/scrna-find-pairwise-markers.R --rds {input.rds} --logfc.threshold {logfc_threshold} --test.use {test_use} --output.rds {output.rds} --metadata {input.metadata} --metadata.column {wildcards.i}"
+
+rule create_deseq_metadata_tables:
+    input:
+        analyses_folder + "/markers/" + f"{paramspace.wildcard_pattern}" + "/deseq_{sample}-{i}.rds"
+    output:
+        positive=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}"  + "/metatable_positive-markers-{i}.xlsx",
+        allmarkers=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}"  +  "/metatable_all-markers-{i}.xlsx"
+    params:
+        paramaters=paramspace.instance,
+    shell:
+        "{cellsnake_path}workflow/scripts/scrna-marker-tables.R --rds {input} --output.xlsx.positive {output.positive} --output.xlsx.all {output.allmarkers}"
+
+rule volcano_plots:
+    input:
+        rds=analyses_folder + "/markers/" + f"{paramspace.wildcard_pattern}" + "/deseq_{sample}-{i}.rds"
+    output:
+        pdf=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}"  +  "/metaplot_volcano-{i}.pdf"
+    shell:
+        "{cellsnake_path}workflow/scripts/scrna-volcano.R --rds {input.rds} --vplot {output.pdf}"
+
+
 
 rule gsea_cerebro:
     input:
         rds=analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds",
         #csv=lambda wildcards: analyses_folder + "/celltypist/" + celltypist_model + "/" + f"{paramspace.wildcard_pattern}" + "/{sample}/predicted_labels.csv" if wildcards.i == "majority_voting" else [],
         gseafile=gsea_file
     output:
@@ -308,14 +337,7 @@
     output:
         pplot=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/trajectory/plot_monocle-partition-plot.pdf"
     params:
         outputdir=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/trajectory/"
     shell:
         "{cellsnake_path}workflow/scripts/scrna-monocle3.R --rds {input.rds} --output.dir {params.outputdir} --pplot {output.pplot}"
 
-rule subset_final_rds:
-    input:
-        rds=analyses_folder + "/processed/" + f"{paramspace.wildcard_pattern}" + "/{sample}.rds"
-    output:
-        output=results_folder + "/{sample}/" + f"{paramspace.wildcard_pattern}" + "/dataoutput/{keyword}.rds"
-    shell:
-        "{cellsnake_path}workflow/scripts/scrna-subset_final_rds.R --rds {input.rds} --output {output.rds}"
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/rules/test.smk` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/rules/test.smk`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-cellchat.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-cellchat.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-celltypist.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-celltypist.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-celltypist.py` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-celltypist.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-dimplot.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-dimplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-dotplot.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-dotplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-find-markers.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-find-markers.R`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   ),
   optparse::make_option(c("--test.use"),
     type = "character", default = "wilcox",
     help = "Test use [default= %default]", metavar = "character"
   ),
   optparse::make_option(c("--output.rds"),
     type = "character", default = NULL,
-    help = "Excel table of all markers", metavar = "character"
+    help = "RDS table of all markers", metavar = "character"
   ),
   optparse::make_option(c("--idents"),
     type = "character", default = "seurat_clusters",
     help = "Meta data column name for marker analysis", metavar = "character"
   )
 )
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-functions.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-functions.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-go_analysis.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-gsea.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-gsea.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-harmony.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-harmony.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-install-packages.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-install-packages.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-kegg.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kegg.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-kraken2-data-parser.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-heatmap.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-marker-tables.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-metrics.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-metrics.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-microbiome-dimplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-microbiome-sigplot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-monocle3.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-monocle3.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,17 @@
 scrna <- RunPCA(scrna, features = not.all.genes)
 dimensionReduction <- function_pca_dimensions(scrna)
 scrna <- FindNeighbors(scrna, dims = 1:dimensionReduction)
 
 if (!opt$resolution %in% c("auto", "AUTO", "Auto")) {
   scrna <- FindClusters(scrna, resolution = as.numeric(opt$resolution))
 } else {
+  if (!requireNamespace("MultiKParallel", quietly = TRUE)) {
+    remotes::install_github("sinanugur/MultiKParallel")
+  }
   require(MultiKParallel)
   scrna_tmp <- FindClusters(scrna, resolution = seq(0.2, 2.5, 0.15))
   multik <- MultiKParallel(scrna_tmp, reps = 10, seed = 255, resolution = seq(0.2, 2.5, 0.15), numCores = opt$cpu, nPC = dimensionReduction)
   multik$k %>%
     tibble::as_tibble() %>%
     count(value) %>%
     filter(n == max(n)) %>%
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-read-qc.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-read-qc.R`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,21 @@
       }
       return(scrna.data)
     },
     silent = TRUE
   )
 }
 
+
+
 function_read_input(opt) -> scrna.data
 
 
+
+
 scrna <- CreateSeuratObject(counts = scrna.data, project = make.names(opt$sampleid), min.cells = opt$min.cells, min.features = opt$min.features)
 rm(scrna.data)
 
 
 scrna <- RenameCells(object = scrna, add.cell.id = make.names(opt$sampleid)) # add cell.id to cell name
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-singler-plots.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 #!/usr/bin/env Rscript
 
-
 option_list <- list(
-    optparse::make_option(c("--rds"),
-        type = "character", default = NULL,
-        help = "Processed rds file of a Seurat object", metavar = "character"
-    ),
-    optparse::make_option(c("--keywords"),
-        type = "character", default = NULL,
-        help = "Keywords to slice object", metavar = "character"
-    ),
-    optparse::make_option(c("--idents"),
-        type = "character", default = NULL,
-        help = "Meta data column name for selecting the slice", metavar = "character"
-    ),
-    optparse::make_option(c("--output.rds"),
-        type = "character", default = "output.rds",
-        help = "Output RDS file name [default= %default]", metavar = "character"
-    )
+  optparse::make_option(c("--rds"),
+    type = "character", default = NULL,
+    help = "A list of RDS files of Seurat objects", metavar = "character"
+  ),
+  optparse::make_option(c("--output"),
+    type = "character", default = "output.h5ad",
+    help = "Output h5ad file name", metavar = "character"
+  )
 )
 
-
-
 opt_parser <- optparse::OptionParser(option_list = option_list)
 opt <- optparse::parse_args(opt_parser)
 
 if (is.null(opt$rds)) {
-    optparse::print_help(opt_parser)
-    stop("At least one argument must be supplied (rds file)", call. = FALSE)
+  optparse::print_help(opt_parser)
+  stop("At least one argument must be supplied (rds file and sampleid)", call. = FALSE)
 }
 
-
+if (!requireNamespace("SeuratDisk", quietly = TRUE)) {
+  remotes::install_github("mojaveazure/seurat-disk")
+}
 require(Seurat)
+require(SeuratDisk)
 require(tidyverse)
 
 
-
 scrna <- readRDS(file = opt$rds)
 
+UpdateSeuratObject(scrna) -> scrna
+DefaultAssay(scrna) <- "RNA"
+
+DietSeurat(scrna) -> scrna
+
+scrna@meta.data %>% dplyr::mutate(dplyr::across(where(is.factor), as.character)) -> scrna@meta.data
+
+
+output_file_name <- str_remove_all(opt$output, ".h5ad$")
 
-if (!is.null(opt$keywords)) {
-    keywords <- strsplit(opt$keywords, ",")[[1]]
-    patterns <- paste0("(?i)", "(", paste(keywords, collapse = "|"), ")")
-    scrna@meta.data %>% dplyr::filter(if_any(everything(), str_detect, pattern = patterns))
-}
+SaveH5Seurat(scrna, filename = paste0(output_file_name, ".h5Seurat"), overwrite = TRUE)
+SeuratDisk::Convert(paste0(output_file_name, ".h5Seurat"), dest = "h5ad", overwrite = TRUE)
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-technicals.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-technicals.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R` & `cellsnake-0.2.0.dev8/cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R`

 * *Files identical despite different names*

### Comparing `cellsnake-0.2.0.dev7/cellsnake.egg-info/PKG-INFO` & `cellsnake-0.2.0.dev8/cellsnake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: cellsnake
-Version: 0.2.0.dev7
+Version: 0.2.0.dev8
 Summary: cellsnake
 Home-page: https://github.com/sinanugur/cellsnake
 Author: Sinan U. Umu
 Author-email: sinanugur@gmail.com
 Keywords: scRNA single-cell RNA analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cellsnake
 
-A command line tool for easy and scalable single cell analysis
-
-<img src="cellsnake-logo.png" width="80" height="80">
+A command line tool for easy and scalable single cell analysis  
+![Docker Pulls](https://img.shields.io/docker/pulls/sinanugur/cellsnake)
 
 Installation
 ------------
 
 Method for installing directly from the GitHub repo:
 ```
 git clone https://github.com/sinanugur/cellsnake.git
@@ -83,15 +82,14 @@
 Usage:
     cellsnake <INPUT> [--resolution <text>] [--percent_mt <text>] [--configfile <text>] [--gene <text>] [--jobs <integer>] [--option <text>]... [--release-the-kraken <text>] [--taxa <text>] [--unlock|--remove] [--dry]
     cellsnake <INPUT> [--unlock|--remove] [--dry]
     cellsnake --generate-template
     cellsnake --install-packages
     cellsnake (-h | --help)
     cellsnake --version
-    cellsnake --init
 
 Arguments:
     INPUT                                   Input directory or a file to process (if a directory given, batch mode is ON).
     -c <text>, --configfile <text>          Config file name (if not supplied, it will use default settings, you may generate a template, change it and use it in your runs).
     --resolution <text>                     Resolution for cluster detection, write "auto" for auto detection [default: 0.8].
     --percent_mt <text>                     Maximum mitochondrial gene percentage cutoff, for example, 5 or 10, write "auto" for auto detection [default: 10].
     --gene <text>                           Create publication ready plots for a gene or a list of genes from a text file.
```

### Comparing `cellsnake-0.2.0.dev7/cellsnake.egg-info/SOURCES.txt` & `cellsnake-0.2.0.dev8/cellsnake.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,27 @@
 cellsnake/scrna/workflow/mg2sc/src/.ipynb_checkpoints/k2sc-checkpoint.py
 cellsnake/scrna/workflow/rules/extra_functions.smk
 cellsnake/scrna/workflow/rules/integration.smk
 cellsnake/scrna/workflow/rules/microbiome.smk
 cellsnake/scrna/workflow/rules/params_detect.smk
 cellsnake/scrna/workflow/rules/params_write.smk
 cellsnake/scrna/workflow/rules/seurat.smk
+cellsnake/scrna/workflow/rules/subset.smk
 cellsnake/scrna/workflow/rules/test.smk
 cellsnake/scrna/workflow/scripts/scrna-cellchat.R
 cellsnake/scrna/workflow/scripts/scrna-cellchat_plots.R
 cellsnake/scrna/workflow/scripts/scrna-celltypist.R
 cellsnake/scrna/workflow/scripts/scrna-celltypist.py
 cellsnake/scrna/workflow/scripts/scrna-clusteringtree.R
 cellsnake/scrna/workflow/scripts/scrna-combine-microbiome-rds.R
 cellsnake/scrna/workflow/scripts/scrna-convert-to-h5ad.R
 cellsnake/scrna/workflow/scripts/scrna-dimplot.R
 cellsnake/scrna/workflow/scripts/scrna-dotplot.R
 cellsnake/scrna/workflow/scripts/scrna-find-markers.R
+cellsnake/scrna/workflow/scripts/scrna-find-pairwise-markers.R
 cellsnake/scrna/workflow/scripts/scrna-functions.R
 cellsnake/scrna/workflow/scripts/scrna-go_analysis.R
 cellsnake/scrna/workflow/scripts/scrna-gsea.R
 cellsnake/scrna/workflow/scripts/scrna-harmony.R
 cellsnake/scrna/workflow/scripts/scrna-install-packages.R
 cellsnake/scrna/workflow/scripts/scrna-kegg.R
 cellsnake/scrna/workflow/scripts/scrna-kraken2-collapse.py
@@ -60,8 +62,9 @@
 cellsnake/scrna/workflow/scripts/scrna-normalization-pca.R
 cellsnake/scrna/workflow/scripts/scrna-read-qc.R
 cellsnake/scrna/workflow/scripts/scrna-selected-marker-plots.R
 cellsnake/scrna/workflow/scripts/scrna-seurat-integration.R
 cellsnake/scrna/workflow/scripts/scrna-singler-plots.R
 cellsnake/scrna/workflow/scripts/scrna-subset_final_rds.R
 cellsnake/scrna/workflow/scripts/scrna-technicals.R
-cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R
+cellsnake/scrna/workflow/scripts/scrna-top-marker-plot.R
+cellsnake/scrna/workflow/scripts/scrna-volcano.R
```

### Comparing `cellsnake-0.2.0.dev7/setup.py` & `cellsnake-0.2.0.dev8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 with open("README.md","r") as readme:
     long_description=readme.read()
 
 setup(
     name="cellsnake",
-    version="0.2.0.dev7",
+    version="0.2.0.dev8",
     packages=find_packages(exclude=('tests*','testing*')),
     long_description=long_description,
     long_description_content_type="text/markdown",
     #extras_require={"dev":["pytest>=3.7"]},
     install_requires=requirements,
     include_package_data=True,
     zip_safe=False,
```

### Comparing `cellsnake-0.2.0.dev7/test_counts.txt` & `cellsnake-0.2.0.dev8/test_counts.txt`

 * *Files identical despite different names*

