# Comparing `tmp/solvation-analysis-0.3.2.tar.gz` & `tmp/solvation-analysis-0.3.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solvation-analysis-0.3.2.tar", last modified: Thu Apr  6 16:21:02 2023, max compression
+gzip compressed data, was "solvation-analysis-0.3.3a0.tar", last modified: Sun Apr  9 17:47:02 2023, max compression
```

## Comparing `solvation-analysis-0.3.2.tar` & `solvation-analysis-0.3.3a0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.812451 solvation-analysis-0.3.2/
--rw-r--r--   0 orioncohen   (505) staff       (20)     8081 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 orioncohen   (505) staff       (20)    34684 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/LICENSE
--rw-r--r--   0 orioncohen   (505) staff       (20)      234 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/MANIFEST.in
--rw-r--r--   0 orioncohen   (505) staff       (20)    44782 2023-04-06 16:21:02.399305 solvation-analysis-0.3.2/PKG-INFO
--rw-r--r--   0 orioncohen   (505) staff       (20)     3879 2023-04-02 16:17:13.000000 solvation-analysis-0.3.2/README.md
--rw-r--r--   0 orioncohen   (505) staff       (20)     1940 2023-04-02 16:08:07.000000 solvation-analysis-0.3.2/pyproject.toml
--rw-r--r--   0 orioncohen   (505) staff       (20)      106 2023-04-02 16:08:07.000000 solvation-analysis-0.3.2/requirements.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)      381 2023-04-06 16:21:02.399748 solvation-analysis-0.3.2/setup.cfg
--rw-r--r--   0 orioncohen   (505) staff       (20)     2400 2023-04-05 15:18:21.000000 solvation-analysis-0.3.2/setup.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:21:02.400015 solvation-analysis-0.3.2/solvation_analysis/
--rw-r--r--   0 orioncohen   (505) staff       (20)      335 2022-10-28 18:42:42.000000 solvation-analysis-0.3.2/solvation_analysis/__init__.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      728 2022-10-28 18:42:42.000000 solvation-analysis-0.3.2/solvation_analysis/_column_names.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     8016 2022-10-28 18:42:42.000000 solvation-analysis-0.3.2/solvation_analysis/_utils.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      498 2023-04-06 16:21:02.400143 solvation-analysis-0.3.2/solvation_analysis/_version.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     6593 2023-04-06 16:18:52.000000 solvation-analysis-0.3.2/solvation_analysis/coordination.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    10777 2023-04-02 16:08:07.000000 solvation-analysis-0.3.2/solvation_analysis/networking.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     5709 2023-04-02 16:08:07.000000 solvation-analysis-0.3.2/solvation_analysis/pairing.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    13759 2023-04-06 16:18:52.000000 solvation-analysis-0.3.2/solvation_analysis/plotting.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    11231 2022-10-28 18:42:42.000000 solvation-analysis-0.3.2/solvation_analysis/rdf_parser.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    10944 2023-04-02 16:08:07.000000 solvation-analysis-0.3.2/solvation_analysis/residence.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    38245 2023-02-14 18:50:22.000000 solvation-analysis-0.3.2/solvation_analysis/solute.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     8970 2023-04-06 16:18:52.000000 solvation-analysis-0.3.2/solvation_analysis/speciation.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.732936 solvation-analysis-0.3.2/solvation_analysis/tests/
--rw-r--r--   0 orioncohen   (505) staff       (20)      112 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/__init__.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     9536 2023-02-14 18:28:50.000000 solvation-analysis-0.3.2/solvation_analysis/tests/conftest.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.734030 solvation-analysis-0.3.2/solvation_analysis/tests/data/
--rw-r--r--   0 orioncohen   (505) staff       (20)     8196 2022-10-02 21:12:27.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/.DS_Store
--rw-r--r--   0 orioncohen   (505) staff       (20)     2848 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/README.md
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.743302 solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)  1418421 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_fec.data
--rw-r--r--   0 orioncohen   (505) staff       (20)    14285 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_fec_elements.csv
--rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)  5563748 2022-10-28 18:42:42.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.761334 solvation-analysis-0.3.2/solvation_analysis/tests/data/ea_fec_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)   892516 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   761309 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.709316 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.766206 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/ea/
--rw-r--r--   0 orioncohen   (505) staff       (20)   871090 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/ea/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1023556 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.769158 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/eaf/
--rw-r--r--   0 orioncohen   (505) staff       (20)   874261 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/eaf/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1027396 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.772043 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/fea/
--rw-r--r--   0 orioncohen   (505) staff       (20)   875050 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/fea/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1028356 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.774787 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/feaf/
--rw-r--r--   0 orioncohen   (505) staff       (20)   876623 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/feaf/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1030276 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.779974 solvation-analysis-0.3.2/solvation_analysis/tests/data/iba_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)   721156 2022-09-27 18:34:04.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   610100 2022-09-27 18:34:04.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.798669 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.805336 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:20:23.811963 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)     2601 2022-09-27 18:34:04.000000 solvation-analysis-0.3.2/solvation_analysis/tests/datafiles.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1672 2023-04-06 16:18:52.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_coordination.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      867 2023-02-14 18:28:50.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_networking.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1516 2023-04-02 16:08:07.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_pairing.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    10037 2023-04-06 16:18:52.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_plotting.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     6317 2022-10-28 18:42:42.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_rdf_parser.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      961 2023-02-14 18:28:50.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_residence.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     4012 2022-10-28 18:42:42.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_selection.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    12563 2023-04-02 16:08:07.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_solute.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1572 2023-04-06 16:18:52.000000 solvation-analysis-0.3.2/solvation_analysis/tests/test_speciation.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-06 16:21:02.396207 solvation-analysis-0.3.2/solvation_analysis.egg-info/
--rw-r--r--   0 orioncohen   (505) staff       (20)    44782 2023-04-06 16:21:02.000000 solvation-analysis-0.3.2/solvation_analysis.egg-info/PKG-INFO
--rw-r--r--   0 orioncohen   (505) staff       (20)     7068 2023-04-06 16:21:02.000000 solvation-analysis-0.3.2/solvation_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)        1 2023-04-06 16:21:02.000000 solvation-analysis-0.3.2/solvation_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)       96 2023-04-06 16:21:02.000000 solvation-analysis-0.3.2/solvation_analysis.egg-info/requires.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)       19 2023-04-06 16:21:02.000000 solvation-analysis-0.3.2/solvation_analysis.egg-info/top_level.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)    78254 2022-08-17 22:41:48.000000 solvation-analysis-0.3.2/versioneer.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.534578 solvation-analysis-0.3.3a0/
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8081 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 orioncohen   (505) staff       (20)    34684 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/LICENSE
+-rw-r--r--   0 orioncohen   (505) staff       (20)      234 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/MANIFEST.in
+-rw-r--r--   0 orioncohen   (505) staff       (20)    44784 2023-04-09 17:47:02.983612 solvation-analysis-0.3.3a0/PKG-INFO
+-rw-r--r--   0 orioncohen   (505) staff       (20)     3879 2023-04-02 16:17:13.000000 solvation-analysis-0.3.3a0/README.md
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1925 2023-04-09 17:20:57.000000 solvation-analysis-0.3.3a0/pyproject.toml
+-rw-r--r--   0 orioncohen   (505) staff       (20)      106 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/requirements.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)      381 2023-04-09 17:47:02.984218 solvation-analysis-0.3.3a0/setup.cfg
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2400 2023-04-05 15:18:21.000000 solvation-analysis-0.3.3a0/setup.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:47:02.984917 solvation-analysis-0.3.3a0/solvation_analysis/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      335 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/__init__.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      728 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/_column_names.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8016 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/_utils.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      504 2023-04-09 17:47:02.984993 solvation-analysis-0.3.3a0/solvation_analysis/_version.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     6570 2023-04-09 17:43:35.000000 solvation-analysis-0.3.3a0/solvation_analysis/coordination.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    10777 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/networking.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     5709 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/pairing.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    13759 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3a0/solvation_analysis/plotting.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    11231 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/rdf_parser.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    10944 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/residence.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    38245 2023-02-14 18:50:22.000000 solvation-analysis-0.3.3a0/solvation_analysis/solute.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8970 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3a0/solvation_analysis/speciation.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.472765 solvation-analysis-0.3.3a0/solvation_analysis/tests/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      112 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/__init__.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     9536 2023-02-14 18:28:50.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/conftest.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.474241 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8196 2022-10-02 21:12:27.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/.DS_Store
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2848 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/README.md
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.481722 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1418421 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec.data
+-rw-r--r--   0 orioncohen   (505) staff       (20)    14285 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_elements.csv
+-rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)  5563748 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.496293 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   892516 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   761309 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.450151 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.500539 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   871090 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1023556 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.503346 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   874261 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1027396 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.506236 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   875050 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1028356 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.509482 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   876623 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1030276 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.512342 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   721156 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   610100 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.525390 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.529744 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.534331 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2601 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/datafiles.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1596 2023-04-09 17:25:23.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_coordination.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      867 2023-02-14 18:28:50.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_networking.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1516 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_pairing.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    10037 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_plotting.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     6317 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_rdf_parser.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      961 2023-02-14 18:28:50.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_residence.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     4012 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_selection.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    12563 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_solute.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1572 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_speciation.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:47:02.980183 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/
+-rw-r--r--   0 orioncohen   (505) staff       (20)    44784 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 orioncohen   (505) staff       (20)     7068 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)        1 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)       88 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/requires.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)       19 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/top_level.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)    78254 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/versioneer.py
```

### Comparing `solvation-analysis-0.3.2/CODE_OF_CONDUCT.md` & `solvation-analysis-0.3.3a0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/LICENSE` & `solvation-analysis-0.3.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/PKG-INFO` & `solvation-analysis-0.3.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvation-analysis
-Version: 0.3.2
+Version: 0.3.3a0
 Summary: A toolkit to analyze solvation structure in molecular dynamics trajectories.
 Author: Orion Cohen
 Author-email: Orion Cohen <orioncohen@berkeley.edu>
 Maintainer-email: Orion Cohen <orioncohen@berkeley.edu>, Hugo MacDermott-Opeskin <hugomacdermott@gmail.com>
 License:                         GNU GENERAL PUBLIC LICENSE 
                                   Version 3, 29 June 2007
