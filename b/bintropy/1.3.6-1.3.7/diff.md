# Comparing `tmp/bintropy-1.3.6.tar.gz` & `tmp/bintropy-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bintropy-1.3.6.tar", last modified: Fri Mar  3 21:56:59 2023, max compression
+gzip compressed data, was "bintropy-1.3.7.tar", last modified: Sun Apr  9 10:37:51 2023, max compression
```

## Comparing `bintropy-1.3.6.tar` & `bintropy-1.3.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:56:59.238272 bintropy-1.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:56:59.234272 bintropy-1.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:56:59.234272 bintropy-1.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-03 21:56:51.000000 bintropy-1.3.6/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-03-03 21:56:51.000000 bintropy-1.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-03 21:56:51.000000 bintropy-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-03-03 21:56:59.238272 bintropy-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-03-03 21:56:51.000000 bintropy-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:56:59.234272 bintropy-1.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-03-03 21:56:51.000000 bintropy-1.3.6/docs/example-not-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-03-03 21:56:51.000000 bintropy-1.3.6/docs/example-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-03-03 21:56:51.000000 bintropy-1.3.6/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-03 21:56:51.000000 bintropy-1.3.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-03 21:56:51.000000 bintropy-1.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 21:56:59.238272 bintropy-1.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:56:59.234272 bintropy-1.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:56:59.234272 bintropy-1.3.6/src/bintropy/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-03 21:56:51.000000 bintropy-1.3.6/src/bintropy/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-03 21:56:51.000000 bintropy-1.3.6/src/bintropy/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-03-03 21:56:51.000000 bintropy-1.3.6/src/bintropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-03-03 21:56:51.000000 bintropy-1.3.6/src/bintropy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 21:56:59.238272 bintropy-1.3.6/src/bintropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-03-03 21:56:59.000000 bintropy-1.3.6/src/bintropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-03 21:56:59.000000 bintropy-1.3.6/src/bintropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 21:56:59.000000 bintropy-1.3.6/src/bintropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-03 21:56:59.000000 bintropy-1.3.6/src/bintropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-03 21:56:59.000000 bintropy-1.3.6/src/bintropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-03 21:56:59.000000 bintropy-1.3.6/src/bintropy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.410348 bintropy-1.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.406348 bintropy-1.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.406348 bintropy-1.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-09 10:37:43.000000 bintropy-1.3.7/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-09 10:37:43.000000 bintropy-1.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 10:37:43.000000 bintropy-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-09 10:37:51.410348 bintropy-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-09 10:37:43.000000 bintropy-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.406348 bintropy-1.3.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-09 10:37:43.000000 bintropy-1.3.7/docs/example-not-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-09 10:37:43.000000 bintropy-1.3.7/docs/example-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-09 10:37:43.000000 bintropy-1.3.7/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-09 10:37:43.000000 bintropy-1.3.7/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-04-09 10:37:43.000000 bintropy-1.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 10:37:51.410348 bintropy-1.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.406348 bintropy-1.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.410348 bintropy-1.3.7/src/bintropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 10:37:43.000000 bintropy-1.3.7/src/bintropy/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 10:37:43.000000 bintropy-1.3.7/src/bintropy/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-04-09 10:37:43.000000 bintropy-1.3.7/src/bintropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-09 10:37:43.000000 bintropy-1.3.7/src/bintropy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:37:51.410348 bintropy-1.3.7/src/bintropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 10:37:51.000000 bintropy-1.3.7/src/bintropy.egg-info/top_level.txt
```

### Comparing `bintropy-1.3.6/.github/workflows/python-package.yml` & `bintropy-1.3.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/.gitignore` & `bintropy-1.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/LICENSE` & `bintropy-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/PKG-INFO` & `bintropy-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.3.6
+Version: 1.3.7
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bintropy-1.3.6/README.md` & `bintropy-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/docs/example-not-packed.png` & `bintropy-1.3.7/docs/example-not-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/docs/example-packed.png` & `bintropy-1.3.7/docs/example-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/docs/logo.png` & `bintropy-1.3.7/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/pyproject.toml` & `bintropy-1.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/src/bintropy/__info__.py` & `bintropy-1.3.7/src/bintropy/__info__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/src/bintropy/__init__.py` & `bintropy-1.3.7/src/bintropy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,21 @@
         if logger:
             msg = "Entropy (average): {}".format(e[1] or "-")
             if e[0] != [None]:
                 iw = len(str(len(e[0])))
                 for i, j in enumerate(e[0]):
                     msg += ("\n    #{: <%s}: {}" % iw).format(i + 1, "-" if j is None else j)
             __log(logger, msg)
-        return is_packed(e[0], e[1], _t1, _t2, logger) if decide else (max([x for x in e[0] if x is not None]), e[1])
+        if decide:
+            return is_packed(e[0], e[1], _t1, _t2, logger)
+        else:
+            try:
+                return max([x for x in e[0] if x is not None]), e[1]
+            except ValueError:  # occurs when ignore_half_block_zeros=True and all the blocks have more than half of
+                return 0., 0.   #  their bytes being zeros
     # SECOND AND THIRD MODES: compute a weighted entropy of all the sections or segments of the executable
     else:
         def _handle(n, d):
             r = entropy(d, blocksize, ignore_half_block_zeros)
             e[n] = r if isinstance(r, (list, tuple)) else ([r], r)
             w[n] = len(d)
         e, w = {}, {}
```

### Comparing `bintropy-1.3.6/src/bintropy/__main__.py` & `bintropy-1.3.7/src/bintropy/__main__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.3.6/src/bintropy.egg-info/PKG-INFO` & `bintropy-1.3.7/src/bintropy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.3.6
+Version: 1.3.7
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

