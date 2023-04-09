# Comparing `tmp/heartfelt_tools-0.9.0.tar.gz` & `tmp/heartfelt_tools-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartfelt_tools-0.9.0.tar", max compression
+gzip compressed data, was "heartfelt_tools-1.7.0.tar", max compression
```

## Comparing `heartfelt_tools-0.9.0.tar` & `heartfelt_tools-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2022-10-21 01:09:12.000000 heartfelt_tools-0.9.0/LICENSE
--rw-r--r--   0        0        0     7303 2023-02-09 01:30:00.000000 heartfelt_tools-0.9.0/README.md
--rw-r--r--   0        0        0        0 2023-02-12 21:09:30.000000 heartfelt_tools-0.9.0/database_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 20:53:23.596958 heartfelt_tools-0.9.0/database_tools/datastores/__init__.py
--rw-r--r--   0        0        0      938 2023-04-07 19:00:09.619442 heartfelt_tools-0.9.0/database_tools/datastores/records.py
--rw-r--r--   0        0        0     2520 2023-04-07 18:53:23.861591 heartfelt_tools-0.9.0/database_tools/datastores/signals.py
--rw-r--r--   0        0        0        0 2023-04-05 20:53:23.596958 heartfelt_tools-0.9.0/database_tools/errors.py
--rw-r--r--   0        0        0        0 2023-04-05 20:53:23.596958 heartfelt_tools-0.9.0/database_tools/io/__init__.py
--rw-r--r--   0        0        0      470 2023-04-07 17:47:29.796060 heartfelt_tools-0.9.0/database_tools/io/data.py
--rw-r--r--   0        0        0      224 2023-04-07 17:58:25.968297 heartfelt_tools-0.9.0/database_tools/io/utils.py
--rw-r--r--   0        0        0     7001 2023-04-07 20:08:43.428482 heartfelt_tools-0.9.0/database_tools/io/wfdb.py
--rw-r--r--   0        0        0        0 2023-02-09 01:25:56.000000 heartfelt_tools-0.9.0/database_tools/processing/__init__.py
--rw-r--r--   0        0        0     1228 2023-04-05 20:48:44.315318 heartfelt_tools-0.9.0/database_tools/processing/cardiac.py
--rw-r--r--   0        0        0     2721 2023-04-07 19:06:50.432508 heartfelt_tools-0.9.0/database_tools/processing/detect.py
--rw-r--r--   0        0        0     4765 2023-04-07 19:04:56.823116 heartfelt_tools-0.9.0/database_tools/processing/metrics.py
--rw-r--r--   0        0        0     1859 2023-04-07 20:26:24.799112 heartfelt_tools-0.9.0/database_tools/processing/modify.py
--rw-r--r--   0        0        0     5038 2023-04-07 20:26:09.535953 heartfelt_tools-0.9.0/database_tools/processing/utils.py
--rw-r--r--   0        0        0    10403 2023-04-05 21:19:59.194064 heartfelt_tools-0.9.0/database_tools/tools/DataEvaluator.py
--rw-r--r--   0        0        0     3080 2023-02-09 01:25:56.000000 heartfelt_tools-0.9.0/database_tools/tools/DataLocator.py
--rw-r--r--   0        0        0       82 2023-04-07 20:11:00.337873 heartfelt_tools-0.9.0/database_tools/tools/__init__.py
--rw-r--r--   0        0        0    12276 2023-04-07 21:42:30.599494 heartfelt_tools-0.9.0/database_tools/tools/dataset.py
--rw-r--r--   0        0        0     6884 2023-04-07 20:11:10.345976 heartfelt_tools-0.9.0/database_tools/tools/records.py
--rw-r--r--   0        0        0      953 2023-04-07 21:42:52.932048 heartfelt_tools-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8623 1970-01-01 00:00:00.000000 heartfelt_tools-0.9.0/setup.py
--rw-r--r--   0        0        0     8342 1970-01-01 00:00:00.000000 heartfelt_tools-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-21 01:09:12.000000 heartfelt_tools-1.7.0/LICENSE
+-rw-r--r--   0        0        0     7303 2023-02-09 01:30:00.000000 heartfelt_tools-1.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-12 21:09:30.000000 heartfelt_tools-1.7.0/database_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/datastores/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/datastores/records.py
+-rw-r--r--   0        0        0     2520 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/datastores/signals.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/errors.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/io/__init__.py
+-rw-r--r--   0        0        0      470 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/io/data.py
+-rw-r--r--   0        0        0      224 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/io/utils.py
+-rw-r--r--   0        0        0     6945 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/io/wfdb.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/__init__.py
+-rw-r--r--   0        0        0     1228 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/cardiac.py
+-rw-r--r--   0        0        0     2811 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/detect.py
+-rw-r--r--   0        0        0     4765 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/metrics.py
+-rw-r--r--   0        0        0     1859 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/modify.py
+-rw-r--r--   0        0        0     5175 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/processing/utils.py
+-rw-r--r--   0        0        0    10403 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/tools/DataEvaluator.py
+-rw-r--r--   0        0        0     3080 2023-02-09 01:25:56.000000 heartfelt_tools-1.7.0/database_tools/tools/DataLocator.py
+-rw-r--r--   0        0        0       82 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/tools/__init__.py
+-rw-r--r--   0        0        0    12151 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/tools/dataset.py
+-rw-r--r--   0        0        0     6884 2023-04-09 21:23:36.811381 heartfelt_tools-1.7.0/database_tools/tools/records.py
+-rw-r--r--   0        0        0      953 2023-04-09 21:24:33.784095 heartfelt_tools-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8623 1970-01-01 00:00:00.000000 heartfelt_tools-1.7.0/setup.py
+-rw-r--r--   0        0        0     8342 1970-01-01 00:00:00.000000 heartfelt_tools-1.7.0/PKG-INFO
```

### Comparing `heartfelt_tools-0.9.0/LICENSE` & `heartfelt_tools-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/README.md` & `heartfelt_tools-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/datastores/records.py` & `heartfelt_tools-1.7.0/database_tools/datastores/records.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/datastores/signals.py` & `heartfelt_tools-1.7.0/database_tools/datastores/signals.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/io/wfdb.py` & `heartfelt_tools-1.7.0/database_tools/io/wfdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 import logging
 import requests
 import numpy as np
 import pandas as pd
 from typing import Union, List
 from alive_progress import alive_bar
 
