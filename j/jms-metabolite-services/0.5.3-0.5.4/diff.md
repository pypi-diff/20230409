# Comparing `tmp/jms-metabolite-services-0.5.3.tar.gz` & `tmp/jms-metabolite-services-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shuzhao/li.github/JMS/dist/.tmp-jy6lueb_/jms-metabolite-services-0.5.3.tar", last modified: Sun Apr  9 10:42:33 2023, max compression
+gzip compressed data, was "/Users/shuzhao/li.github/JMS/dist/.tmp-z4wejmnf/jms-metabolite-services-0.5.4.tar", last modified: Sun Apr  9 12:04:54 2023, max compression
```

## Comparing `jms-metabolite-services-0.5.3.tar` & `jms-metabolite-services-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/
--rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 jms-metabolite-services-0.5.3/LICENSE
--rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)     4720 2023-01-09 23:02:36.000000 jms-metabolite-services-0.5.3/README.md
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms/
--rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.3/jms/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2355 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.3/jms/coverage.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms/data/
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:27:53.000000 jms-metabolite-services-0.5.3/jms/data/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)  3085036 2022-02-23 20:21:57.000000 jms-metabolite-services-0.5.3/jms/data/list_formula_mass.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       84 2022-02-10 00:56:47.000000 jms-metabolite-services-0.5.3/jms/data/masters.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    37884 2023-04-09 02:06:42.000000 jms-metabolite-services-0.5.3/jms/dbStructures.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4548 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.3/jms/empiricalCpds.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     2265 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.3/jms/formula.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4605 2023-04-06 21:06:32.000000 jms-metabolite-services-0.5.3/jms/io.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     1801 2023-03-08 18:14:43.000000 jms-metabolite-services-0.5.3/jms/ions.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    10988 2023-04-09 02:08:37.000000 jms-metabolite-services-0.5.3/jms/modelConvert.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      461 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.3/jms/model_port.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    11998 2023-03-08 17:59:27.000000 jms-metabolite-services-0.5.3/jms/search.py
--rw-r--r--   0 shuzhao    (501) staff       (20)      649 2023-01-01 22:01:32.000000 jms-metabolite-services-0.5.3/jms/test.py
--rw-r--r--   0 shuzhao    (501) staff       (20)       58 2022-02-10 00:39:06.000000 jms-metabolite-services-0.5.3/jms/updates.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms/utils/
--rw-r--r--   0 shuzhao    (501) staff       (20)     5832 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.3/jms/utils/Tabular2Json.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:28:13.000000 jms-metabolite-services-0.5.3/jms/utils/__init__.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:16.000000 jms-metabolite-services-0.5.3/jms/utils/chemebi.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    10125 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.3/jms/utils/gems.py
--rw-r--r--   0 shuzhao    (501) staff       (20)    11707 2022-02-10 02:05:11.000000 jms-metabolite-services-0.5.3/jms/utils/hmdb.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:21.000000 jms-metabolite-services-0.5.3/jms/utils/pubchem.py
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:26.000000 jms-metabolite-services-0.5.3/jms/utils/refmet.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/
--rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)      666 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/SOURCES.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/dependency_links.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       10 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/requires.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/top_level.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-04-09 10:42:33.000000 jms-metabolite-services-0.5.3/setup.cfg
--rw-r--r--   0 shuzhao    (501) staff       (20)     1300 2022-05-19 20:56:08.000000 jms-metabolite-services-0.5.3/setup.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1073 2020-05-11 14:03:57.000000 jms-metabolite-services-0.5.4/LICENSE
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4720 2023-01-09 23:02:36.000000 jms-metabolite-services-0.5.4/README.md
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms/
+-rw-r--r--   0 shuzhao    (501) staff       (20)       22 2023-04-09 12:03:10.000000 jms-metabolite-services-0.5.4/jms/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     2355 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.4/jms/coverage.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms/data/
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:27:53.000000 jms-metabolite-services-0.5.4/jms/data/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)  3085036 2022-02-23 20:21:57.000000 jms-metabolite-services-0.5.4/jms/data/list_formula_mass.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)       84 2022-02-10 00:56:47.000000 jms-metabolite-services-0.5.4/jms/data/masters.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    37884 2023-04-09 02:06:42.000000 jms-metabolite-services-0.5.4/jms/dbStructures.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4548 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.4/jms/empiricalCpds.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     2265 2023-04-03 14:08:48.000000 jms-metabolite-services-0.5.4/jms/formula.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     4605 2023-04-06 21:06:32.000000 jms-metabolite-services-0.5.4/jms/io.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1801 2023-03-08 18:14:43.000000 jms-metabolite-services-0.5.4/jms/ions.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    14262 2023-04-09 12:03:10.000000 jms-metabolite-services-0.5.4/jms/modelConvert.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)      461 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.4/jms/model_port.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    11998 2023-03-08 17:59:27.000000 jms-metabolite-services-0.5.4/jms/search.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)      649 2023-01-01 22:01:32.000000 jms-metabolite-services-0.5.4/jms/test.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)       58 2022-02-10 00:39:06.000000 jms-metabolite-services-0.5.4/jms/updates.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms/utils/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5832 2022-05-19 20:33:17.000000 jms-metabolite-services-0.5.4/jms/utils/Tabular2Json.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 02:28:13.000000 jms-metabolite-services-0.5.4/jms/utils/__init__.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:16.000000 jms-metabolite-services-0.5.4/jms/utils/chemebi.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    10125 2023-04-06 15:29:23.000000 jms-metabolite-services-0.5.4/jms/utils/gems.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)    11707 2022-02-10 02:05:11.000000 jms-metabolite-services-0.5.4/jms/utils/hmdb.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:21.000000 jms-metabolite-services-0.5.4/jms/utils/pubchem.py
+-rw-r--r--   0 shuzhao    (501) staff       (20)        0 2022-02-10 00:48:26.000000 jms-metabolite-services-0.5.4/jms/utils/refmet.py
+drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/
+-rw-r--r--   0 shuzhao    (501) staff       (20)     5597 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/PKG-INFO
+-rw-r--r--   0 shuzhao    (501) staff       (20)      666 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/SOURCES.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        1 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/dependency_links.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)       10 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/requires.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)        4 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/top_level.txt
+-rw-r--r--   0 shuzhao    (501) staff       (20)       38 2023-04-09 12:04:54.000000 jms-metabolite-services-0.5.4/setup.cfg
+-rw-r--r--   0 shuzhao    (501) staff       (20)     1300 2022-05-19 20:56:08.000000 jms-metabolite-services-0.5.4/setup.py
```

### Comparing `jms-metabolite-services-0.5.3/LICENSE` & `jms-metabolite-services-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/PKG-INFO` & `jms-metabolite-services-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jms-metabolite-services
-Version: 0.5.3
+Version: 0.5.4
 Summary: conversion, search of metabolic models and metabolomics data
 Home-page: https://github.com/shuzhao-li/JMS
 Author: Shuzhao Li, Minghao Gong
 Author-email: shuzhao.li@gmail.com
 License: Python
 Keywords: metabolomics,chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jms-metabolite-services-0.5.3/README.md` & `jms-metabolite-services-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/coverage.py` & `jms-metabolite-services-0.5.4/jms/coverage.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/data/list_formula_mass.py` & `jms-metabolite-services-0.5.4/jms/data/list_formula_mass.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/dbStructures.py` & `jms-metabolite-services-0.5.4/jms/dbStructures.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/empiricalCpds.py` & `jms-metabolite-services-0.5.4/jms/empiricalCpds.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/formula.py` & `jms-metabolite-services-0.5.4/jms/formula.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/io.py` & `jms-metabolite-services-0.5.4/jms/io.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/ions.py` & `jms-metabolite-services-0.5.4/jms/ions.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/modelConvert.py` & `jms-metabolite-services-0.5.4/jms/modelConvert.py`

 * *Files 14% similar despite different names*

```diff
@@ -202,25 +202,89 @@
         Match model compounds with empirical compounds, via the JMS KCD-EED architecture.
         The search here cannot distinguish isomers, thus centering on neutral mass/formula.
 
         Returns
         -------
         dict_empCpds : {id: empCpd, ...} with matched compounds in empCpd['list_matches'],
             which have KCD empCpd identifiers but compound records need to pull out KCD later.