```

### Comparing `solvation-analysis-0.3.2/README.md` & `solvation-analysis-0.3.3a0/README.md`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/pyproject.toml` & `solvation-analysis-0.3.3a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 ]
 
 dependencies = [
     'numpy>=1.20.0',
     'pandas',
     'mdanalysis>=2.0.0',
     'pytest',
-    'pathlib',
     'matplotlib',
     'scipy',
     'statsmodels',
     'plotly',
     'rdkit'
 ]
```

### Comparing `solvation-analysis-0.3.2/setup.py` & `solvation-analysis-0.3.3a0/setup.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/_column_names.py` & `solvation-analysis-0.3.3a0/solvation_analysis/_column_names.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/_utils.py` & `solvation-analysis-0.3.3a0/solvation_analysis/_utils.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/coordination.py` & `solvation-analysis-0.3.3a0/solvation_analysis/coordination.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,35 +119,37 @@
         solvent_counts_list = [
             solvent_counts[solvent] for solvent in
             type_counts.index.get_level_values(SOLVENT)
         ]
         type_fractions = type_counts[SOLVENT_ATOM_IX] / solvent_counts_list
         type_fractions.name = FRACTION
         # change index type
-        type_fractions = (type_fractions
-                         .reset_index(ATOM_TYPE)
-                         .astype({ATOM_TYPE: str})
-                         .set_index(ATOM_TYPE, append=True)
-                         )
+        type_fractions = (
+            type_fractions
+            .reset_index(ATOM_TYPE)
+            .astype({ATOM_TYPE: str})
+            .set_index(ATOM_TYPE, append=True)
+        )
         return type_fractions[type_fractions[FRACTION] > tol]
 
     def _calculate_coordination_vs_random(self):
         """
         Calculate the coordination number relative to random coordination.
 
         Values higher than 1 imply a higher coordination than expected from
         random distribution of solvents. Values lower than 1 imply a lower
         coordination than expected from random distribution of solvents.
         """
         average_shell_size = sum(self.coordination_numbers.values())
         total_solvents = sum(self.solvent_counts.values())
         coordination_vs_random = {}
