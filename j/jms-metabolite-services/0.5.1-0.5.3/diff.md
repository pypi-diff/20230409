# Comparing `tmp/jms-metabolite-services-0.5.1.tar.gz` & `tmp/jms-metabolite-services-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shuzhao/li.github/JMS/dist/.tmp-q35effvk/jms-metabolite-services-0.5.1.tar", last modified: Thu Mar  9 01:53:39 2023, max compression
+gzip compressed data, was "/Users/shuzhao/li.github/JMS/dist/.tmp-jy6lueb_/jms-metabolite-services-0.5.3.tar", last modified: Sun Apr  9 10:42:33 2023, max compression
```

## Comparing `jms-metabolite-services-0.5.1.tar` & `jms-metabolite-services-0.5.3.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/
--rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 jms-metabolite-services-0.5.1/LICENSE
--rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)     4720 2023-01-09 23:02:36.000000 jms-metabolite-services-0.5.1/README.md
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms/
--rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-03-08 18:03:41.000000 jms-metabolite-services-0.5.1/jms/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2338 2023-03-09 01:51:28.000000 jms-metabolite-services-0.5.1/jms/coverage.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms/data/
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:27:53.000000 jms-metabolite-services-0.5.1/jms/data/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)  3085036 2022-02-23 20:21:57.000000 jms-metabolite-services-0.5.1/jms/data/list_formula_mass.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       84 2022-02-10 00:56:47.000000 jms-metabolite-services-0.5.1/jms/data/masters.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    35008 2023-03-09 01:22:13.000000 jms-metabolite-services-0.5.1/jms/dbStructures.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2794 2023-03-09 01:32:16.000000 jms-metabolite-services-0.5.1/jms/empiricalCpds.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     1992 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.1/jms/formula.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4562 2022-02-27 19:09:15.000000 jms-metabolite-services-0.5.1/jms/io.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     1801 2023-03-08 18:14:43.000000 jms-metabolite-services-0.5.1/jms/ions.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     5197 2023-03-09 00:51:03.000000 jms-metabolite-services-0.5.1/jms/modelConvert.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    11998 2023-03-08 17:59:27.000000 jms-metabolite-services-0.5.1/jms/search.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      649 2023-01-01 22:01:32.000000 jms-metabolite-services-0.5.1/jms/test.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       58 2022-02-10 00:39:06.000000 jms-metabolite-services-0.5.1/jms/updates.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms/utils/
--rw-r--r--   0 shuzhao    (501) staff       (20)     6587 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.1/jms/utils/AGORA2JMS.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     5832 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.1/jms/utils/Tabular2Json.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:28:13.000000 jms-metabolite-services-0.5.1/jms/utils/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:16.000000 jms-metabolite-services-0.5.1/jms/utils/chemebi.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     8162 2022-08-26 21:03:43.000000 jms-metabolite-services-0.5.1/jms/utils/gems.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     1960 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.1/jms/utils/git_download.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    11707 2022-02-10 02:05:11.000000 jms-metabolite-services-0.5.1/jms/utils/hmdb.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     6575 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.1/jms/utils/humanGEM2JMS.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:21.000000 jms-metabolite-services-0.5.1/jms/utils/pubchem.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:26.000000 jms-metabolite-services-0.5.1/jms/utils/refmet.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms_metabolite_services.egg-info/
--rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms_metabolite_services.egg-info/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)      723 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms_metabolite_services.egg-info/SOURCES.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms_metabolite_services.egg-info/dependency_links.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       10 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms_metabolite_services.egg-info/requires.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/jms_metabolite_services.egg-info/top_level.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-03-09 01:53:39.000000 jms-metabolite-services-0.5.1/setup.cfg
--rw-r--r--   0 shuzhao    (501) staff       (20)     1300 2022-05-19 20:56:08.000000 jms-metabolite-services-0.5.1/setup.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 jms-metabolite-services-0.5.3/LICENSE
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4720 2023-01-09 23:02:36.000000 jms-metabolite-services-0.5.3/README.md
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms/
+-rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.3/jms/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     2355 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.3/jms/coverage.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms/data/
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:27:53.000000 jms-metabolite-services-0.5.3/jms/data/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)  3085036 2022-02-23 20:21:57.000000 jms-metabolite-services-0.5.3/jms/data/list_formula_mass.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)       84 2022-02-10 00:56:47.000000 jms-metabolite-services-0.5.3/jms/data/masters.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    37884 2023-04-09 02:06:42.000000 jms-metabolite-services-0.5.3/jms/dbStructures.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4548 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.3/jms/empiricalCpds.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     2265 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.3/jms/formula.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4605 2023-04-06 21:06:32.000000 jms-metabolite-services-0.5.3/jms/io.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1801 2023-03-08 18:14:43.000000 jms-metabolite-services-0.5.3/jms/ions.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    10988 2023-04-09 02:08:37.000000 jms-metabolite-services-0.5.3/jms/modelConvert.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)      461 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.3/jms/model_port.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    11998 2023-03-08 17:59:27.000000 jms-metabolite-services-0.5.3/jms/search.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)      649 2023-01-01 22:01:32.000000 jms-metabolite-services-0.5.3/jms/test.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)       58 2022-02-10 00:39:06.000000 jms-metabolite-services-0.5.3/jms/updates.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms/utils/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5832 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.3/jms/utils/Tabular2Json.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:28:13.000000 jms-metabolite-services-0.5.3/jms/utils/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:16.000000 jms-metabolite-services-0.5.3/jms/utils/chemebi.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    10125 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.3/jms/utils/gems.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    11707 2022-02-10 02:05:11.000000 jms-metabolite-services-0.5.3/jms/utils/hmdb.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:21.000000 jms-metabolite-services-0.5.3/jms/utils/pubchem.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:26.000000 jms-metabolite-services-0.5.3/jms/utils/refmet.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)      666 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/SOURCES.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/dependency_links.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)       10 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/requires.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/top_level.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/setup.cfg
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1300 2022-05-19 20:56:08.000000 jms-metabolite-services-0.5.3/setup.py
```

### Comparing `jms-metabolite-services-0.5.1/LICENSE` & `jms-metabolite-services-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.1/PKG-INFO` & `jms-metabolite-services-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jms-metabolite-services
-Version: 0.5.1
+Version: 0.5.3
 Summary: conversion, search of metabolic models and metabolomics data
 Home-page: https://github.com/shuzhao-li/JMS
 Author: Shuzhao Li, Minghao Gong
 Author-email: shuzhao.li@gmail.com
 License: Python
 Keywords: metabolomics,chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jms-metabolite-services-0.5.1/README.md` & `jms-metabolite-services-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.1/jms/coverage.py` & `jms-metabolite-services-0.5.3/jms/coverage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 '''
 Test coverage of a dataset or a model on pathways/ontologies.
 
 Could exclude currency metabolites in future.
+
+To refactor -
+
+
 '''
 
 from .modelConvert import convert_json_model
 from .search import build_centurion_tree
 from .empiricalCpds import *
