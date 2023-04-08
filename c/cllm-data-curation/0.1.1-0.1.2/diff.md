# Comparing `tmp/cllm-data-curation-0.1.1.tar.gz` & `tmp/cllm-data-curation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cllm-data-curation-0.1.1.tar", last modified: Sat Apr  8 20:55:59 2023, max compression
+gzip compressed data, was "cllm-data-curation-0.1.2.tar", last modified: Sat Apr  8 23:49:13 2023, max compression
```

## Comparing `cllm-data-curation-0.1.1.tar` & `cllm-data-curation-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.891193 cllm-data-curation-0.1.1/
--rw-r--r--   0 darienschettler   (501) staff       (20)      816 2023-04-08 20:55:59.891095 cllm-data-curation-0.1.1/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      176 2023-03-27 19:27:04.000000 cllm-data-curation-0.1.1/README.md
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.889036 cllm-data-curation-0.1.1/cllm_data_curation/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-27 18:56:48.000000 cllm-data-curation-0.1.1/cllm_data_curation/__init__.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.890230 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-22 21:31:03.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2023 2023-03-23 16:08:20.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/multiprocessing_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)      744 2023-03-29 23:32:35.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/other_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     1768 2023-03-28 17:42:00.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/parallel_dl.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     3284 2023-03-28 17:40:35.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/preprocessing_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     7872 2023-03-28 17:40:35.000000 cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/processing_utils.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.890922 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/
--rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-27 18:57:34.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/__init__.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2736 2023-03-28 16:55:45.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/curation_configs.py
--rw-r--r--   0 darienschettler   (501) staff       (20)    16183 2023-04-08 20:54:00.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/curation_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     4123 2023-03-27 22:03:56.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/download.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     6188 2023-03-27 22:00:32.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/download_utils.py
--rw-r--r--   0 darienschettler   (501) staff       (20)     2492 2023-03-27 21:22:03.000000 cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/general_utils.py
-drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 20:55:59.889552 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/
--rw-r--r--   0 darienschettler   (501) staff       (20)      816 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/PKG-INFO
--rw-r--r--   0 darienschettler   (501) staff       (20)      873 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/SOURCES.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/dependency_links.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       86 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/requires.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-08 20:55:59.000000 cllm-data-curation-0.1.1/cllm_data_curation.egg-info/top_level.txt
--rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-08 20:55:59.891229 cllm-data-curation-0.1.1/setup.cfg
--rw-r--r--   0 darienschettler   (501) staff       (20)     1110 2023-04-08 20:55:09.000000 cllm-data-curation-0.1.1/setup.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 23:49:13.100194 cllm-data-curation-0.1.2/
+-rw-r--r--   0 darienschettler   (501) staff       (20)      816 2023-04-08 23:49:13.100079 cllm-data-curation-0.1.2/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      176 2023-03-27 19:27:04.000000 cllm-data-curation-0.1.2/README.md
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 23:49:13.096438 cllm-data-curation-0.1.2/cllm_data_curation/
+-rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-27 18:56:48.000000 cllm-data-curation-0.1.2/cllm_data_curation/__init__.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 23:49:13.098353 cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/
+-rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-22 21:31:03.000000 cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2023 2023-03-23 16:08:20.000000 cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/multiprocessing_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)      744 2023-03-29 23:32:35.000000 cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/other_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1768 2023-03-28 17:42:00.000000 cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/parallel_dl.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     3284 2023-03-28 17:40:35.000000 cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/preprocessing_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     7872 2023-03-28 17:40:35.000000 cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/processing_utils.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 23:49:13.099729 cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/
+-rw-r--r--   0 darienschettler   (501) staff       (20)        0 2023-03-27 18:57:34.000000 cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/__init__.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2736 2023-03-28 16:55:45.000000 cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/curation_configs.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)    16656 2023-04-08 23:48:18.000000 cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/curation_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     4123 2023-03-27 22:03:56.000000 cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/download.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     6188 2023-03-27 22:00:32.000000 cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/download_utils.py
+-rw-r--r--   0 darienschettler   (501) staff       (20)     2492 2023-03-27 21:22:03.000000 cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/general_utils.py
+drwxr-xr-x   0 darienschettler   (501) staff       (20)        0 2023-04-08 23:49:13.097126 cllm-data-curation-0.1.2/cllm_data_curation.egg-info/
+-rw-r--r--   0 darienschettler   (501) staff       (20)      816 2023-04-08 23:49:13.000000 cllm-data-curation-0.1.2/cllm_data_curation.egg-info/PKG-INFO
+-rw-r--r--   0 darienschettler   (501) staff       (20)      873 2023-04-08 23:49:13.000000 cllm-data-curation-0.1.2/cllm_data_curation.egg-info/SOURCES.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)        1 2023-04-08 23:49:13.000000 cllm-data-curation-0.1.2/cllm_data_curation.egg-info/dependency_links.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       86 2023-04-08 23:49:13.000000 cllm-data-curation-0.1.2/cllm_data_curation.egg-info/requires.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       19 2023-04-08 23:49:13.000000 cllm-data-curation-0.1.2/cllm_data_curation.egg-info/top_level.txt
+-rw-r--r--   0 darienschettler   (501) staff       (20)       38 2023-04-08 23:49:13.100232 cllm-data-curation-0.1.2/setup.cfg
+-rw-r--r--   0 darienschettler   (501) staff       (20)     1110 2023-04-08 23:49:08.000000 cllm-data-curation-0.1.2/setup.py
```

### Comparing `cllm-data-curation-0.1.1/PKG-INFO` & `cllm-data-curation-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cllm-data-curation
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to visualize tokenization of text using HTML
 Home-page: https://github.com/ds08tf/cllm-data-curation
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cllm-data-curation Version: 0.1.1 Summary: A
+Metadata-Version: 2.1 Name: cllm-data-curation Version: 0.1.2 Summary: A
 package to visualize tokenization of text using HTML Home-page: https://
 github.com/ds08tf/cllm-data-curation Author: Darien Schettler Author-email:
 ds08tf@gmail.com Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.7