-log_dir = '/'.join(os.getcwd().split('/')[0:5]) + '/logs/'
 logging.basicConfig(
-     filename=f'{log_dir}io.log',
+     filename=f'{__name__}.log',
      format= '[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s',
      datefmt='%H:%M:%S'
 )
-logger = logging.getLogger('io')
+logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 MIMIC_DIR = 'mimic3wdb/1.0/'
 
 def generate_record_paths(name: str = None, shuffle: bool = True) -> str:
     if name is None:
         rec_dir = MIMIC_DIR + 'RECORDS'
```

### Comparing `heartfelt_tools-0.9.0/database_tools/processing/cardiac.py` & `heartfelt_tools-1.7.0/database_tools/processing/cardiac.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/processing/detect.py` & `heartfelt_tools-1.7.0/database_tools/processing/detect.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,25 @@
 def detect_peaks(sig, show=False, **kwargs):
     """Modified version of neuroki2 ppg_findpeaks method. Returns peaks and troughs
        instead of just peaks. See neurokit2 documentation for original function.
     """
     peaks, troughs = _ppg_findpeaks_bishop(sig, show=show, **kwargs)
     return dict(peaks=peaks[0], troughs=troughs[0])
 
-def detect_notches(sig: np.ndarray, peaks: np.ndarray, troughs: np.ndarray, dx: int = 10, thresh=10) -> list:
+def detect_notches(sig: np.ndarray, peaks: np.ndarray, troughs: np.ndarray, dx: int = 10, thresh: int = 10) -> list:
     """Detect dichrotic notch by find the maximum velocity
        at least 10 samples after peak and 30 samples before
        the subsequent trough.
 
     Args:
         sig (np.ndarray): Cardiac signal.
         peaks (list): List of signal peak indices.
         troughs (list): List of signal trough indices.
         dx (int, optional): Spacing between sig values (for np.gradient). Defaults to 10.
+        thresh (int, optional): Minimum distance between peak and subsequent notch.
 
     Returns:
         notches (list): List of dichrotic notch indices.
     """
     # always start with first peak
     try:
         if peaks[0] > troughs[0]:
@@ -44,15 +45,15 @@
         return []
 
     notches = []
     for i, j in zip(peaks, troughs):
         try:
             vel = np.gradient(sig[i:j], dx)
             vel_len = vel.shape[0]
-            n = np.argmax(vel[int(vel_len / 100 * 25):int(vel_len / 100 * 75)])
+            n = np.argmax(vel[int(vel_len / 100 * 10):int(vel_len / 100 * 90)])
             notches.append(n + i)  # add first index of slice to get correct notch index
         except ValueError:  # gradient fails if slice of sig is too small
             continue
 
     # look for a notch after the last peak if the highest index is a peak.
     try:
         if peaks[-1] > troughs[-1]:
@@ -64,11 +65,11 @@
             except ValueError:
                 pass
     except IndexError:
         pass
 
     # remove notches that are closer than thresh distance in samples
     a, b = np.meshgrid(notches, peaks)
-    peak_notch_distances = np.abs(b - a)
-    valid_notch_idx = np.array(np.where(peak_notch_distances >= thresh))[1, :]  # get index in notch array
+    notch_to_peak_distances = np.abs(b - a).transpose()
+    valid_notch_idx = [i for i, x in enumerate(notch_to_peak_distances) if x[i] >= thresh]
     notches = np.array(notches)[valid_notch_idx]
     return notches
```

### Comparing `heartfelt_tools-0.9.0/database_tools/processing/metrics.py` & `heartfelt_tools-1.7.0/database_tools/processing/metrics.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/processing/modify.py` & `heartfelt_tools-1.7.0/database_tools/processing/modify.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/processing/utils.py` & `heartfelt_tools-1.7.0/database_tools/processing/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,14 +138,18 @@
                     i_first += 1
             else: # inverse of other else condition
                 i_second += 1
         except IndexError: # catch index error (always thrown in last iteration)
             first_repaired.append(poi_1)
             second_repaired.append(poi_2)
 
+    # remove duplicates
+    first_repaired = sorted(list(set(first_repaired)))
+    second_repaired = sorted(list(set(second_repaired)))
+
     # place indices in the correct order
     try:
         if peaks[0] < troughs[0]:
             return (np.array(first_repaired), np.array(second_repaired))
         else:
             return (np.array(second_repaired), np.array(first_repaired))
     except IndexError:
```

### Comparing `heartfelt_tools-0.9.0/database_tools/tools/DataEvaluator.py` & `heartfelt_tools-1.7.0/database_tools/tools/DataEvaluator.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/tools/DataLocator.py` & `heartfelt_tools-1.7.0/database_tools/tools/DataLocator.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/database_tools/tools/dataset.py` & `heartfelt_tools-1.7.0/database_tools/tools/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import ast
 import configparser
 import glob
 import json
-import logging
-import os
 import random
 from dataclasses import InitVar, dataclass, field
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
 from alive_progress import alive_bar
@@ -18,25 +16,14 @@
 from database_tools.processing.detect import (detect_flat_lines,
                                               detect_notches, detect_peaks)
 from database_tools.processing.metrics import (get_beat_similarity,
                                                get_similarity, get_snr)
 from database_tools.processing.modify import align_signals, bandpass
 from database_tools.processing.utils import repair_peaks_troughs_idx, window
 
-log_dir = '/'.join(os.getcwd().split('/')[0:5]) + '/logs/'
-if 'database_tools' in log_dir:
-    logging.basicConfig(
-        filename=f'{log_dir}tools.log',
-        format= '[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s',
-        datefmt='%H:%M:%S'
-    )
-    logger = logging.getLogger('tools')
-    logger.setLevel(logging.INFO)
-
-
 @dataclass(frozen=True)
 class ConfigItem:
     def set_attr(self, config_item):
         for key, value in config_item.items():
             try:
                 object.__setattr__(self, key, ast.literal_eval(value))
             except:
@@ -71,19 +58,19 @@
     valid_samples: int = 0
     rejected_samples: int = 0
     patient_samples: int = 0
     prev_patient: str = ''
 
     def __post_init__(self, cm: list):
         self.metrics_dict = {}
-        for m in cm.metrics:
+        for m in cm.data.metrics:
             self.metrics_dict.update({m: []})
-        self.samples_per_file = cm.samples_per_file
-        self.samples_per_patient = cm.samples_per_patient
-        self.max_samples = cm.max_samples
+        self.samples_per_file = cm.data.samples_per_file
+        self.samples_per_patient = cm.data.samples_per_patient
+        self.max_samples = cm.data.max_samples
 
     def update_metrics(self, metrics: dict) -> None:
         """Update dataset metrics dictionary and return next action.
            0 -> Continue
            1 -> Write data to file and continue.
            2 -> Write remaining data and stop.
 
@@ -141,74 +128,76 @@
         object.__setattr__(self, 'vpg', vpg)
         object.__setattr__(self, 'apg', apg)
         object.__setattr__(self, 'abp', np.array(data['abp'].to_list()))
         self.info
 
     @property
     def info(self):
-        logger.info(f'Data was extracted from {self._nframes} JSONLINES files.')
-        logger.info(f'The total number of windows is {self.ppg.shape[0]}.')
+        print(f'Data was extracted from {self._nframes} JSONLINES files.')
+        print(f'The total number of windows is {self.ppg.shape[0]}.')
 
 
 @dataclass
 class Window:
 
     sig: np.ndarray
     cm: ConfigMapper
     checks: List[str]
 
     @property
     def _snr_check(self) -> bool:
-        self.snr, self.f0 = get_snr(self.sig, low=self.cm.freq_band[0], high=self.cm.freq_band[1], df=0.2, fs=self.cm.fs)
-        return self.snr > self.cm.snr
+        self.snr, self.f0 = get_snr(self.sig, low=self.cm.data.freq_band[0], high=self.cm.data.freq_band[1], df=0.2, fs=self.cm.data.fs)
+        return self.snr > self.cm.data.snr
 
     @property
     def _hr_check(self) -> bool:
-        return (self.f0 > self.cm.hr_freq_band[0]) & (self.f0 < self.cm.hr_freq_band[1])
+        return (self.f0 > self.cm.data.hr_freq_band[0]) & (self.f0 < self.cm.data.hr_freq_band[1])
 
     @property
     def _flat_check(self) -> bool:
-        return not detect_flat_lines(self.sig, n=self.cm.flat_line_length)
+        return not detect_flat_lines(self.sig, n=self.cm.data.flat_line_length)
 
     @property
     def _beat_check(self) -> bool:
         self.beat_sim = get_beat_similarity(
             self.sig,
             troughs=self.troughs,
-            fs=self.cm.fs,
+            fs=self.cm.data.fs,
         )
-        return self.beat_sim > self.cm.beat_sim
+        return self.beat_sim > self.cm.data.beat_sim
 
     @property
     def _notch_check(self) -> bool:
         notches = detect_notches(
             self.sig,
             peaks=self.peaks,
             troughs=self.troughs,
         )
-        return len(notches) > self.cm.min_notches
+        return len(notches) > self.cm.data.min_notches
 
     @property
     def _bp_check(self) -> bool:
         self.dbp, self.sbp = np.min(self.sig), np.max(self.sig)
-        dbp_check = (self.dbp > self.cm.dbp_bounds[0]) & (self.dbp < self.cm.dbp_bounds[1])
-        sbp_check = (self.sbp > self.cm.sbp_bounds[0]) & (self.sbp < self.cm.sbp_bounds[1])
+        dbp_check = (self.dbp > self.cm.data.dbp_bounds[0]) & (self.dbp < self.cm.data.dbp_bounds[1])
+        sbp_check = (self.sbp > self.cm.data.sbp_bounds[0]) & (self.sbp < self.cm.data.sbp_bounds[1])
         return dbp_check & sbp_check
 
     @property
     def valid(self) -> bool:
         v = [object.__getattribute__(self, '_' + c + '_check') for c in self.checks]
         return np.array(v).all()
 
     def get_peaks(self, pad_width=40) -> None:
         x_pad = np.pad(self.sig, pad_width=pad_width, constant_values=np.mean(self.sig))
         peaks, troughs = detect_peaks(x_pad).values()
         peaks, troughs = repair_peaks_troughs_idx(peaks, troughs)
-        self.peaks = peaks - pad_width - 1
-        self.troughs = troughs - pad_width - 1
+        peaks = peaks - pad_width - 1
+        self.peaks = [p for p in peaks if p > -1]
+        troughs = troughs - pad_width - 1
+        self.troughs = [t for t in troughs if t > -1]
 
 
 def congruency_check(ppg: Window, abp: Window, cm: ConfigMapper) -> Tuple[float, float, bool]:
     """Performs checks between ppg and abp Window objects.
 
     Args:
         ppg (Window): Object with ppg data.