```

### Comparing `jms-metabolite-services-0.5.1/jms/data/list_formula_mass.py` & `jms-metabolite-services-0.5.3/jms/data/list_formula_mass.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.1/jms/dbStructures.py` & `jms-metabolite-services-0.5.3/jms/dbStructures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 '''
 Class structures to connect metabolite/compound databases to empirical compounds;
 and to connect experimental data to empirical compounds.
 '''
+
 import json
 from operator import itemgetter
 import numpy as np
 
 from khipu.epdsConstructor import epdsConstructor
 
 from khipu.utils import adduct_search_patterns, \
@@ -15,40 +16,58 @@
 
 from .search import *
 from .formula import *
 from .ions import compute_adducts_formulae, generate_ion_signature
 from .data.list_formula_mass import list_formula_mass
 
 
-def annotate_peaks_against_kcds(list_peaks, list_compounds, 
+def annotate_peaks_against_kcds(list_peaks, 
+                                list_compounds, 
                                 export_file_name_prefix='jms_annotated_',
-                                mode='pos',  mz_tolerance_ppm=5, check_isotope_ratio = True):
+                                mode='pos',  
+                                mz_tolerance_ppm=5, 
+                                rt_tolerance = 2,
+                                check_isotope_ratio = False):
     '''
     Wrapper function as example, to generate three annotation files for input list_peaks.
     list_compounds is known compound database, e.g.
     list_compounds = json.load(open('jms/data/compounds/list_compounds_HMDB4.json'))
-    
+    list_peaks is experimental data, list of features in json.
     '''
     KCD = knownCompoundDatabase()
     KCD.mass_index_list_compounds(list_compounds)
     KCD.build_emp_cpds_index()
-    KCD.export_mass_indexed_compounds(export_file_name_prefix+"KCD_mass_indexed_compounds.json")
-    EED = ExperimentalEcpdDatabase(mode=mode, mz_tolerance_ppm=mz_tolerance_ppm)
+    # optional to export_mass_indexed_compounds
+    # KCD.export_mass_indexed_compounds(export_file_name_prefix+"KCD_mass_indexed_compounds.json")
+
+    EED = ExperimentalEcpdDatabase(mode=mode, 
+                                   mz_tolerance_ppm=mz_tolerance_ppm,
+                                   rt_tolerance=rt_tolerance)
     EED.build_from_list_peaks(list_peaks)
