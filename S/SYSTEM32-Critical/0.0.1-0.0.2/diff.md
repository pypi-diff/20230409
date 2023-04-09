# Comparing `tmp/system32_critical-0.0.1.tar.gz` & `tmp/system32_critical-0.0.2.tar.gz`

## Comparing `system32_critical-0.0.1.tar` & `system32_critical-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 system32_critical-0.0.1/src/SYSTEM32_Critical/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 system32_critical-0.0.1/src/SYSTEM32_Critical/example.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 system32_critical-0.0.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 system32_critical-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 system32_critical-0.0.1/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 system32_critical-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 system32_critical-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 system32_critical-0.0.2/src/SYSTEM32_Critical/__init__.py
+-rw-r--r--   0        0        0    37443 2020-02-02 00:00:00.000000 system32_critical-0.0.2/src/SYSTEM32_Critical/example.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 system32_critical-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 system32_critical-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 system32_critical-0.0.2/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 system32_critical-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 system32_critical-0.0.2/PKG-INFO
```

### Comparing `system32_critical-0.0.1/LICENSE` & `system32_critical-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `system32_critical-0.0.1/pyproject.toml` & `system32_critical-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "SYSTEM32_Critical"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Harley Davidson", email="author@harley-davidson.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.2"
 classifiers = [
```