@@ -216,18 +205,18 @@
         cm (ConfigMapper): Config mapping dataclass.
 
     Returns:
         bool: True if valid, False if not.
     """
     time_sim = get_similarity(ppg.sig, abp.sig)
     ppg_f = np.abs(np.fft.fft(ppg.sig))
-    abp_f = np.abs(np.fft.fft(bandpass(abp.sig, low=cm.freq_band[0], high=cm.freq_band[1], fs=cm.fs)))
+    abp_f = np.abs(np.fft.fft(bandpass(abp.sig, low=cm.data.freq_band[0], high=cm.data.freq_band[1], fs=cm.data.fs)))
     spec_sim = get_similarity(ppg_f, abp_f)
-    sim_check = (time_sim > cm.sim) & (spec_sim > cm.sim)
-    hr_delta_check = np.abs(ppg.f0 - abp.f0) < cm.hr_delta
+    sim_check = (time_sim > cm.data.sim) & (spec_sim > cm.data.sim)
+    hr_delta_check = np.abs(ppg.f0 - abp.f0) < cm.data.hr_delta
     congruency_check = sim_check & hr_delta_check
     return {
         'time_sim': time_sim,
         'spec_sim': spec_sim,
         'cong_check': congruency_check
     }
 
@@ -236,15 +225,15 @@
     def __init__(
         self,
         data_dir,
     ) -> None:
         self._data_dir = data_dir
         self._partner = 'mimic3'
     def run(self):
-        cm = ConfigMapper(self._data_dir + '/config.ini').data
+        cm = ConfigMapper(self._data_dir + '/config.ini')
         metrics_logger = MetricLogger(cm)
 
         print('Gettings valid segments...')
         valid_records = load_valid_records(self._data_dir + 'valid_records.csv')
 
         print('Collecting samples...')
         json_data = ''
@@ -252,36 +241,36 @@
             data = self._get_data(record_path)
             if data:
                 ppg, abp = data[0], data[1]
             else:
                 continue
 
             # Apply bandpass filter to ppg
-            ppg = bandpass(ppg, low=cm.freq_band[0], high=cm.freq_band[1], fs=cm.fs)
+            ppg = bandpass(ppg, low=cm.data.freq_band[0], high=cm.data.freq_band[1], fs=cm.data.fs)
 
-            overlap = int(cm.fs / 2)
-            l = cm.win_len + overlap
+            overlap = int(cm.data.fs / 2)
+            l = cm.data.win_len + overlap
             idx = window(ppg, l, overlap)
 
             title_len = 50
             with alive_bar(total=len(idx), title_length=title_len, force_tty=True) as bar:
                 for i, j in idx:
                     bar.title(f'Rejected: {metrics_logger.rejected_samples} --- Collected: {metrics_logger.valid_samples}'.rjust(title_len))
                     p = ppg[i:j]
                     a = abp[i:j]
 
-                    p, a = align_signals(p, a, win_len=cm.win_len, fs=cm.fs)
+                    p, a = align_signals(p, a, win_len=cm.data.win_len, fs=cm.data.fs)
 
                     # Evaluate ppg
-                    p_win = Window(p, cm, cm.checks)
+                    p_win = Window(p, cm, cm.data.checks)
                     p_win.get_peaks()
                     p_valid = p_win.valid
 
                     # Evaluate abp
-                    a_win = Window(a, cm, cm.checks + ['bp'])
+                    a_win = Window(a, cm, cm.data.checks + ['bp'])
                     a_win.get_peaks()
                     a_valid = a_win.valid
 
                     # Evaluate ppg vs abp
                     congruence_check = congruency_check(p_win, a_win, cm)
                     valid = p_valid & a_valid & congruence_check['cong_check']
 
@@ -289,23 +278,23 @@
                     status = metrics_logger.update_metrics(metrics)
 
                     if valid:
                         json_data += json.dumps(dict(ppg=p.tolist(), abp=a.tolist())) + '\n'
 
                         # Write to file when count is reached. 
                         if status in [1, 2]:
-                            file_name = str(int(metrics_logger.valid_samples / cm.samples_per_file) - 1).zfill(3)
+                            file_name = str(int(metrics_logger.valid_samples / cm.data.samples_per_file) - 1).zfill(3)
                             file_path = self._data_dir + f'data/lines/{self._partner}_{file_name}.jsonlines'
                             write_to_json(json_data, file_path); json_data = ''
                             if status == 2:
                                 metrics_logger.save_stats(self._data_dir + f'{self._partner}_stats.csv')
                                 print('Done!')
                                 return
                     bar()
-                    if metrics_logger.patient_samples == cm.samples_per_patient:
+                    if metrics_logger.patient_samples == cm.data.samples_per_patient:
                         break
         return
 
     def _get_valid_segs(self, valid_path):
         valid_df = pd.read_csv(valid_path)
 
         # Extract data from valid_df and shuffle in the same order
```

### Comparing `heartfelt_tools-0.9.0/database_tools/tools/records.py` & `heartfelt_tools-1.7.0/database_tools/tools/records.py`

 * *Files identical despite different names*

### Comparing `heartfelt_tools-0.9.0/pyproject.toml` & `heartfelt_tools-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heartfelt-tools"
-version = "0.9.0"
+version = "1.7.0"
 description = "Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb."
 authors = ["Cameron Johnson"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "database_tools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `heartfelt_tools-0.9.0/setup.py` & `heartfelt_tools-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'tensorflow==2.9.2',
  'tqdm>=4.64.1,<5.0.0',
  'vitaldb>=1.2.10,<2.0.0',
  'wfdb>=4.0.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'heartfelt-tools',
-    'version': '0.9.0',
+    'version': '1.7.0',
     'description': 'Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb.',
     'long_description': '<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->\n<a name="readme-top"></a>\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n      \n            \n <img src="images/heartfelt-logo.png"  width="300em" height="300em"> \n\n  \n  <h1 align="center">MIMIC-III Database Tools</h1>\n\n  <p align="center">\n    For extracting and cleaning ppg and abp data from the MIMIC-III Waveforms Database.\n    <br />\n  </p>\n</div>\n\n\n\n<!-- TABLE OF CONTENTS -->\n<details>\n  <summary>Table of Contents</summary>\n  <ol>\n    <li>\n      <a href="#introduction">Introduction</a>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n      <ul>\n        <li><a href="#poetry">Poetry</a></li>\n        <li><a href="#get-valid-records">Get Valid Records</a></li>\n        <li><a href="#build-database">Build Database</a></li>\n        <li><a href="#evaluate-dataset">Evaluate Dataset</a></li>\n        <li><a href="#generate-records">Generate Records</a></li>\n        <li><a href="#read-records">Read Records</a></li>\n      </ul>\n    <li><a href="#license">License</a></li>\n  </ol>\n</details>\n\n\n\n<!-- Introduction -->\n## Introduction\n\nThis repo contains a set of tools for extracting and cleaning photoplethysmography (ppg) and artial blood pressure (abp) waveforms from the [MIMIC-III Waveforms Database](https://physionet.org/content/mimic3wdb/1.0/) for the purpose of blood pressure estimation via deep learning. \n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n<!-- GETTING STARTED -->\n## Getting Started\n\nThis sections details the requirements to start using this library. Links are for Ubuntu installation.\n\n### Prerequisites\n\n1. Python\n```shell\nsudo apt install python3.8 -y\nsudo apt install python3.8-dev python3.8-venv -y\n\necho \'export PATH="$PATH:/home/ubuntu/.local/bin"\' >> ~/.bashrc\nsource ~/.bashrc\n\ncurl -sS https://bootstrap.pypa.io/get-pip.py | python3.8\npython3.8 -m pip install virtualenv\npython3.8 -m venv .venv/base-env\necho \'alias base-env="source ~/.venv/base-env/bin/activate"\' >> ~/.bashrc\nbase-env\n\npython3.8 -m pip install --upgrade pip\n```\n2. Poetry\n```shell\ncurl -sSL https://install.python-poetry.org | python3 -\necho \'export PATH="$PATH:$HOME/.local/bin"\' >> ~/.bashrc\nsource ~/.bashrc\n\n# Verify installation\npoetry --version\n```\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\n### Poetry\nThe commands below can be used to install the poetry environment, build the project, and activate the environment.\n```shell\ncd database-tools\npoetry lock\npoetry install\npoetry build\npoetry shell\n```\n\n### Create Data Directory\nThe functions in this library rely on a data folder named with the convention `data-YYYY-MM-DD`. This directory contains two additional folders, `mimic3/` and `figures/`. The `mimic3/lines/` folder is intended to hold the jsonlines files the data will initially saved to. The `mimic3/records/` folder will hold the TFRecords files generated from these jsonlines files. This will be discussed in greater depth in the <a href="#generate-records">Generate Records</a> section.\n\n### Get Valid Records\nThe class DataLocator (located in `database_tools/tools/`) is specifically written to find valid data files in the MIMIC-III Waveforms subset and create a csv of the html links for these data files. Performing this task prior to downloading is done to improve runtime and the usability of this workflow. Valid records refers to data files that contain both PPG and ABP recordings and are at least 10 minutes in length. Currently this code is only intended for the MIMIC-III Waveforms subset but will likely be adapated to allow for valid segments to be identified in the MIMIC-III Matched Subset (records are linked to clinical data). To perform an extraction the file `scripts/get-valid-segs.py` can be run (data directory and repository path must be configured manually). This function will output a csv called `valid-segments.csv` to the data directory provided. The figure below shows how these signals are located.\n\nAdd mimic3 valid segs logic figure.\n\n### Build Database\nThe class `BuildDatabase` (located in `database_tools/tools/`) downloads data from `valid-segments.csv`, extracts PPG and ABP data, and then processed it by leveraging the `SignalProcessor` class (located in `database_tools/preprocessing/`). A database can be build by running `scripts/build_database.py` (be sure to configure the paths). BuildDatabase takes a few important parameters which modify how signals are excluded and how the signals are divided prior to processing. The `win_len` parameter controls the length of each window, `fs` is the sampling rate of the data (125 Hz in the case of MIMIC-III), while `samples_per_file`, `samples_per_patient`, and `max_samples` control the size of the dataset (how many files the data is spread across, how many samples a patient can contribute, and the total number of samples in the dataset. The final parameter `config` controls the various constants of the SignalProcessor that determine the quality threshold for accepting signals. The SignalProcessor filters signals according to the figure chart below. The functions used for this filtering can be found in `database_tools/preprocessing/`. Data exctracted with this script is saved directly to the `mimic3/lines/` folder in the data directory. A file named `mimic3_stats.csv` containing the stats of every processed waveform (not just the valid ones) will also be saved to the data directory.\n\nAdd data preprocessing figure.\n\n### Evaluate Dataset\nThe class `DataEvaluator` (located in `database_tools/tools/`) reads the `mimic3_stats.csv` file from the provided data directory and outputs figures to visualize the statistics. These figures are saved directly to the `figures/` folder in the data directory in addition to be output such that they can be viewed in a Jupyter notebook. The 3D histogram are generated using the fuction `histogram3d` located in `database_tools/plotting/`.\n\n### Generate Records\nOnce data has been extracted TFRecords can be generated for training a Tensorflow model. The class `RecordsHandler` contains the method `GenerateRecords` which is used to create the TFRecords. This can be done using `scripts/generate_records.py` (paths must be configured). When calling `GenerateRecords` the size of the train, validation, and test splits, as well as the max number of samples per file and a boolean to control whether or not the data is standardized must be specified (using `sklearn.preprocessing.StandardScaler()`.\n\n### Read Records\nThe class `RecordsHandler` also contains the function `ReadRecords` which can be used to read the TFRecords into a Tensorflow `TFRecordsDataset` object. This function can be used to inspect the integrity of the dataset or for loading the dataset for model training. The number of cores and a TensorFlow `AUTOTUNE` object must be provided.\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the MIT License. See `LICENSE.txt` for more information.\n\n<p align="right">(<a href="#readme-top">back to top</a>)</p>\n',
     'author': 'Cameron Johnson',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 'database_tools.processing', 'database_tools.tools'] package_data = \ {'':
 ['*']} install_requires = \ ['alive-progress>=3.0.1,<4.0.0',
 'heartpy>=1.2.7,<2.0.0', 'neurokit2>=0.2.1,<0.3.0', 'numpy>=1.23.4,<2.0.0',
 'openpyxl>=3.0.10,<4.0.0', 'pandas>=1.5.1,<2.0.0', 'plotly>=5.10.0,<6.0.0',
 'pytest>=7.2.1,<8.0.0', 'scikit-learn>=1.1.2,<2.0.0', 'scipy>=1.9.3,<2.0.0',
 'tabulate>=0.9.0,<0.10.0', 'tensorflow==2.9.2', 'tqdm>=4.64.1,<5.0.0',
 'vitaldb>=1.2.10,<2.0.0', 'wfdb>=4.0.0,<5.0.0'] setup_kwargs = { 'name':
-'heartfelt-tools', 'version': '0.9.0', 'description': 'Extract and process
+'heartfelt-tools', 'version': '1.7.0', 'description': 'Extract and process
 photoplethysmography and arterial blood pressure data from mimic3-waveforms and
 vitaldb.', 'long_description': '\n\n\n\n
 \n
                  \n \n \n [images/heartfelt-logo.png] \n\n \n
                     ****** MIMIC-III Database Tools ******
                                      \n\n
  \n For extracting and cleaning ppg and abp data from the MIMIC-III Waveforms
```

### Comparing `heartfelt_tools-0.9.0/PKG-INFO` & `heartfelt_tools-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartfelt-tools
-Version: 0.9.0
+Version: 1.7.0
 Summary: Extract and process photoplethysmography and arterial blood pressure data from mimic3-waveforms and vitaldb.
 License: MIT
 Author: Cameron Johnson
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: heartfelt-tools Version: 0.9.0 Summary: Extract and
+Metadata-Version: 2.1 Name: heartfelt-tools Version: 1.7.0 Summary: Extract and
 process photoplethysmography and arterial blood pressure data from mimic3-
 waveforms and vitaldb. License: MIT Author: Cameron Johnson Requires-Python:
 >=3.9,<3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Requires-Dist: alive-progress (>=3.0.1,<4.0.0) Requires-Dist: heartpy
 (>=1.2.7,<2.0.0) Requires-Dist: neurokit2 (>=0.2.1,<0.3.0) Requires-Dist: numpy
 (>=1.23.4,<2.0.0) Requires-Dist: openpyxl (>=3.0.10,<4.0.0) Requires-Dist:
```