+    # Second, singletons that get a formula match in KCD
+    EED.annotate_singletons(KCD)       
+    # Third, the remaining features unmatched to anything (orphans). Exported for potential downstream work.
+    # EED.dict_empCpds = self.append_orphans_to_epmCpds(EED.dict_empCpds)
+    
     EED.export_annotations(KCD, export_file_name_prefix)
 
 
 #----------------------------------------------------------------------------------------
 class knownCompoundDatabase:
     '''
-    Indexed data store for known compounds. 
-    One can search by mass or mass tree (patterns of isotopes/adducts, in the form of empCpd).
-    centurion_mass_tree is an indexed dictionary to group ions by 100th decimal.
+    Indexed data store for known compounds, e.g., from a database or a metabolic model. 
+    The search should be on empCpd not Cpd.
     An empCpd is an empirical compound, a set of features drived from the same mass (see README), 
-    which often include isomers.
+    which often include isomers. The regular mass search cannot distinguish isomers.
+
+    One can search by mass or mass tree (patterns of isotopes/adducts, in the form of empCpd.
+    We use build_centurion_tree to index empCpds;
+    centurion_mass_tree is an indexed dictionary to group ions by 100th decimal.
+    There are situations where only neutral mass is searched; others requiring ionized forms.
+    This class generates three trees to accommodate them: 'neutral', 'pos' and 'neg'.
     '''
     def __init__(self):
         '''
         Two main data containers, mass_indexed_compounds and emp_cpds_trees.
         The latter is indexed for searches, separately for positive and negative ion modes.
         '''
         self.mass_indexed_compounds = {}
@@ -83,15 +102,16 @@
 
         Update
         ======
         self.mass_indexed_compounds so that isomers are grouped under same empCpd.
         '''
         _db = {}
         for cpd in list_compounds:
-            k = cpd['neutral_formula']+ '_' + str(round(float(cpd['neutral_formula_mass']),6))  # ensuring unique formula and mass
+            k = cpd['neutral_formula']+ '_' + str(round(float(cpd['neutral_formula_mass']),6))  
+            # ensuring unique formula and mass
             if k in _db:  
                 _db[k].append( cpd )  
             else:  
                 _db[k] = [cpd]  
 
         for k,v in _db.items():
             self.mass_indexed_compounds[k] = {
@@ -127,15 +147,15 @@
             __ion_generator__ = generate_ion_signature
 
         pos_peak_list, neg_peak_list, neutral_peak_list = [], [], []
         pos_epd_ions, neg_epd_ions = {}, {}     # dictionaries using same keys as self.mass_indexed_compounds
         for k, v in self.mass_indexed_compounds.items():
             # neutral
             neutral_peak_list.append(
-                {'mz': v['neutral_formula_mass'], 'parent_epd_id': k, 'ion_relation': '',}
+                {'mz': v['neutral_formula_mass'], 'parent_epd_id': k, 'ion_relation': 'neutral',}
             )
 
             # do pos ions now
             __LL = __ion_generator__(v['neutral_formula_mass'], v['neutral_formula'], mode='pos', primary_only=True)
             # signature format e.g. [[304.203251, 'M[1+]', 'C19H28O3'], ...]
             pos_epd_ions[k] = __LL
             for ion in __LL:
@@ -185,40 +205,41 @@
             return ratio
         else:
             print("No m/z match found in database to estimate mass accuracy.")
             return None
 
     def search_emp_cpd_single(self, emp_cpd, mode='pos', mz_tolerance_ppm=5):
         '''
-        If input emp_cpd is from khipu, neutral_formula_mass is usually alrady assigned. 
-        This is simple search on neutral_formula_mass.
-        Otherwise, emp_cpd format has to follow (loosely) specificiations in metDataModel, requiring anchor ion, e.g.
+        emp_cpd : empirical compound, following loosely specificiations in metDataModel, e.g.
         {interim_id': 12,
         'neutral_formula_mass': None,
         'neutral_formula': None,
         'MS1_pseudo_Spectra': [{'id_number': 'F94',
                                 'mz': 98.97531935309317,
                                 'rtime': 700.0,
                                 'charged_formula': '',
                                 'ion_relation': 'anchor',
                                 'parent_epd_id': 12}, ], ...}
-        Note that neutral_formula is not assigned from experimental measurements, which only indicate m/z distances
-        between coeluting ions. 
-        The emp_cpds_trees (from mass_indexed_compounds) only considers primary ions here, and
-        should NOT include isotopes, which are considered in the experimental data.
+
+        If input emp_cpd is generated from khipu, neutral_formula_mass is usually alrady assigned, 
+        and this is simple search on neutral_formula_mass.
+        Otherwise, anchor ion is searched in emp_cpds_trees (from mass_indexed_compounds).
         The ion_relations are expected to be ['M[1+]', 'M+H[1+]', 'M+Na[1+]', 'M+H2O+H[1+]'] for pos,
         and ['M[-]', 'M-H[-]', 'M-H2O-H[-]', 'M+Cl[-]'] for neg.
 
+        This searches only neutral mass or anchor ion, because if anchor ion is not found in the database, 
+        other adducts are not possible.
+
         Return
         ======
         list of matched db empCpd as [(empCpd_id, ion_relation, score), ...], sorted by score.