-        for solvent, count in self.solvent_counts.items():
+        for solvent, cn in self.coordination_numbers.items():
+            count = self.solvent_counts[solvent]
             random = count * average_shell_size / total_solvents
-            vs_random = self.coordination_numbers[solvent] / random
+            vs_random = cn / random
             coordination_vs_random[solvent] = vs_random
         return coordination_vs_random
 
     @property
     def coordination_numbers(self):
         """
         A dictionary where keys are residue names (str) and values are the
```

### Comparing `solvation-analysis-0.3.2/solvation_analysis/networking.py` & `solvation-analysis-0.3.3a0/solvation_analysis/networking.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/pairing.py` & `solvation-analysis-0.3.3a0/solvation_analysis/pairing.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/plotting.py` & `solvation-analysis-0.3.3a0/solvation_analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/rdf_parser.py` & `solvation-analysis-0.3.3a0/solvation_analysis/rdf_parser.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/residence.py` & `solvation-analysis-0.3.3a0/solvation_analysis/residence.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/solute.py` & `solvation-analysis-0.3.3a0/solvation_analysis/solute.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/speciation.py` & `solvation-analysis-0.3.3a0/solvation_analysis/speciation.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/conftest.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/.DS_Store` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/README.md` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_fec.data` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec.data`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/ea/topology.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/eaf/topology.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/fea/topology.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/feaf/topology.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/datafiles.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/datafiles.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_coordination.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_coordination.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,31 +14,29 @@
     [
         ("fec", 0.25),
         ("bn", 4.33),
         ("pf6", 0.15),
     ],
 )
 def test_coordination(name, cn, solvation_data, run_solute):
-    atoms = run_solute.u.atoms
-    coordination = Coordination(solvation_data, 10, 49, atoms)
+    coordination = Coordination.from_solute(run_solute)
     np.testing.assert_allclose(cn, coordination.coordination_numbers[name], atol=0.05)
     assert len(coordination.coordination_numbers_by_frame) == 3
 
 
 @pytest.mark.parametrize(
     "name, atom_type, fraction",
     [
         ("fec", '19', 0.008),
         ("bn", '5', 0.9976),
         ("pf6", '21', 1.000),
     ],
 )
 def test_coordinating_atoms(name, atom_type, fraction, solvation_data, run_solute):
-    atoms = run_solute.u.atoms
-    coordination = Coordination(solvation_data, 10, 49, atoms)
+    coordination = Coordination.from_solute(run_solute)
     calculated_fraction = coordination._coordinating_atoms.loc[(name, atom_type)]
     np.testing.assert_allclose(fraction, calculated_fraction, atol=0.05)
 
 
 @pytest.mark.parametrize(
     "name, coord",
     [
```

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_networking.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_pairing.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_pairing.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_plotting.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_rdf_parser.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_rdf_parser.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_residence.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_residence.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_selection.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_solute.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_solute.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis/tests/test_speciation.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_speciation.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/solvation_analysis.egg-info/PKG-INFO` & `solvation-analysis-0.3.3a0/solvation_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvation-analysis
-Version: 0.3.2
+Version: 0.3.3a0
 Summary: A toolkit to analyze solvation structure in molecular dynamics trajectories.
 Author: Orion Cohen
 Author-email: Orion Cohen <orioncohen@berkeley.edu>
 Maintainer-email: Orion Cohen <orioncohen@berkeley.edu>, Hugo MacDermott-Opeskin <hugomacdermott@gmail.com>
 License:                         GNU GENERAL PUBLIC LICENSE 
                                   Version 3, 29 June 2007
```

### Comparing `solvation-analysis-0.3.2/solvation_analysis.egg-info/SOURCES.txt` & `solvation-analysis-0.3.3a0/solvation_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.2/versioneer.py` & `solvation-analysis-0.3.3a0/versioneer.py`

 * *Files identical despite different names*