+            This dict includes singletons and empCpds without matches.
+
+        Examples
+        --------
+        A intermediary EED.dict_empCpds before updating identity: 
+        {'interim_id': 'kp203_202.1317', 
+            'neutral_formula_mass': 202.13169603323, 'neutral_formula': None, 
+            'Database_referred': [], 'identity': [], 
+            'MS1_pseudo_Spectra': [{'id_number': 'F3900', 'mz': 204.1424, 'rtime': 23.04, 'rtime_left_base': '21.88', 
+                    'rtime_right_base': '25.37', 'parent_masstrack_id': '2519', 'peak_area': '111965925', 'cSelectivity': '0.86', 
+                    'goodness_fitting': '0.98', 'snr': '6675', 'detection_counts': '15', ' 'apex': 23.04, 
+                    'representative_intensity': '111965925', 'id': 'F3900', 
+                    'isotope': '13C/12C', 'modification': 'M+H+', 'ion_relation': '13C/12C,M+H+', 'parent_epd_id': 'kp203_202.1317'}, 
+            {'id_number': 'F3684', 'mz': 203.1389, 'rtime': 23.04, 'rtime_left_base': '21.88', 'rtime_right_base': '25.37', 
+                    'parent_masstrack_id': '2495', 'peak_area': '402792917', 'cSelectivity': '0.86', 'goodness_fitting': '0.98', 
+                    'snr': '120', 'detection_counts': '15',  'apex': 23.04, 'representative_intensity': '402792917', 
+                    'id': 'F3684', 'isotope': 'M0', 'modification': 'M+H+', 'ion_relation': 'M0,M+H+', 'parent_epd_id': 'kp203_202.1317'}], 
+            'MS2_Spectra': [], 
+            'list_matches': [('C9H18N2O3_202.131742', 'neutral', 1)]}
+
+        An indexed KCD empCpd, KCD.mass_indexed_compounds['C9H18N2O3_202.131742']:
+        {'interim_id': 'C9H18N2O3_202.131742',
+            'neutral_formula': 'C9H18N2O3',
+            'neutral_formula_mass': 202.13174244717,
+            'compounds': [{'id': 'MAM03375',
+            'name': 'L-Alanyl-L-Leucine',
+            'identifiers': [['humanGEM', 'MAM03375'],
+                ['bigg.metabolite', 'CE5866'],
+                ['pubchem.compound', '6992388'],
+                ['vmhmetabolite', 'CE5866'],
+                ['metanetx.chemical', 'MNXM15786'],
+                ['inchi',
+                'InChI=1S/C9H18N2O3/c1-5(2)4-7(9(13)14)11-8(12)6(3)10/h5-7H,4,10H2,1-3H3,(H,11,12)(H,13,14)/t6-,7+/m1/s1']],
+            'neutral_formula': 'C9H18N2O3',
+            'charge': 0,
+            'charged_formula': 'C9H18N2O3',
+            'neutral_mono_mass': 202.13174244717,
+            'SMILES': '',
+            'inchi': '',
+            'neutral_formula_mass': 202.13174244717}]}
         '''
         KCD = knownCompoundDatabase()
-        KCD.mass_index_list_compounds(self.model['Compounds'])
+        KCD.mass_index_list_compounds(self.model['Compounds'].values())
         KCD.build_emp_cpds_index()
         EED = ExperimentalEcpdDatabase(mode=self.mode, 
                                        mz_tolerance_ppm=self.mz_tolerance_ppm, 
                                        rt_tolerance=self.rt_tolerance)
         EED.build_from_list_peaks(self.userFeatureList)
         EED.extend_empCpd_annotation(KCD)
-        EED.annotate_singleton_mummichog(KCD)       
-        return EED.dict_empCpds
+        EED.annotate_singleton_mummichog(KCD)
+
+        return self.update_identity(EED.dict_empCpds, KCD)
+
+
+    def update_identity(self, dict_empCpds, KCD):
+        '''
+        Updates dict_empCpds by adding field `identity` with compound IDs.
+        E.g. {'identity': ['MAM03375'], ... }
+        This overwrites field `identity` if it exists.
+        '''
+        def _get_kcd_ids_(interim_id, KCD):
+            e = KCD.mass_indexed_compounds.get(interim_id, None)
+            if e:
+                return [x['id'] for x in e['compounds']]
+            else:
+                return []
+
+        for k,v in dict_empCpds.items():
+            if 'list_matches' in v:
+                v['identity'] = []
+                for M in v['list_matches']:
+                    v['identity'] += _get_kcd_ids_(M[0], KCD)
+
+        return dict_empCpds
+
 
     def _construct_EmpiricalCompounds_(self):
         '''
         For testing only. Use EED class for full application, as in self.match_all().
         Returns
         -------
         dict_empCpds : {id: empCpd, ...}
```

### Comparing `jms-metabolite-services-0.5.3/jms/search.py` & `jms-metabolite-services-0.5.4/jms/search.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/test.py` & `jms-metabolite-services-0.5.4/jms/test.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/utils/Tabular2Json.py` & `jms-metabolite-services-0.5.4/jms/utils/Tabular2Json.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/utils/gems.py` & `jms-metabolite-services-0.5.4/jms/utils/gems.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms/utils/hmdb.py` & `jms-metabolite-services-0.5.4/jms/utils/hmdb.py`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/PKG-INFO` & `jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jms-metabolite-services
-Version: 0.5.3
+Version: 0.5.4
 Summary: conversion, search of metabolic models and metabolomics data
 Home-page: https://github.com/shuzhao-li/JMS
 Author: Shuzhao Li, Minghao Gong
 Author-email: shuzhao.li@gmail.com
 License: Python
 Keywords: metabolomics,chemistry,bioinformatics,mass spectrometry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jms-metabolite-services-0.5.3/jms_metabolite_services.egg-info/SOURCES.txt` & `jms-metabolite-services-0.5.4/jms_metabolite_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jms-metabolite-services-0.5.3/setup.py` & `jms-metabolite-services-0.5.4/setup.py`

 * *Files identical despite different names*