-        While most search will return a single match, undeterministic situations exist,
+        While most search will return a single match. Occasionally, undeterministic situations appear,
         e.g. C6H13N and C6H14N could match to M+ and M+H+, respectively.
         The resolution of these will be left to downstream methods (bayesian etc).
-        The score is number of matched ions.
+        The score is number of matched ions, which may or may not be useful.
         '''
         results = []
         if emp_cpd['neutral_formula_mass']:
             matches = self.search_mz_single(emp_cpd['neutral_formula_mass'], 'neutral', mz_tolerance_ppm)
             for _M in matches:
                 results.append((_M['parent_epd_id'],
                                 _M['ion_relation'], 1))
@@ -258,61 +279,62 @@
         '''
         pass
 
 
 #----------------------------------------------------------------------------------------
 class ExperimentalEcpdDatabase:
     '''
-    Build a boutique data store for user's experimental data, input being list of peaks or empCpds (i.e. emp_cpd).
+    Build a boutique data store for user's experimental data, list of JSON features/peaks.
     Allow search of Compounds, which support targeted compound search in a dataset.
-
-    The construction of empirical compounds (empCpds) is based on 
-    1) initial search of ion patterns (C13, +H, +Na, -H, +Na-2H +Cl-) based on mass2chem.epdsConstructor
-    2) match to databased generated through knownCompoundDatabase
-    3) augment formula match via data.list_formula_mass (HMDB4+PubChemLite)
-    4) formula based grid search to extend all empCpds
-
-    self.dict_empCpds is updated in situ.
-    Not using check_isotope_ratios. First pass by khipu generates JSON annotations, 
-        where ratios can be calculated after.
     '''
-    def __init__(self, mode='pos', mz_tolerance_ppm=5, rt_tolerance=2):
+    def __init__(self, 
+                 mode='pos', 
+                 mz_tolerance_ppm=5, 
+                 rt_tolerance=2,
+                 ):
         '''
         mode: ionizaation mode, 'pos' or 'neg'.
         mz_tolerance_ppm: ppm tolerance in examining m/z patterns.
         rt_tolerance: tolerance threshold for deviation in retetion time, arbitrary unit depending on input data.
                 Default intended as 2 seconds.
-        Takes input list of peaks. Peaks here are usually features.
+        The isotope/adduct patterns here are populated via self.get_isotope_adduct_patterns, as imported from khipu.
+        But one can directly overwrite the patterns for customization (e.g. in asari).
         '''
         self.mode = mode
         self.mz_tolerance_ppm = mz_tolerance_ppm
         self.rt_tolerance = rt_tolerance
         self.get_isotope_adduct_patterns()
         self.list_peaks = []
         self.indexed_peaks = {}
         self.dict_peaks = {}
         self.dict_empCpds = {}
         self.indexed_empCpds = {}
         self.peak_to_empCpd = {}
         self.peak_to_empCpd_ion_relation = {}
 
-    def get_isotope_adduct_patterns(self):
+    def get_isotope_adduct_patterns(self, 
+                                    adduct_search_patterns=adduct_search_patterns,
+                                    adduct_search_patterns_neg=adduct_search_patterns_neg,
+                                    isotope_search_patterns=isotope_search_patterns[:2],
+                                    extended_adducts=extended_adducts
+                                    ):
         '''
         Populate isotope/adduct patterns for this instance.
-        The isotope/adduct patterns here are imported from khipu as global variables here.
+        The default isotope/adduct patterns here are imported from khipu.
+        The default isotope_search_patterns are limited to M0 and M1.
         '''
         self.adduct_patterns = adduct_search_patterns
         if self.mode == 'neg':
             self.adduct_patterns = adduct_search_patterns_neg
         self.isotope_search_patterns = isotope_search_patterns
         self.extended_adducts = extended_adducts
 
     def build_from_list_peaks(self, list_peaks):
         '''
-        Wrapper of khipu epdsConstructor.
+        Wrapper of khipu epdsConstructor, to construct empirical compounds (empCpds).
         Updates self.dict_empCpds and does self.index_empCpds().
 
         list_peaks : [{'parent_masstrace_id': 1670, 'mz': 133.09702315984987, 'rtime': 654, 
                 'height': 14388.0, 'id_number': 555}, ...]
         isotope/adduct patterns, mz_tolerance_ppm and rt_tolerance are from self,
         as they are parameters to this class.
 
@@ -346,21 +368,25 @@
         for E in list_empCpds:
             self.dict_empCpds[E['interim_id']] = E
         self.index_empCpds()
 
     def index_empCpds(self):
         '''
         Build indices for self.list_peaks and self.empCpds.