```

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/multiprocessing_utils.py` & `cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/other_utils.py` & `cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/other_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/parallel_dl.py` & `cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/parallel_dl.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/preprocessing_utils.py` & `cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/parallel_dl/processing_utils.py` & `cllm-data-curation-0.1.2/cllm_data_curation/parallel_dl/processing_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/curation_configs.py` & `cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/curation_configs.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/curation_utils.py` & `cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/curation_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,45 +58,53 @@
         meta_df = meta_df[meta_df.lang_size_mb > mb_size_thresh]
     elif pq_file_cnt_thresh:
         meta_df = meta_df[meta_df.lang_file_cnt >= pq_file_cnt_thresh]
     return meta_df[~meta_df.lang.isin(bad_langs)].reset_index(drop=True)
 
 
 def filter_parquet_file(pq_path, output_dir,
-                        max_ll=600, min_len=50, min_max_ll=25, max_size_kbs=1_000, keep_original_index=True,
-                        min_alphanum=0.001, max_alphanum=0.975, min_ave_ll=16, min_lines=3, is_slim=True, **kwargs):
+                        max_ll=600, min_len=50, min_max_ll=25, max_size_kbs=1_000, keep_original_index=False,
+                        check_python2=True, min_alphanum=0.001, max_alphanum=0.975, min_ave_ll=16, min_lines=3,
+                        is_slim=True, **kwargs):
     """Filter a Parquet file by applying multiple criteria such as line length, file size,
     number of lines, and alphanumerical fraction.
 
     Args:
         pq_path (str): Path to the input Parquet file.
             - NOTE: This is expected to be in the form: .../<root_dir>/<lang>/<pq_file_name>.pq
         output_dir (str): Directory to save the filtered Parquet file.
         max_ll (int, optional): Maximum allowed line length. Defaults to 600.
         min_len (int, optional): Minimum allowed file size. Defaults to 50.
         min_max_ll (int, optional): Minimum allowed maximum line length. Defaults to 25.
         max_size_kbs (int, optional): Maximum allowed file size in kilobytes. Defaults to 1000.
         keep_original_index (bool, optional): Whether to keep the original index. Defaults to True.
+        check_python2 (bool, optional): Whether to check for Python 2 compatibility. Defaults to True.
         min_alphanum (float, optional): Minimum allowed alphanumerical fraction. Defaults to 0.001.
         max_alphanum (float, optional): Maximum allowed alphanumerical fraction. Defaults to 0.975.
         min_ave_ll (int, optional): Minimum allowed average line length. Defaults to 16.
         min_lines (int, optional): Minimum allowed number of lines. Defaults to 3.
         is_slim (bool, optional): Whether to apply slim filtering or not. Defaults to True.
 
     Returns:
         str: Path to the filtered Parquet file.
     """
     print(f"\nWORKING ON {pq_path} ...")
 
     # Step 0: Identify input directory and create destination directory (if necessary)
     _root_path, _origin_root_dir, _lang, _fname = pq_path.rsplit("/", 3)
     _dest_dir = os.path.join(output_dir, _lang)
-    _dest_path = pq_path.replace(_origin_root_dir, output_dir.rsplit("/", 1)[-1])
-    if not os.path.isdir(_dest_dir):
-        os.makedirs(_dest_dir, exist_ok=True)
+    _reject_dir = os.path.join(_dest_dir, "rejects")
+    _reject_path = os.path.join(_reject_dir, _fname)
+    _dest_path = os.path.join(_dest_dir, _fname)
+    # _dest_path = pq_path.replace(_origin_root_dir, output_dir.rsplit("/", 1)[-1])
+
+    if not os.path.isdir(_reject_dir):
+        os.makedirs(_reject_dir, exist_ok=True)
+        if not os.path.isdir(_dest_dir):
+            os.makedirs(_dest_dir, exist_ok=True)
 
     # Step 1: Load the DataFrame from the Parquet file (slim if necessary)
     _df = open_pq_as_df(pq_path, is_slim=is_slim)
     print(f"\t--> ORIGINAL LENGTH: {len(_df)}")
 
     # Step 2: Filter out rows/files with maximum line lengths outside the required range
     filter_flag = ((_df.max_ll <= max_ll) & (_df.max_ll >= min_max_ll))
@@ -136,28 +144,29 @@
     # Step 7: Filter out rows/files with fewer than `min_lines` lines
     filter_flag = (_df.file_size / _df.ave_ll) >= min_lines
     reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
     reject_df.loc[:, "reason"] = reject_df["reason"].fillna("min_lines")
     _df = _df[filter_flag]
     print(f"\t--> AFTER MIN NUMBER OF LINES REDUCTION: {len(_df)}")
 
-    # Step 8: Filter out rows/files written in Python 2
-    filter_flag = _df.content.apply(test_source_code_compatible)
-    reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
-    reject_df.loc[:, "reason"] = reject_df["reason"].fillna("python2")
-    _df = _df[filter_flag]
-    print(f"\t--> AFTER PYTHON 2 DETECTION REDUCTION: {len(_df)}")
+    # Step 8: Filter out rows/files written in Python 2 (OPTIONAL - TIME CONSUMING)
+    if check_python2:
+        filter_flag = _df.content.apply(test_source_code_compatible)
+        reject_df = pd.concat((reject_df, _df[~filter_flag].copy()))
+        reject_df.loc[:, "reason"] = reject_df["reason"].fillna("python2")
+        _df = _df[filter_flag]
+        print(f"\t--> AFTER PYTHON 2 DETECTION REDUCTION: {len(_df)}")
 
     # Step 9: Save the filtered DataFrame to a Parquet file
     print(f"\t--> SAVING ...\n\t--> `{_dest_path}` ...\n")
     _df.to_parquet(_dest_path, index=keep_original_index)
 
     # Step 9.5: Save the rejection DataFrame to a Parquet file
     reject_df = reject_df.sort_index()  # sort to reorder according to the original ordering
-    reject_df.to_parquet(_dest_path.replace(".parquet", "_rejects.parquet"), index=keep_original_index)
+    reject_df.to_parquet(_reject_path.replace(".parquet", "_rejects.parquet"), index=keep_original_index)
 
     # Step 10: Return the path to the filtered Parquet file
     return _dest_path
 
 
 def open_pq_as_df(pq_path, is_slim=False):
     """Open a Parquet file as a Pandas DataFrame.
```

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/download.py` & `cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/download.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/download_utils.py` & `cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/download_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation/thestack_curation/general_utils.py` & `cllm-data-curation-0.1.2/cllm_data_curation/thestack_curation/general_utils.py`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation.egg-info/PKG-INFO` & `cllm-data-curation-0.1.2/cllm_data_curation.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cllm-data-curation
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to visualize tokenization of text using HTML
 Home-page: https://github.com/ds08tf/cllm-data-curation
 Author: Darien Schettler
 Author-email: ds08tf@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cllm-data-curation Version: 0.1.1 Summary: A
+Metadata-Version: 2.1 Name: cllm-data-curation Version: 0.1.2 Summary: A
 package to visualize tokenization of text using HTML Home-page: https://
 github.com/ds08tf/cllm-data-curation Author: Darien Schettler Author-email:
 ds08tf@gmail.com Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Requires-Python: >=3.7
```

### Comparing `cllm-data-curation-0.1.1/cllm_data_curation.egg-info/SOURCES.txt` & `cllm-data-curation-0.1.2/cllm_data_curation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cllm-data-curation-0.1.1/setup.py` & `cllm-data-curation-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cllm-data-curation",
-    version="0.1.1",
+    version="0.1.2",
     author="Darien Schettler",
     author_email="ds08tf@gmail.com",
     description="A package to visualize tokenization of text using HTML",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ds08tf/cllm-data-curation",
     packages=find_packages(),
```

