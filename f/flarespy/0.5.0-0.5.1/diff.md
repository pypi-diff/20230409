# Comparing `tmp/flarespy-0.5.0.tar.gz` & `tmp/flarespy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.5.0.tar", max compression
+gzip compressed data, was "flarespy-0.5.1.tar", max compression
```

## Comparing `flarespy-0.5.0.tar` & `flarespy-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.5.0/LICENSE
--rw-r--r--   0        0        0      615 2023-03-29 16:17:57.866520 flarespy-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.5.0/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.5.0/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.5.0/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    25108 2023-03-30 09:31:09.941091 flarespy-0.5.0/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4172 2023-03-29 03:24:28.928776 flarespy-0.5.0/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-03-29 16:17:57.868589 flarespy-0.5.0/src/flarespy/version.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 flarespy-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.5.1/LICENSE
+-rw-r--r--   0        0        0      663 2023-04-07 13:43:15.879227 flarespy-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.5.1/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.5.1/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.5.1/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    25108 2023-03-30 09:31:09.941091 flarespy-0.5.1/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     3994 2023-04-07 14:40:27.932103 flarespy-0.5.1/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-07 03:16:36.299414 flarespy-0.5.1/src/flarespy/version.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 flarespy-0.5.1/PKG-INFO
```

### Comparing `flarespy-0.5.0/LICENSE` & `flarespy-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.0/pyproject.toml` & `flarespy-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "flarespy"
-version = "0.5.0"
+version = "0.5.1"
 description = "Find flares in TESS light curves"
 authors = ["Keyu Xing <kyxing@mail.bnu.edu.cn>"]
 license = "MIT"
 homepage = "https://github.com/keyuxing/flarespy"
 repository = "https://github.com/keyuxing/flarespy"
 
 [tool.poetry.dependencies]
 bottleneck = ">=1.3"
 lightkurve = ">=2.3"
-numba = ">=0.55.2"
-python = ">=3.8,<=3.11"
+numba = { version = ">=0.55.2", allow-prereleases = true}
+pandas = "<2.0"
+python = ">=3.8"
 retrying = ">=1.3"
 scikit-learn = ">=1.1"
 tsfresh = ">=0.20"
 wotan = ">=1.10"
 
 [tool.poetry.dev-dependencies]
 black = ">=22.8"
```

### Comparing `flarespy-0.5.0/src/flarespy/Flare_model.py` & `flarespy-0.5.1/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.0/src/flarespy/data/model.dat` & `flarespy-0.5.1/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.0/src/flarespy/flarefinder.py` & `flarespy-0.5.1/src/flarespy/flarefinder.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.0/src/flarespy/utils.py` & `flarespy-0.5.1/src/flarespy/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,44 +60,44 @@
 
 def extend(time, flux, t_start, t_stop, t_max_extend, n_sigma=1, n_left=1, n_right=1, mode=1):
     indexes_range = np.nonzero((time >= t_start - t_max_extend) & (time <= t_stop + t_max_extend))[0]
     i_start = np.nonzero(time == t_start)[0][0]
     i_stop = np.nonzero(time == t_stop)[0][0]
 
     # left
-    if mode == 1:
-        while (flux[i_start - n_left : i_start] > n_sigma).any() and i_start > indexes_range[0]:
-            i_start -= 1
-            if i_start < n_left:
-                i_start = 0
-                break
-        i_start = max(0, i_start - 1, indexes_range[0])
-    elif mode == -1:
-        while (flux[i_start - n_left : i_start] < n_sigma).any() and i_start > indexes_range[0]:
-            i_start -= 1
-            if i_start < n_left:
-                i_start = 0
-                break
-        i_start = max(0, i_start - 1, indexes_range[0])
+    def condition_left(index):
+        if mode == 1:
+            return (flux[index - n_left : index] > n_sigma).any()
+        elif mode == -1:
+            return (flux[index - n_left : index] < n_sigma).any()
+        else:
+            raise ValueError("mode must be 1 or -1")
+
+    while condition_left(i_start) and i_start > indexes_range[0]:
+        i_start -= 1
+        if i_start < n_left:
+            i_start = 0
+            break
+    i_start = max(0, i_start - 1, indexes_range[0])
 
     # right
-    if mode == 1:
-        while (flux[i_stop + 1 : i_stop + 1 + n_right] > n_sigma).any() and i_stop < indexes_range[-1]:
-            i_stop += 1
-            if i_stop + 1 + n_right > time.size:
-                i_stop = time.size - 1
-                break
-        i_stop = min(time.size - 1, i_stop + 1, indexes_range[-1])
-    elif mode == -1:
-        while (flux[i_stop + 1 : i_stop + 1 + n_right] < n_sigma).any() and i_stop < indexes_range[-1]:
-            i_stop += 1
-            if i_stop + 1 + n_right > time.size:
-                i_stop = time.size - 1
-                break
-        i_stop = min(time.size - 1, i_stop + 1, indexes_range[-1])
+    def condition_right(index):
+        if mode == 1:
+            return (flux[index + 1 : index + 1 + n_right] > n_sigma).any()
+        elif mode == -1:
+            return (flux[index + 1 : index + 1 + n_right] < n_sigma).any()
+        else:
+            raise ValueError("mode must be 1 or -1")
+
+    while condition_right(i_stop) and i_stop < indexes_range[-1]:
+        i_stop += 1
+        if i_stop + 1 + n_right > time.size:
+            i_stop = time.size - 1
+            break
+    i_stop = min(time.size - 1, i_stop + 1, indexes_range[-1])
 
     return time[i_start], time[i_stop]
 
 
 def find_consecutive(indexes, n_consecutive, gap=1, data=None):
     if data is None:
         grouped_data = np.split(indexes, np.nonzero(np.diff(indexes) > gap)[0] + 1)
```

### Comparing `flarespy-0.5.0/PKG-INFO` & `flarespy-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
-Requires-Python: >=3.8,<=3.11
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bottleneck (>=1.3)
 Requires-Dist: lightkurve (>=2.3)
 Requires-Dist: numba (>=0.55.2)
+Requires-Dist: pandas (<2.0)
 Requires-Dist: retrying (>=1.3)
 Requires-Dist: scikit-learn (>=1.1)
 Requires-Dist: tsfresh (>=0.20)
 Requires-Dist: wotan (>=1.10)
 Project-URL: Repository, https://github.com/keyuxing/flarespy
```