-        Minor possibility that peak:empCpd is not N:1.
-        round 1 index of self.dict_empCpds; round 2 to be done after annotation
+        Khipu has peak:empCpd built N:1 but other methods should comply too.
+
+        Updates
+        -------
+        self.indexed_peaks, self.formula_tree, self.indexed_empCpds
         '''
         for P in self.list_peaks:
             self.dict_peaks[P['id_number']] = P
 
         self.indexed_peaks  = build_centurion_tree(self.list_peaks)
+        # use formula.get_formula_ions_tree
         self.formula_tree = get_formula_ions_tree(list_formula_mass, mode=self.mode)
 
         __PL = []
         for interim_id, epd in self.dict_empCpds.items():
             peaks = epd['MS1_pseudo_Spectra']
             for P in peaks:
                 self.peak_to_empCpd[P['id_number']] = interim_id
@@ -421,21 +447,16 @@
                 self.search_peaks_compound_single(cpd, cpd, mz_tolerance_ppm)
             )
         return results
 
     def annotate_empCpds_against_KCD(self, KCD, mz_tolerance_ppm=5):
         '''
         Get all empCpd matches between this experimental dataset and a known compound database.
-        KCD: knownCompoundDatabase instance.
-        >>> KCD.search_emp_cpd_single( EED.dict_empCpds[15] )
-        [('C6H14N_100.112624', 'M[1+]', 2), ('C6H13N_99.104799', 'M+H[1+]', 2)]
-        This search empCpds first, in which only anchor ion is searched. 
-        Because if anchor ion is not found in the database, other adducts are not possible.
-
-        return dictionary e.g.
+        KCD: knownCompoundDatabase instance. KCD.search_emp_cpd_single() searches only neutral mass or anchor ion. 
+        Returns dictionary e.g.
                 {(101, []),
                 (102,
                 [('C9H20NO2_174.149404', 'M[1+]', 2),
                 ('C9H17NO_155.131014', 'M+H2O+H[1+]', 1)]),
                 (103,
                 [('C6H15N4O2_175.119501', 'M[1+]', 2),
                 ('C6H14N4O2_174.111676', 'M+H[1+]', 2)]),
@@ -454,101 +475,138 @@
                                'neutral_formula_mass': mass}
         '''
         return search_mz_formula_tree(mz, self.formula_tree, limit_ppm=mz_tolerance_ppm)
 
     # Annotation functions
     def extend_empCpd_annotation(self, KCD):
         '''
-        Before khipu:
-        self.empCpds_formula_search(KCD)
-        self.__extend_empCpds__()
+        This searches KCD for the list of empCpds.
+        With khipu, most empCpds have neutral mass, which is used for KCD search.
+        If no neutral mass, an anchor ion is used for KCD search (KCD.search_emp_cpd_single).
+        Returned list_matches have KCD empCpd identifiers but compound records need to pull out KCD later.
         '''
         epd_search_result_dict = self.annotate_empCpds_against_KCD(KCD, self.mz_tolerance_ppm)
         for interim_id, V in epd_search_result_dict.items():
             if V:
                 self.dict_empCpds[interim_id]['list_matches'] = V
 
-
     def empCpds_formula_search(self, KCD):
         '''
         Update self.dict_empCpds for formulae first by KCD search then .data.formula_tree.
         KCD: knownCompoundDatabase instance.
         '''
         epd_search_result_dict = self.annotate_empCpds_against_KCD(KCD, self.mz_tolerance_ppm)
         for interim_id, V in epd_search_result_dict.items():
             if V:
                 # update empCpd with formula matches
                 self.dict_empCpds[interim_id]['list_matches'] = V
                 #       expecting probem from khipu to this
-                self.dict_empCpds[interim_id]['neutral_formula'] = KCD.mass_indexed_compounds[V[0][0]]['neutral_formula']
-                self.dict_empCpds[interim_id]['neutral_formula_mass'] = KCD.mass_indexed_compounds[V[0][0]]['neutral_formula_mass']
+                self.dict_empCpds[interim_id]['neutral_formula'] = \
+                    KCD.mass_indexed_compounds[V[0][0]]['neutral_formula']
+                self.dict_empCpds[interim_id]['neutral_formula_mass'] = \
+                    KCD.mass_indexed_compounds[V[0][0]]['neutral_formula_mass']
             else:
                 # first peak should be anchor
                 anchor_mz = self.dict_empCpds[interim_id]['MS1_pseudo_Spectra'][0]['mz']
                 F = self.search_mz_for_formula(anchor_mz, self.mz_tolerance_ppm)
                 if F:
                     self.dict_empCpds[interim_id]['neutral_formula'] = F['neutral_formula']
                     self.dict_empCpds[interim_id]['neutral_formula_mass'] = F['neutral_formula_mass']
 
     def __extend_empCpds__(self):
         '''
         Extend empCpds by 
         additional isotopes/adducts, based on mass2chem.formula.compute_adducts_formulae
 
-        Hold off from khipu results.
+        Hold off; no need now from khipu results.
         '''
         peakList = [P for P in self.list_peaks if P['id_number'] not in self.peak_to_empCpd]
         peakTree = build_centurion_tree(peakList)
         for k,E in self.dict_empCpds.items():
             if E['neutral_formula']:
                 anchor = E['MS1_pseudo_Spectra'][0]
                 expected_ions = compute_adducts_formulae(E['neutral_formula_mass'], 
                                                 E['neutral_formula'], self.mode, primary_only=False)
                                                 # [(58.53894096677, 'M+2H[2+]', result_formula), ...,]
                 for ion in expected_ions:
                     matches = find_all_matches_centurion_indexed_list(ion[0], peakTree, self.mz_tolerance_ppm)
                     for peak in matches:
-                        if is_coeluted(anchor, peak, rt_tolerance=10):
+                        if is_coeluted(anchor, peak, rt_tolerance=self.rt_tolerance):
                             peak['ion_relation'] = ion[1]
                             E['MS1_pseudo_Spectra'].append(peak)
                             self.peak_to_empCpd_ion_relation[peak['id_number']] = peak['ion_relation']
                             self.peak_to_empCpd[peak['id_number']] = E['interim_id']
                             # this may overwrite 1:N relationships
 
     def singleton_formula_search(self, KCD):
         '''
         Search singletons for formulae first by KCD search then .data.formula_tree.
         KCD: knownCompoundDatabase instance.
+
+        Returns
+        -------
+        List of first matched KCD compound for each singleton in self.dict_peaks, e.g.
+        [('F17904', {'interim_id': 15321, 'neutral_formula_mass': 916.606449, 'neutral_formula': 'C56H84O10',...}), ...]
         '''
         found = []
         singletons = [p for p in self.dict_peaks if p not in self.peak_to_empCpd.keys()]
         for p in singletons:
             _mz = self.dict_peaks[p]['mz']
             list_matches = KCD.search_mz_single(_mz, self.mode, self.mz_tolerance_ppm)
             # [{'mz': 130.017306555, 'parent_epd_id': 'C4H3FN2O2_130.017856', 'ion_relation': 'M[1+]'}]
             if list_matches:
-                # take 1st match only here
+                # take 1st match only here; will model better in future
                 _epd = KCD.mass_indexed_compounds[list_matches[0]['parent_epd_id']]
+                _epd['isotope'] = '13C/12C'
+                _epd['ion_relation'] = _epd['modification'] = list_matches[0]['ion_relation']
                 found.append((p, _epd))
             else:
                 # formula search
                 F = self.search_mz_for_formula(_mz, self.mz_tolerance_ppm)
                 if F:
                     found.append((p, F))            # p is id_number
 
         return found
+    
+
+    def annotate_singleton_mummichog(self, KCD):
+        '''
+        This applies to KCD using a metabolic model as the sole database.
+
+        Updates
+        -------
+        self.dict_empCpds : {id: empCpd, ...}
+        '''
+        singletons = [p for p in self.dict_peaks if p not in self.peak_to_empCpd.keys()]
+        for p in singletons:
+            peak = self.dict_peaks[p]
+            interim_id = 'epd_' + peak['id_number']
+            list_matches = KCD.search_mz_single(peak['mz'], self.mode, self.mz_tolerance_ppm)
+            # [{'mz': 130.017306555, 'parent_epd_id': 'C4H3FN2O2_130.017856', 'ion_relation': 'M[1+]'}]
+            if list_matches:
+                self.dict_empCpds[interim_id] = {'interim_id': interim_id,
+                    'MS1_pseudo_Spectra': [peak],
+                    'list_matches': [(LL['parent_epd_id'], LL['ion_relation'], 1) for LL in list_matches],
+                }
+
 
     def annotate_singletons(self, KCD):
         '''
         Search singletons for formulae first by KCD search then .data.formula_tree.
         Add new empCpds to self.dict_empCpds as new empCpds, and extend adduct search.
         Assign new identifiers as (10000 +number of dict_empCpds + numerical count).
+
+        Updates
+        -------
+        self.dict_empCpds : {id: empCpd, ...}
         '''
         formula_to_peaks = {}
         found = self.singleton_formula_search(KCD)
+        # multiple singletons can match to same formula as different ions, 
+        # if ion calculation differs btw here and KCD
         for p,F in found:
             k = F['neutral_formula']
             if k in formula_to_peaks:
                 formula_to_peaks[k].append((p, F))
             else:
                 formula_to_peaks[k] = [(p, F)]
 
@@ -560,15 +618,15 @@
         new_id_start = len(self.dict_empCpds) + 10000
         for formula, PP in formula_to_peaks.items():
             neutral_formula_mass = PP[0][1]['neutral_formula_mass']
             P1 = self.dict_peaks[PP[0][0]]
             tmp = [P1, ]
             for jj in range(1, len(PP)):
                 _P = self.dict_peaks[PP[jj][0]]
-                if is_coeluted(tmp[-1], _P, rt_tolerance=10):
+                if is_coeluted(tmp[-1], _P, rt_tolerance=self.rt_tolerance):
                     tmp.append(_P)
                 else:
                     # not coeluted, new empCpd
                     new_id_start += 1
                     self.dict_empCpds[new_id_start] = {'interim_id': new_id_start,
                             'neutral_formula_mass': neutral_formula_mass, 'neutral_formula': formula,
                             'MS1_pseudo_Spectra': self.__extend_peakList__(
@@ -593,22 +651,24 @@
         '''
         new = []
         anchor = epd_peaks[0]
         for ion in compute_adducts_formulae(neutral_formula_mass, neutral_formula,
                                         self.mode, primary_only=False):
             matches = find_all_matches_centurion_indexed_list(ion[0], peakTree, mz_tolerance_ppm)
             for peak in matches:
-                if is_coeluted(anchor, peak, rt_tolerance=10):
+                if is_coeluted(anchor, peak, rt_tolerance=self.rt_tolerance):
                     peak['ion_relation'] = ion[1]
                     new.append(peak)
         return epd_peaks + new
 
 
     def annotate_all_against_KCD(self, KCD, mz_tolerance_ppm=5):
         '''
+        Not used now.
+
         Get matches of both empCpds and singleton peaks only in KCD.
         This function should not be used if one uses empCpds_formula_search and annotate_by_formula_grid.
         Results contain annotation via empCpd, via singleton, or empCpd features as if singleton.
 
         KCD: knownCompoundDatabase instance.
         return: peak_result_dict, epd_search_result_dict
         '''
@@ -650,46 +710,45 @@
 
 
     def export_empCpds(self, outfile="EED_empCpds.json"):
         with open(outfile, 'w', encoding='utf-8') as O:
             json.dump(list(self.dict_empCpds.values()), O, ensure_ascii=False, indent=2)
 
 
-    def export_annotations(self, KCD, export_file_name_prefix, include_succinct=False):
+    def export_annotations(self, KCD, export_file_name_prefix):
         '''
-        Export expt empCpds, match relationships, and a tsv table for input list_peaks, with all matched db empCpds.
-
-        To-do:
-        Will add option to include a version succinct annotation of anchor ions and recommended matches only.
+        Export expt empCpds and a tsv table for input list_peaks, with all matched db empCpds.
         '''
-        peak_result_dict, epd_search_result_dict = self.annotate_all_against_KCD(KCD)
-
         self.export_empCpds(export_file_name_prefix+"EED_empCpds.json")
-        with open(export_file_name_prefix+"mapping.json", 'w', encoding='utf-8') as O:
-            json.dump(epd_search_result_dict, O, ensure_ascii=False, indent=2)
-
-        s = "[peak]id_number\tmz\tapex\t[EmpCpd]interim_id\t[EmpCpd]ion_relation\tmatched_DB_shorts\tmatched_DB_records\n"
-        for ii, V in peak_result_dict.items():
-            matched_DB_shorts, matched_DB_records = '', ''
-            list_matches = V['list_matches']
-            if list_matches:
+        s = "[peak]id_number\tmz\trtime\tapex(scan number)\t[EmpCpd]interim_id\t[EmpCpd]ion_relation\tneutral_formula\tneutral_formula_mass\
+        \tname_1st_guess\tmatched_DB_shorts\tmatched_DB_records\n"
+        
+        for _, V in self.dict_empCpds.items():
+            name_1st_guess, matched_DB_shorts, matched_DB_records = '', '', ''
+            if 'list_matches' in V:
+                list_matches = V['list_matches']
+                if list_matches:
+                    name_1st_guess = KCD.mass_indexed_compounds[list_matches[0][0]]['compounds'][0]['name']
                     matched_DB_shorts = ", ".join([ "(" + KCD.short_report_emp_cpd(xx[0]) + ")"  for xx in list_matches])
                     matched_DB_records = ", ".join([str(xx) for xx  in list_matches])
 
-            s += '\t'.join([str(x) for x in [
-                ii, V['peak']['mz'], V['peak']['apex'], V['interim_id'], V['epd_ion_relation'],
-                matched_DB_shorts, matched_DB_records]]) + "\n"
+            for peak in V['MS1_pseudo_Spectra']:
+                s += '\t'.join([str(x) for x in [
+                    peak['id_number'], peak['mz'], peak['rtime'], peak['apex'], V['interim_id'], peak.get('ion_relation', ''),
+                    V['neutral_formula'], V['neutral_formula_mass'],
+                    name_1st_guess, matched_DB_shorts, matched_DB_records]]) + "\n"
 
         outfile = export_file_name_prefix + '.tsv'
-        with open(outfile, 'w') as O:
+        with open(outfile, encoding='utf-8', mode='w') as O:
             O.write(s)
 
         print("\nAnnotation of %d Empirical compounds was written to %s." %(len(self.dict_empCpds), outfile))
 
 
+
     #-----------------------------------------
 
     def update_annotation(self, KCD, peak_result_dict, adduct_patterns, mz_tolerance_ppm):
         '''
         Placeholder. Not used now but for future consieration -
 
         Update self.dict_empCpds, and extend search by formula-based additional isotopes/adducts.
```

### Comparing `jms-metabolite-services-0.5.1/jms/formula.py` & `jms-metabolite-services-0.5.3/jms/formula.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,25 +29,42 @@
     '''
     return the best matched ion (as peak format) in formula_tree.
 
     formula_tree = get_formula_ions_tree(list_formula_mass, mode='pos')
     '''
     return find_best_match_centurion_indexed_list(mz, formula_tree, limit_ppm)
 
-def adjust_charge_in_formula(charged_formula,charge): 
-    '''
-    adjust charged formula to neutral formula
-    '''
+def adjust_charge_in_formula(charged_formula:str,charge:int)->str: 
+    """adjust charged formula to neutral formula
+
+    Parameters
+    ----------
+    charged_formula : str
+        charged formula
+    charge : int
+        charge
+
+    Returns
+    -------
+    str
+        neutral formula
+
+    Examples
+    --------
+    >>> adjust_charge_in_formula('C17H31O2',-1)
+    'C17H32O2'
+    
+    """ 
     if charge == 0:
         result = charged_formula
     else:
         formula_dict = parse_chemformula_dict(charged_formula)
         hydrogen_dict = {'H':-charge}
         hypothetical_neutral_formula_dict = add_formula_dict(formula_dict, hydrogen_dict)
         if hypothetical_neutral_formula_dict:
             result = dict_to_hill_formula(hypothetical_neutral_formula_dict)
         else: 
             if charge < 0:
                 result = None
             else:  # if charge >0, e.g., Fe, charge is 2+; it should still be Fe as formula
                 result = charged_formula # here dealing with Metal etc.
-    return(result)
+    return result
```

### Comparing `jms-metabolite-services-0.5.1/jms/io.py` & `jms-metabolite-services-0.5.3/jms/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         if feature_id != None:
             fid = a[feature_id].strip()
         else:
             ii += 1
             fid = _make_id(ii, mz, rt)
         peak = {'id_number': fid, 'mz': mz, 'rtime': rt, 'apex': rt}
         if has_header and full_extract:
+            # will remove redundant fields
             peak2 = dict(zip(header, a))
             peak2.update(peak)
             peak = peak2
 
         list_peaks.append( peak )
 
     return list_peaks
```

### Comparing `jms-metabolite-services-0.5.1/jms/ions.py` & `jms-metabolite-services-0.5.3/jms/ions.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.1/jms/search.py` & `jms-metabolite-services-0.5.3/jms/search.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.1/jms/test.py` & `jms-metabolite-services-0.5.3/jms/test.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.1/jms/utils/Tabular2Json.py` & `jms-metabolite-services-0.5.3/jms/utils/Tabular2Json.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.1/jms/utils/hmdb.py` & `jms-metabolite-services-0.5.3/jms/utils/hmdb.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.1/jms_metabolite_services.egg-info/PKG-INFO` & `jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jms-metabolite-services
-Version: 0.5.1
+Version: 0.5.3
 Summary: conversion, search of metabolic models and metabolomics data
 Home-page: https://github.com/shuzhao-li/JMS
 Author: Shuzhao Li, Minghao Gong
 Author-email: shuzhao.li@gmail.com
 License: Python
 Keywords: metabolomics,chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jms-metabolite-services-0.5.1/jms_metabolite_services.egg-info/SOURCES.txt` & `jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 jms/coverage.py
 jms/dbStructures.py
 jms/empiricalCpds.py
 jms/formula.py
 jms/io.py
 jms/ions.py
 jms/modelConvert.py
+jms/model_port.py
 jms/search.py
 jms/test.py
 jms/updates.py
 jms/data/__init__.py
 jms/data/list_formula_mass.py
 jms/data/masters.py
-jms/utils/AGORA2JMS.py
 jms/utils/Tabular2Json.py
 jms/utils/__init__.py
 jms/utils/chemebi.py
 jms/utils/gems.py
-jms/utils/git_download.py
 jms/utils/hmdb.py
-jms/utils/humanGEM2JMS.py
 jms/utils/pubchem.py
 jms/utils/refmet.py
 jms_metabolite_services.egg-info/PKG-INFO
 jms_metabolite_services.egg-info/SOURCES.txt
 jms_metabolite_services.egg-info/dependency_links.txt
 jms_metabolite_services.egg-info/requires.txt
 jms_metabolite_services.egg-info/top_level.txt
```

### Comparing `jms-metabolite-services-0.5.1/setup.py` & `jms-metabolite-services-0.5.3/setup.py`

 * *Files identical despite different names*

