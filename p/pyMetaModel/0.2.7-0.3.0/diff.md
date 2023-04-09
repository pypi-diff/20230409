# Comparing `tmp/pymetamodel-0.2.7.tar.gz` & `tmp/pymetamodel-0.3.0.tar.gz`

## Comparing `pymetamodel-0.2.7.tar` & `pymetamodel-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/.pydevproject
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.mermaid
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.puml
--rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.sidif
--rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.xlsx
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.yaml
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/ceur-ws/ceur-ws_puml.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/city/city.mermaid
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/city/city.puml
--rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/city/city.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/city/city.sidif
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/city/city.xlsx
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/city/city.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/city/city_puml.txt
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/family/FamilyContext.mermaid
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/family/FamilyContext.puml
--rw-r--r--   0        0        0    21929 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/family/FamilyContext.py
--rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/family/FamilyContext.sidif
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/family/FamilyContext.xlsx
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/family/FamilyContext.yaml
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/family/FamilyContext_puml.txt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/metamodel/metamodel.mermaid
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/metamodel/metamodel.puml
--rw-r--r--   0        0        0    43805 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/metamodel/metamodel.py
--rw-r--r--   0        0        0    36709 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/metamodel/metamodel.sidif
--rw-r--r--   0        0        0     7772 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/metamodel/metamodel.xlsx
--rw-r--r--   0        0        0    36314 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/metamodel/metamodel.yaml
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/metamodel/metamodel_puml.txt
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/scientific-events/scientific-events.mermaid
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/scientific-events/scientific-events.puml
--rw-r--r--   0        0        0    30577 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/scientific-events/scientific-events.py
--rw-r--r--   0        0        0    22450 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/scientific-events/scientific-events.sidif
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/scientific-events/scientific-events.xlsx
--rw-r--r--   0        0        0    20688 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/scientific-events/scientific-events.yaml
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/scientific-events/scientific-events_puml.txt
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/teaching/TeachingSchema.mermaid
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/teaching/TeachingSchema.puml
--rw-r--r--   0        0        0    46242 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/teaching/TeachingSchema.py
--rw-r--r--   0        0        0    31307 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/teaching/TeachingSchema.sidif
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/teaching/TeachingSchema.xlsx
--rw-r--r--   0        0        0    26187 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/teaching/TeachingSchema.yaml
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/examples/teaching/TeachingSchema_puml.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/__init__.py
--rw-r--r--   0        0        0    18961 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/metamodel.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/metamodel_cmd.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/mw.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/profiler.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/sidif2linkml.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/smw_type.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/uml.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/meta/version.py
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/scripts/genexamples
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/scripts/install
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/tests/basemwtest.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/tests/basetest.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/tests/test_linkml.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/tests/test_metamodel.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/tests/test_mw.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/tests/test_plantuml.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/tests/test_sidif.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/LICENSE
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/README.md
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    15891 2020-02-02 00:00:00.000000 pymetamodel-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.pydevproject
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.mermaid
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.puml
+-rw-r--r--   0        0        0    16059 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.py
+-rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.sidif
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.xlsx
+-rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.yaml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws_puml.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.mermaid
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.puml
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.sidif
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.xlsx
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city_puml.txt
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.mermaid
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.puml
+-rw-r--r--   0        0        0    21685 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.py
+-rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.sidif
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.xlsx
+-rw-r--r--   0        0        0    10664 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.yaml
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext_puml.txt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.mermaid
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.puml
+-rw-r--r--   0        0        0    43565 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.py
+-rw-r--r--   0        0        0    36709 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.sidif
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.xlsx
+-rw-r--r--   0        0        0    35205 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.yaml
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel_puml.txt
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.mermaid
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.puml
+-rw-r--r--   0        0        0    30338 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.py
+-rw-r--r--   0        0        0    22450 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.sidif
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.xlsx
+-rw-r--r--   0        0        0    19579 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.yaml
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events_puml.txt
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.mermaid
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.puml
+-rw-r--r--   0        0        0    45997 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.py
+-rw-r--r--   0        0        0    31307 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.sidif
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.xlsx
+-rw-r--r--   0        0        0    25078 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.yaml
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema_puml.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/__init__.py
+-rw-r--r--   0        0        0    19028 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/metamodel.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/metamodel_cmd.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/mw.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/profiler.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/sidif2linkml.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/smw_type.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/uml.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/version.py
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/scripts/genexamples
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/scripts/install
+-rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/basemwtest.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/basetest.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_linkml.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_metamodel.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_mw.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_plantuml.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_sidif.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/README.md
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    15893 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/PKG-INFO
```

### Comparing `pymetamodel-0.2.7/.github/workflows/build.yml` & `pymetamodel-0.3.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/.github/workflows/upload-to-pypi.yml` & `pymetamodel-0.3.0/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.puml` & `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.puml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 package CeurwsSchema {
   class Volume {
     number:Number
+    acronym:text
+    wikidataid:External identifier
     title:Text
+    description:text
+    url:text
+    date:Date
+    dblp:External identifier
+    k10plus:External identifier
+    urn:External identifier
   }
 Note top of Volume
 A Volume is a collection of papers mostly documenting the results of an academic event
 End note
   class Session {
     title:Text
   }
 Note top of Session
 A Session is a a collection of papers as part of a Volume
 End note
   class Paper {
     id:Text
+    wikidataid:External identifier
+    description:text
     title:Text
-    authors:Text
     pdfUrl:URL
   }
 Note top of Paper
 A paper is e.g. a scholarly article
 End note
 }
 Volume "volume 1" -- "sessions *" Session
 Volume "volume 1" -- "papers *" Paper
+Volume "volumes *" -- "editors *" Scholar
 Session "session 1" -- "papers *" Paper
+Paper "papers *" -- "authors *" Scholar
 
 ' BITPlan Corporate identity skin params
 ' Copyright (c) 2015-2023 BITPlan GmbH
 ' see http://wiki.bitplan.com/PlantUmlSkinParams#BITPlanCI
 ' skinparams generated by com.bitplan.restmodelmanager
 skinparam note {
   BackGroundColor #FFFFFF
```

### Comparing `pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.py` & `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from ceur-ws.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-08T09:55:09
+# Generation date: 2023-03-23T07:28:10
 # Schema: CeurwsSchema
 #
 # id: CeurwsSchema
 # description:
 # license:
 
 import dataclasses
@@ -18,26 +18,25 @@
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
 from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
 from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.metamodelcore import Bool, Curie, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
+from linkml_runtime.utils.metamodelcore import Bool, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
 CEURWSSCHEMA = CurieNamespace('CeurwsSchema', 'CeurwsSchema/')
 LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
-SCHEMA = CurieNamespace('schema', 'http://schema.org/')
 SHEX = CurieNamespace('shex', 'http://www.w3.org/ns/shex#')
 XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = CEURWSSCHEMA
 
 
 # Types
 class String(str):
@@ -124,22 +123,14 @@
     """ a URI or a CURIE """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uriorcurie"
     type_model_uri = CEURWSSCHEMA.Uriorcurie
 
 
-class Curie(Curie):
-    """ a compact URI """
-    type_class_uri = XSD.string
-    type_class_curie = "xsd:string"
-    type_name = "curie"
-    type_model_uri = CEURWSSCHEMA.Curie
-
-
 class Uri(URI):
     """ a complete URI """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uri"
     type_model_uri = CEURWSSCHEMA.Uri
 
@@ -181,23 +172,55 @@
 
     class_class_uri: ClassVar[URIRef] = CEURWSSCHEMA.Volume
     class_class_curie: ClassVar[str] = "CeurwsSchema:Volume"
     class_name: ClassVar[str] = "Volume"
     class_model_uri: ClassVar[URIRef] = CEURWSSCHEMA.Volume
 
     number: Optional[float] = None
+    acronym: Optional[str] = None
+    wikidataid: Optional[str] = None
     title: Optional[str] = None
+    description: Optional[str] = None
+    url: Optional[str] = None
+    date: Optional[Union[str, XSDDate]] = None
+    dblp: Optional[str] = None
+    k10plus: Optional[str] = None
+    urn: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.number is not None and not isinstance(self.number, float):
             self.number = float(self.number)
 
+        if self.acronym is not None and not isinstance(self.acronym, str):
+            self.acronym = str(self.acronym)
+
+        if self.wikidataid is not None and not isinstance(self.wikidataid, str):
+            self.wikidataid = str(self.wikidataid)
+
         if self.title is not None and not isinstance(self.title, str):
             self.title = str(self.title)
 
+        if self.description is not None and not isinstance(self.description, str):
+            self.description = str(self.description)
+
+        if self.url is not None and not isinstance(self.url, str):
+            self.url = str(self.url)
+
+        if self.date is not None and not isinstance(self.date, XSDDate):
+            self.date = XSDDate(self.date)
+
+        if self.dblp is not None and not isinstance(self.dblp, str):
+            self.dblp = str(self.dblp)
+
+        if self.k10plus is not None and not isinstance(self.k10plus, str):
+            self.k10plus = str(self.k10plus)
+
+        if self.urn is not None and not isinstance(self.urn, str):
+            self.urn = str(self.urn)
+
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class Session(YAMLRoot):
     """
     A Session is a a collection of papers as part of a Volume
@@ -230,31 +253,35 @@
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = CEURWSSCHEMA.Paper
     class_class_curie: ClassVar[str] = "CeurwsSchema:Paper"
     class_name: ClassVar[str] = "Paper"
     class_model_uri: ClassVar[URIRef] = CEURWSSCHEMA.Paper
 
+    description: Optional[str] = None
     id: Optional[str] = None
+    wikidataid: Optional[str] = None
     title: Optional[str] = None
-    authors: Optional[str] = None
     pdfUrl: Optional[Union[str, URI]] = None
     volume: Optional[Union[dict, Volume]] = None
     session: Optional[Union[dict, Session]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self.description is not None and not isinstance(self.description, str):
+            self.description = str(self.description)
+
         if self.id is not None and not isinstance(self.id, str):
             self.id = str(self.id)
 
+        if self.wikidataid is not None and not isinstance(self.wikidataid, str):
+            self.wikidataid = str(self.wikidataid)
+
         if self.title is not None and not isinstance(self.title, str):
             self.title = str(self.title)
 
-        if self.authors is not None and not isinstance(self.authors, str):
-            self.authors = str(self.authors)
-
         if self.pdfUrl is not None and not isinstance(self.pdfUrl, URI):
             self.pdfUrl = URI(self.pdfUrl)
 
         if self.volume is not None and not isinstance(self.volume, Volume):
             self.volume = Volume(**as_dict(self.volume))
 
         if self.session is not None and not isinstance(self.session, Session):
@@ -269,53 +296,101 @@
 # Slots
 class slots:
     pass
 
 slots.number = Slot(uri=CEURWSSCHEMA.number, name="number", curie=CEURWSSCHEMA.curie('number'),
                    model_uri=CEURWSSCHEMA.number, domain=None, range=Optional[float])
 
+slots.acronym = Slot(uri=CEURWSSCHEMA.acronym, name="acronym", curie=CEURWSSCHEMA.curie('acronym'),
+                   model_uri=CEURWSSCHEMA.acronym, domain=None, range=Optional[str])
+
+slots.wikidataid = Slot(uri=CEURWSSCHEMA.wikidataid, name="wikidataid", curie=CEURWSSCHEMA.curie('wikidataid'),
+                   model_uri=CEURWSSCHEMA.wikidataid, domain=None, range=Optional[str])
+
 slots.title = Slot(uri=CEURWSSCHEMA.title, name="title", curie=CEURWSSCHEMA.curie('title'),
                    model_uri=CEURWSSCHEMA.title, domain=None, range=Optional[str])
 
+slots.description = Slot(uri=CEURWSSCHEMA.description, name="description", curie=CEURWSSCHEMA.curie('description'),
+                   model_uri=CEURWSSCHEMA.description, domain=None, range=Optional[str])
+
+slots.url = Slot(uri=CEURWSSCHEMA.url, name="url", curie=CEURWSSCHEMA.curie('url'),
+                   model_uri=CEURWSSCHEMA.url, domain=None, range=Optional[str])
+
+slots.date = Slot(uri=CEURWSSCHEMA.date, name="date", curie=CEURWSSCHEMA.curie('date'),
+                   model_uri=CEURWSSCHEMA.date, domain=None, range=Optional[Union[str, XSDDate]])
+
+slots.dblp = Slot(uri=CEURWSSCHEMA.dblp, name="dblp", curie=CEURWSSCHEMA.curie('dblp'),
+                   model_uri=CEURWSSCHEMA.dblp, domain=None, range=Optional[str])
+
+slots.k10plus = Slot(uri=CEURWSSCHEMA.k10plus, name="k10plus", curie=CEURWSSCHEMA.curie('k10plus'),
+                   model_uri=CEURWSSCHEMA.k10plus, domain=None, range=Optional[str])
+
+slots.urn = Slot(uri=CEURWSSCHEMA.urn, name="urn", curie=CEURWSSCHEMA.curie('urn'),
+                   model_uri=CEURWSSCHEMA.urn, domain=None, range=Optional[str])
+
 slots.volume = Slot(uri=CEURWSSCHEMA.volume, name="volume", curie=CEURWSSCHEMA.curie('volume'),
                    model_uri=CEURWSSCHEMA.volume, domain=None, range=Optional[Union[dict, Volume]])
 
 slots.id = Slot(uri=CEURWSSCHEMA.id, name="id", curie=CEURWSSCHEMA.curie('id'),
                    model_uri=CEURWSSCHEMA.id, domain=None, range=Optional[str])
 
-slots.authors = Slot(uri=CEURWSSCHEMA.authors, name="authors", curie=CEURWSSCHEMA.curie('authors'),
-                   model_uri=CEURWSSCHEMA.authors, domain=None, range=Optional[str])
-
 slots.pdfUrl = Slot(uri=CEURWSSCHEMA.pdfUrl, name="pdfUrl", curie=CEURWSSCHEMA.curie('pdfUrl'),
                    model_uri=CEURWSSCHEMA.pdfUrl, domain=None, range=Optional[Union[str, URI]])
 
 slots.session = Slot(uri=CEURWSSCHEMA.session, name="session", curie=CEURWSSCHEMA.curie('session'),
                    model_uri=CEURWSSCHEMA.session, domain=None, range=Optional[Union[dict, Session]])
 
 slots.volume__number = Slot(uri=CEURWSSCHEMA.number, name="volume__number", curie=CEURWSSCHEMA.curie('number'),
                    model_uri=CEURWSSCHEMA.volume__number, domain=None, range=Optional[float])
 
+slots.volume__acronym = Slot(uri=CEURWSSCHEMA.acronym, name="volume__acronym", curie=CEURWSSCHEMA.curie('acronym'),
+                   model_uri=CEURWSSCHEMA.volume__acronym, domain=None, range=Optional[str])
+
+slots.volume__wikidataid = Slot(uri=CEURWSSCHEMA.wikidataid, name="volume__wikidataid", curie=CEURWSSCHEMA.curie('wikidataid'),
+                   model_uri=CEURWSSCHEMA.volume__wikidataid, domain=None, range=Optional[str])
+
 slots.volume__title = Slot(uri=CEURWSSCHEMA.title, name="volume__title", curie=CEURWSSCHEMA.curie('title'),
                    model_uri=CEURWSSCHEMA.volume__title, domain=None, range=Optional[str])
 
+slots.volume__description = Slot(uri=CEURWSSCHEMA.description, name="volume__description", curie=CEURWSSCHEMA.curie('description'),
+                   model_uri=CEURWSSCHEMA.volume__description, domain=None, range=Optional[str])
+
+slots.volume__url = Slot(uri=CEURWSSCHEMA.url, name="volume__url", curie=CEURWSSCHEMA.curie('url'),
+                   model_uri=CEURWSSCHEMA.volume__url, domain=None, range=Optional[str])
+
+slots.volume__date = Slot(uri=CEURWSSCHEMA.date, name="volume__date", curie=CEURWSSCHEMA.curie('date'),
+                   model_uri=CEURWSSCHEMA.volume__date, domain=None, range=Optional[Union[str, XSDDate]])
+
+slots.volume__dblp = Slot(uri=CEURWSSCHEMA.dblp, name="volume__dblp", curie=CEURWSSCHEMA.curie('dblp'),
+                   model_uri=CEURWSSCHEMA.volume__dblp, domain=None, range=Optional[str])
+
+slots.volume__k10plus = Slot(uri=CEURWSSCHEMA.k10plus, name="volume__k10plus", curie=CEURWSSCHEMA.curie('k10plus'),
+                   model_uri=CEURWSSCHEMA.volume__k10plus, domain=None, range=Optional[str])
+
+slots.volume__urn = Slot(uri=CEURWSSCHEMA.urn, name="volume__urn", curie=CEURWSSCHEMA.curie('urn'),
+                   model_uri=CEURWSSCHEMA.volume__urn, domain=None, range=Optional[str])
+
 slots.session__title = Slot(uri=CEURWSSCHEMA.title, name="session__title", curie=CEURWSSCHEMA.curie('title'),
                    model_uri=CEURWSSCHEMA.session__title, domain=None, range=Optional[str])
 
 slots.session__volume = Slot(uri=CEURWSSCHEMA.volume, name="session__volume", curie=CEURWSSCHEMA.curie('volume'),
                    model_uri=CEURWSSCHEMA.session__volume, domain=None, range=Optional[Union[dict, Volume]])
 
+slots.paper__description = Slot(uri=CEURWSSCHEMA.description, name="paper__description", curie=CEURWSSCHEMA.curie('description'),
+                   model_uri=CEURWSSCHEMA.paper__description, domain=None, range=Optional[str])
+
 slots.paper__id = Slot(uri=CEURWSSCHEMA.id, name="paper__id", curie=CEURWSSCHEMA.curie('id'),
                    model_uri=CEURWSSCHEMA.paper__id, domain=None, range=Optional[str])
 
+slots.paper__wikidataid = Slot(uri=CEURWSSCHEMA.wikidataid, name="paper__wikidataid", curie=CEURWSSCHEMA.curie('wikidataid'),
+                   model_uri=CEURWSSCHEMA.paper__wikidataid, domain=None, range=Optional[str])
+
 slots.paper__title = Slot(uri=CEURWSSCHEMA.title, name="paper__title", curie=CEURWSSCHEMA.curie('title'),
                    model_uri=CEURWSSCHEMA.paper__title, domain=None, range=Optional[str])
 
-slots.paper__authors = Slot(uri=CEURWSSCHEMA.authors, name="paper__authors", curie=CEURWSSCHEMA.curie('authors'),
-                   model_uri=CEURWSSCHEMA.paper__authors, domain=None, range=Optional[str])
-
 slots.paper__pdfUrl = Slot(uri=CEURWSSCHEMA.pdfUrl, name="paper__pdfUrl", curie=CEURWSSCHEMA.curie('pdfUrl'),
                    model_uri=CEURWSSCHEMA.paper__pdfUrl, domain=None, range=Optional[Union[str, URI]])
 
 slots.paper__volume = Slot(uri=CEURWSSCHEMA.volume, name="paper__volume", curie=CEURWSSCHEMA.curie('volume'),
                    model_uri=CEURWSSCHEMA.paper__volume, domain=None, range=Optional[Union[dict, Volume]])
 
 slots.paper__session = Slot(uri=CEURWSSCHEMA.session, name="paper__session", curie=CEURWSSCHEMA.curie('session'),
```

### Comparing `pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.xlsx` & `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.xlsx`

 * *Files 20% similar despite different names*

```diff
@@ -1,365 +1,369 @@
-00000000: 504b 0304 1400 0000 0800 e54e 6856 0741  PK.........NhV.A
+00000000: 504b 0304 1400 0000 0800 853b 7756 0741  PK.........;wV.A
 00000010: 4d62 8100 0000 b100 0000 1000 0000 646f  Mb............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 3d0b 0231 1044 ffca 71bd b741 c142 6240  =..1.D..q..A.Bb@
 00000040: d052 b0b2 0f7b 1b2f 9064 43b2 427e be39  .R...{./.dC.B~.9
 00000050: c18f 6e1e 6f18 46df 0a67 2ae2 a90e 2d86  ..n.o.F..g*...-.
 00000060: 548f e322 920f 0015 178a b64e 5da7 6e1c  T..".......N].n.
 00000070: 9768 a563 7900 3be7 91ce 8ccf 4849 60ab  .h.cy.;.....HI`.
 00000080: d41e a809 a599 e64d fe0e 8e46 9f72 0e1e  .......M...F.r..
 00000090: ad78 4ee6 eab1 7065 27c3 a521 050d ff72  .xN...pe'..!...r
 000000a0: 6dde a9d4 35ef 26f5 961f d6f0 3b69 5e50  m...5.&.....;i^P
-000000b0: 4b03 0414 0000 0008 00e5 4e68 56fb f623  K.........NhV..#
-000000c0: b2ef 0000 002b 0200 0011 0000 0064 6f63  .....+.......doc
+000000b0: 4b03 0414 0000 0008 0085 3b77 5614 9990  K.........;wV...
+000000c0: e0ee 0000 002b 0200 0011 0000 0064 6f63  .....+.......doc
 000000d0: 5072 6f70 732f 636f 7265 2e78 6d6c cd92  Props/core.xml..
-000000e0: c16a c330 0c86 5f65 f89e c849 e828 26cd  .j.0.._e...I.(&.
-000000f0: 65a5 a70d 062b 6cec 666c b535 8b1d 636b  e....+l.fl.5..ck
-00000100: 247d fb39 5e9b 32b6 0718 f862 e9f7 a74f  $}.9^.2....b...O
-00000110: e056 79a1 8680 cf61 f018 c860 bc9b 6cef  .Vy....a...`..l.
-00000120: a250 7ec3 4e44 5e00 4475 422b 6399 122e  .P~.ND^.DuB+c...
-00000130: 350f 43b0 92d2 351c c14b f521 8f08 35e7  5.C...5..K.!..5.
-00000140: f760 91a4 9624 6106 167e 21b2 aed5 4aa8  .`...$a..~!...J.
-00000150: 8092 8670 c16b b5e0 fd67 e833 4c2b c01e  ...p.k...g.3L+..
-00000160: 2d3a 8a50 9515 b06e 9ee8 cf53 dfc2 0d30  -:.P...n...S...0
-00000170: c308 838d df05 d40b 3157 ffc4 e60e b04b  ........1W.....K
-00000180: 728a 6649 8de3 588e 4dce a51d 2a78 7b7a  r.fI..X.M...*x{z
-00000190: 7cc9 eb16 c645 924e 617a 158d a0b3 c70d  |....E.Naz......
-000001a0: bb4e 7e6d 1eb6 fb1d eb6a 5e37 054f 67bd  .N~m.....j^7.Og.
-000001b0: e76b b15a 898a bfcf ae3f fc6e c276 d0e6  .k.Z.....?.n.v..
-000001c0: 60fe b1f1 55b0 6be1 d7bf e8be 0050 4b03  `...U.k......PK.
-000001d0: 0414 0000 0008 00e5 4e68 5699 5c9c 2310  ........NhV.\.#.
-000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
-000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
-00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
-00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
-00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
-00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
-00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
-00000250: b72f dee0 5732 2411 4130 19a7 aff0 c00a  ./..W2$.A0......
-00000260: a54c 5eb5 5a69 00c3 387d c913 12c3 dc82  .L^.Zi..8}......
-00000270: 8b08 4b78 14cb d65c e05b 1a2f 23d6 eab4  ..Kx...\.[./#...
-00000280: dbdd 5684 696c a118 4764 607d 5e2c 6840  ..V.il..Gd`}^,h@
-00000290: d054 515a 6f5f 20b4 e51f 33f8 15cb 548d  .TQZo_ ...3...T.
-000002a0: 65a3 0113 5741 26b9 88b4 f2f9 6cc5 fcda  e...WA&.....l...
-000002b0: de3e 65cf e93a 1d32 816e 301b 5820 7fce  .>e..:.2.n0.X ..
-000002c0: 6fa7 e44e 5a88 e154 c2c4 c06a 673f 566b  o..NZ..T...jg?Vk
-000002d0: c7d1 d248 8082 c97d 9405 ba49 f6a3 d315  ...H...}...I....
-000002e0: 0832 0d3b 3a9d 58ce 767c f6c4 ed9f 8cca  .2.;:.X.v|......
-000002f0: da74 346d 1ae0 e3f1 7838 b6cb d28b 701c  .t4m....x8....p.
-00000300: 04e0 51bb 9ec2 9df4 6cbf a441 09b4 a369  ..Q.....l..A...i
-00000310: d064 d8f6 daae 91a6 aa8d 534f d3f7 7ddf  .d........SO..}.
-00000320: eb9b 689c 0a8d 5b4f d36b 77dd d38e 89c6  ..h...[O.kw.....
-00000330: add0 780d bef1 4f87 c3ae 89c6 abd0 74eb  ..x...O.......t.
-00000340: 6926 27fd ae6b a4e9 1668 4246 e3eb 7a12  i&'..k...hBF..z.
-00000350: 15b5 e540 d320 0058 7076 d6cc d203 965e  ...@. .Xpv.....^
-00000360: 29fa 7594 1ad9 1dbb dd41 5cf0 58ee 3989  ).u......A\.X.9.
-00000370: 11fe c6c5 04d6 69d2 1996 3446 729d 9005  ......i...4Fr...
-00000380: 0e00 37c4 d14c 507c af41 b68a e0c2 92d2  ..7..LP|.A......
-00000390: 5c90 d6cf 29b5 501a 089a c881 f547 8221  \...).P......G.!
-000003a0: c5dc affd f597 bbc9 a433 7a9d 7d3a ce6b  .........3z.}:.k
-000003b0: 947f 69ab 01a7 edbb 9bcf 93fc 73e8 e49f  ..i.........s...
-000003c0: a793 d74d 42ce 70bc 2c09 f1fb 235b 6187  ...MB.p.,...#[a.
-000003d0: 276e 3b13 723a 1c67 427c cff6 f691 a525  'n;.r:.gB|.....%
-000003e0: 32cf eff9 0aeb 4e3c 671f 5696 b05d cfcf  2.....N<g.V..]..
-000003f0: e49e 8c72 23bb ddf6 587d f64f 476e 23d7  ...r#...X}.OGn#.
-00000400: a9c0 b322 d794 4624 459f c82d bae4 1138  ..."..F$E..-...8
-00000410: b549 0d32 133f 089d 8698 6a50 1c02 a409  .I.2.?....jP....
-00000420: 3196 a186 f8b4 c6ac 11e0 137d b7be 08c8  1..........}....
-00000430: df8d 88f7 ab6f 9a3d 57a1 5849 da84 f810  .....o.=W.XI....
-00000440: 461a e29c 73e6 73d1 6cfb 07a5 46d1 f655  F...s.s.l...F..U
-00000450: bcdc a397 5815 0197 18df 34aa 352c c5d6  ....X.....4.5,..
-00000460: 7895 c0f1 ad9c 3c1d 1312 cd94 0b06 4186  x.....<.......A.
-00000470: 9724 2612 a939 7e4d 4813 fe2b a5da fe9c  .$&..9~MH..+....
-00000480: d340 f094 2f24 fa4a 918f 69b3 23a7 7426  .@../$.J..i.#.t&
-00000490: cde8 331a c146 af1b 7587 68d2 3c7a fe05  ..3..F..u.h.<z..
-000004a0: f99c 350a 1c91 1b1d 0267 1bb3 4621 8469  ..5......g..F!.i
-000004b0: bbf0 1eaf 248e 9aad c211 2b42 3e62 1936  ....$.....+B>b.6
-000004c0: 1a72 b516 81b6 71a9 8460 5a12 c6d1 784e  .r....q..`Z...xN
-000004d0: d2b4 11fc 59ac 3593 3e60 c8ec cd91 75ce  ....Y.5.>`....u.
-000004e0: d691 0e11 925e 3742 3e62 ce8b 9011 bf1e  .....^7B>b......
-000004f0: 8638 4a9a eda2 7158 04fd 9e5e c349 c1e8  .8J...qX...^.I..
-00000500: 82cb 66fd b87e 86d5 336c 2c8e f747 d417  ..f..~..3l,..G..
-00000510: 4ae4 0f26 a73f e932 3407 a39a 5909 bd84  J..&.?.24...Y...
-00000520: 566a 9faa 8734 3ea8 1e32 0a05 f1b9 1e3e  Vj...4>..2.....>
-00000530: e57a 780a 3796 c6bc 50ae 827b 01ff d1da  .zx.7...P..{....
-00000540: 37c2 abf8 82c0 397f 2e7d cfa5 efb9 f43d  7.....9..}.....=
-00000550: a1d2 b737 237d 67c1 d38b 5bde 466e 5bc4  ...7#}g...[.Fn[.
-00000560: fbae 31da d734 2e28 6357 72cd c8c7 54af  ..1..4.(cWr...T.
-00000570: 9329 d839 9fc0 ecfd 683e 9ef1 edfa d924  .).9....h>.....$
-00000580: 84af 9a59 2d23 1690 4b81 b341 24b8 fc8b  ...Y-#..K..A$...
-00000590: caf0 2ac4 09e8 645b 2509 cb54 d365 378a  ..*...d[%..T.e7.
-000005a0: 129e 421b 6ee9 53f5 4a95 d7e5 afb9 28b8  ..B.n.S.J.....(.
-000005b0: 3c5b e4e9 afa1 743e 2ccf f93c 5fe7 b4cd  <[....t>,..<_...
-000005c0: 0b33 43b7 724b eab6 94be b526 384a f4b1  .3C.rK.....&8J..
-000005d0: cc70 4e1e cb0c 3b67 3c92 1db6 77a0 1d35  .pN...;g<...w..5
-000005e0: fbf6 5d76 e423 a530 5397 43b8 1a42 be03  ..]v.#.0S.C..B..
-000005f0: 6dba 9ddc 3a38 9e98 91b9 0ad3 5290 6fc3  m...:8......R.o.
-00000600: f9e9 c578 1ae2 39d9 04b9 7d98 576d e7d8  ...x..9...}.Wm..
-00000610: d1d1 fbe7 c151 b0a3 ef3c 961d c788 f2a2  .....Q...<......
-00000620: 21ee a186 98cf c343 8779 7b5f 9867 95c6  !......C.y{_.g..
-00000630: 5034 146d 6cac 242c 46b7 60b8 d7f1 2c14  P4.ml.$,F.`...,.
-00000640: e064 602d a007 83af 5102 f252 5560 315b  .d`-....Q..RU`1[
-00000650: c603 2b90 a27c 4c8c 45e8 70e7 975c 5fe3  ..+..|L.E.p..\_.
-00000660: d192 e3db a665 b56e af29 7719 6d22 5239  .....e.n.)w.m"R9
-00000670: c269 9813 67ab cade 65b1 c155 1dcf 555b  .i..g...e..U..U[
-00000680: f2b0 be6a 3db4 154e cffe 59ad c89f 0c11  ...j=..N..Y.....
-00000690: 4e16 0b12 4863 9417 a64a a2f3 1953 bee7  N...Hc...J...S..
-000006a0: 2b49 c455 38bf 4533 b612 9718 bce3 e6c7  +I.U8.E3........
-000006b0: 714e 53b8 1276 b60f 0232 b9bb 39a9 7a65  qNS..v...2..9.ze
-000006c0: 3167 a6f2 df2d 0c09 2c5b 8859 12e2 4d5d  1g...-..,[.Y..M]
-000006d0: edd5 e79b 9cae 7a22 76fa 9777 c160 f2fd  ......z"v..w.`..
-000006e0: 70c9 470f e53b e75f f45d 43ae 7ef6 dde3  p.G..;._.]C.~...
-000006f0: fa6e 933b 484c 9c79 c511 0174 4502 2395  .n.;HL.y...tE.#.
-00000700: 1c06 1617 32e4 50ee 9290 0613 01cd 94c9  ....2.P.........
-00000710: 44f0 0282 64a6 1c80 98fa 0bbd f20c b929  D...d..........)
-00000720: 15ce ad3e 397f 452c 8386 4e5e d225 1214  ...>9.E,..N^.%..
-00000730: 8ab0 0c05 2117 72e3 efef 936a 778c d7fa  ....!.r....jw...
-00000740: 2c81 6d84 5432 64d5 17ca 4389 c13d 3372  ,.m.T2d...C..=3r
-00000750: 43d8 5425 f3ae da26 0b85 dbe2 54cd bb1a  C.T%...&....T...
-00000760: be26 604b c37a 6e9d 2d27 ffdb 5ed4 3db4  .&`K.zn.-'..^.=.
-00000770: 173d 46f3 a399 e01e b387 739b 7ab8 c245  .=F.......s.z..E
-00000780: acff 58d6 1ef9 32df 3970 db3a de03 5ee6  ..X...2.9p.:..^.
-00000790: 132c 43a4 7ec1 7d8a 8a80 11ab 62be baaf  .,C.~.}.....b...
-000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
-000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
-000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
-000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
-000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
-000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
-00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
-00000810: 0304 1400 0000 0800 e54e 6856 695e 91e4  .........NhVi^..
-00000820: 7101 0000 3003 0000 1800 0000 786c 2f77  q...0.......xl/w
-00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00000840: 2e78 6d6c 8593 c14e c330 0c86 5fa5 ca03  .xml...N.0.._...
-00000850: 900e 6980 505b 0906 131c 9026 d0e0 88b2  ..i.P[.....&....
-00000860: d65d a325 7570 5c0a 6f4f d2ad d390 26f5  .].%up\.oO....&.
-00000870: 54db f1f7 db4e dcac 47da f906 8093 1f6b  T....N..G......k
-00000880: 5a9f 8b86 d9dd 4ae9 cb06 acf2 17e8 a00d  Z.....J.........
-00000890: 2735 9255 1c5c da4a ef08 5435 40d6 c8cb  '5.U.\.J..T5@...
-000008a0: 34bd 9256 e956 14d9 105b 5191 61c7 46b7  4..V.V...[Q.a.F.
-000008b0: b0a2 c477 d62a fabd 0783 7d2e 6662 0cbc  ...w.*....}.fb..
-000008c0: ea6d c331 208b cca9 2dbc 01af dd8a 8227  .m.1 ...-......'
-000008d0: 8f2a 95b6 d07a 8d6d 4250 e7e2 6e76 bb1c  .*...z.mBP..nv..
-000008e0: f287 8477 0dbd 3fb1 9338 c906 7117 9de7  ...w..?..8..q...
-000008f0: 2a17 696c 080c 941c 1554 f87c c302 8c89  *.il.....T.|....
-00000900: 42a1 8daf 83a6 3896 8ce0 a93d aa2f 87d9  B.....8....=./..
-00000910: c32c 1be5 6181 e643 57dc e4e2 4624 15d4  .,..a..CW...F$..
-00000920: aa33 fc8a fd13 1ce6 991f 1b7c 50ac 8a8c  .3.........|P...
-00000930: b04f 28ce 5964 6534 62ed 90a7 db78 3f6f  .O(.Yde4b....x?o
-00000940: 4c21 ae43 212e 9c72 409f 9fba ca24 872e  L!.C!..r@....$..
-00000950: 6250 9607 e87e 0262 cd06 ce70 8b09 4e75  bP...~.b...p..Nu
-00000960: dc20 f933 e4c3 04e9 aa7a 4de6 0cf8 3801  . .3.....zM...8.
-00000970: 7ea3 e9ec b95e 9713 a007 1f57 e13f 29c3  ~....^.....W.?).
-00000980: f58e 4fb6 bfef b84b 2f8a b6ba f589 813a  ..O....K/......:
-00000990: 28a6 17d7 7391 d0fe 7df6 0ea3 1b76 7183  (...s...}....vq.
-000009a0: cc68 07b3 092b 0d14 13c2 798d c8a3 13d7  .h...+....y.....
-000009b0: e3f8 9314 7f50 4b03 0414 0000 0008 00e5  .....PK.........
-000009c0: 4e68 5639 d0d6 e84c 0100 0052 0200 0018  NhV9...L...R....
-000009d0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-000009e0: 2f73 6865 6574 322e 786d 6c85 52cb 4ec3  /sheet2.xml.R.N.
-000009f0: 3010 fc95 c81f 50a7 4805 5425 9168 1182  0.....P.H.T%.h..
-00000a00: 0352 d50a 3856 6eb2 49ac dade 606f 1af8  .R..8Vn.I...`o..
-00000a10: 7bbc 6953 212e 9cb2 af99 9d59 271b d01f  {.iS!......Y'...
-00000a20: 430b 40c9 9735 2ee4 a225 ea96 5286 b205  C.@..5...%..R...
-00000a30: abc2 0c3b 70b1 53a3 b78a 62ea 1b19 3a0f  ...;p.S...b...:.
-00000a40: aa1a 41d6 c89b 34bd 9556 6927 8a6c ac6d  ..A...4..Vi'.l.m
-00000a50: 7c91 614f 463b d8f8 24f4 d62a ffbd 0283  |.aOF;..$..*....
-00000a60: 432e e662 2a6c 75d3 1217 6491 75aa 811d  C..b*lu...d.u...
-00000a70: d05b b7f1 3193 5796 4a5b 7041 a34b 3cd4  .[..1.W.J[pA.K<.
-00000a80: b978 982f 57e3 fc38 f0ae 6108 bfe2 849d  .x./W..8..a.....
-00000a90: 1c10 8f9c bc54 b948 5910 1828 8919 54fc  .....T.HY..(..T.
-00000aa0: 9c60 0dc6 3051 94f1 79e1 14d7 950c fc1d  .`..0Q..y.......
-00000ab0: 4fec 4fa3 f7e8 e5a0 02ac d17c e88a da5c  O.O........|...\
-00000ac0: dc8b a482 5af5 86b6 383c c3c5 cfe2 2af0  ....Z...8<....*.
-00000ad0: 5191 2a32 8f43 e2d9 6791 951c f0ee 38a7  Q.*2.C..g.....8.
-00000ae0: 1ddf 6747 3ed6 755c 4445 80c0 56f7 7bd2  ..gG>.u\DE..V.{.
-00000af0: 6420 9314 a570 4796 17e4 ea5f e409 4d6f  d ...pG...._..Mo
-00000b00: ff40 6514 3099 3a2b e26b bf2a df68 1712  .@e.0.:+.k.*.h..
-00000b10: 0375 a44c 6777 0b91 f8b3 8373 42d8 8daf  .u.Lgw.....sB...
-00000b20: 7540 22b4 63d8 c647 07cf 03b1 5f23 d294  u@".c..G...._#..
-00000b30: f001 afbf 51f1 0350 4b03 0414 0000 0008  ....Q..PK.......
-00000b40: 00e5 4e68 561f 23f7 674c 0100 0050 0200  ..NhV.#.gL...P..
-00000b50: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00000b60: 7473 2f73 6865 6574 332e 786d 6c85 52cb  ts/sheet3.xml.R.
-00000b70: 4ec3 3010 fc15 cb1f 50a7 4805 5425 9168  N.0.....P.H.T%.h
-00000b80: 1182 0352 d50a 3856 4eb2 49ac dade 606f  ...R..8VN.I...`o
-00000b90: 1af8 7bec b489 e0c4 29fb 9ad9 9975 d201  ..{.....)....u..
-00000ba0: ddc9 b700 c4be 8cb6 3ee3 2d51 b716 c297  ........>.-Q....
-00000bb0: 2d18 e917 d881 0d9d 1a9d 9114 52d7 08df  -...........R...
-00000bc0: 3990 d508 325a dc24 c9ad 3052 599e a763  9...2Z.$..0RY..c
-00000bd0: 6de7 f214 7bd2 cac2 ce31 df1b 23dd f706  m...{....1..#...
-00000be0: 340e 195f f2a9 b057 4d4b b120 f2b4 930d  4.._...WMK. ....
-00000bf0: 1c80 deba 9d0b 9998 592a 65c0 7a85 9639  ........Y*e.z..9
-00000c00: a833 feb0 5c6f c6f9 71e0 5dc1 e07f c52c  .3..\o..q.]....,
-00000c10: 3a29 104f 3179 a932 9e44 41a0 a1a4 c820  :).O1y.2.DA.... 
-00000c20: c3e7 0c5b d03a 1205 199f 574e 3eaf 8cc0  ...[.:....WN>...
-00000c30: dff1 c4fe 347a 0f5e 0ae9 618b fa43 55d4  ....4z.^..a..CU.
-00000c40: 66fc 9eb3 0a6a d96b dae3 f00c 573f ab59  f....j.k....W?.Y
-00000c50: e0a3 2499 a70e 07e6 a2cf 3c2d 6310 7787  ..$.......<-c.w.
-00000c60: 3965 e37d 0ee4 425d 8545 949f 51f7 068e  9e.}..B].E..Q...
-00000c70: 47db 9b02 5c2a 2848 891d 515e 919b ff90  G...\*(H..Q^....
-00000c80: a448 c35f a008 eb27 4b17 3df1 d6af d235  .H._...'K.=....5
-00000c90: ca7a a6a1 0e84 c9e2 6ec5 99bb e8bf 2484  .z......n.....$.
-00000ca0: ddf8 5605 12a1 19c3 363c 39b8 3810 fa35  ..V.....6<9.8..5
-00000cb0: 224d 493c dffc 13e5 3f50 4b03 0414 0000  "MI<....?PK.....
-00000cc0: 0008 00e5 4e68 567c f3a3 dc51 0200 00f6  ....NhV|...Q....
-00000cd0: 0900 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
-00000ce0: 2e78 6d6c dd56 db8a db30 10fd 15e1 0fa8  .xml.V...0......
-00000cf0: 9398 3571 49f2 5043 60a1 2d0b bb0f 7d55  ..5qI.PC`.-...}U
-00000d00: 6239 11e8 e2ca f292 f4eb 3b23 3976 b3ab  b9........;#9v..
-00000d10: 5928 7dab 4df0 cc1c 9db9 1b67 d3fb ab12  Y(}.M......g....
-00000d20: cf67 213c bb68 65fa 6d76 f6be fb9c e7fd  .g!<.he.mv......
-00000d30: f12c 34ef 3fd9 4e18 405a eb34 f7a0 ba53  .,4.?.N.@Z.4...S
-00000d40: de77 4ef0 a647 9256 f96a b128 73cd a5c9  .wN..G.V.j.(s...
-00000d50: 761b 33e8 bdf6 3d3b dac1 f86d b6c8 f2dd  v.3...=;...m....
-00000d60: a6b5 66b6 2cb3 6880 a35c 0bf6 cad5 36ab  ..f.,.h..\....6.
-00000d70: b992 0727 c359 aea5 ba46 f30a 0d47 abac  ...'.Y...F...G..
-00000d80: 631e 5211 4806 4bff 2bc2 cba8 6196 a31f  c.R.H.K.+...a...
-00000d90: 2d8d 7568 cc63 84f0 e8c1 a954 6a4a 6095  -.uh.c.....TjJ`.
-00000da0: 45c3 6ed3 71ef 8533 7b50 0227 18df 416c  E.n.q..3{P.'..Al
-00000db0: 945f ae1d 6470 72fc ba5c 3d64 3321 3c20  ._..dpr..\=d3!< 
-00000dc0: c8c1 ba46 b8bb 3aa3 69b7 51a2 f540 70f2  ...F..:.i.Q..@p.
-00000dd0: 74c6 a7b7 5d8e a0f7 5683 d048 7eb2 8687  t...]...V..H~...
-00000de0: 1c6e 8c51 00b7 47a1 d433 8ee8 477b e7fb  .n.Q..G..3..G{..
-00000df0: d2b2 d8eb c706 dbcc b0d4 9b08 098d 6274  ..............bt
-00000e00: 1315 f4ff a7b7 e8fb 9fdd b24e be5a ff65  ...........N.Z.e
-00000e10: 806a 4cd0 7f0e d68b 2727 5a79 09fa a5bd  .jL.....''Zy....
-00000e20: 8f3f 850e 89dc 459f ac0c 9763 9b7d c79d  .?....E....c.}..
-00000e30: 53b3 0b76 18a4 f2d2 8cda 5936 8d30 ef6a  S..v......Y6.0.j
-00000e40: 03f7 9e1f 60a9 effc c3f9 46b4 7c50 fe65  ....`.....F.|P.e
-00000e50: 02b7 d92c 7f13 8d1c 7435 9d7a c2b2 c653  ...,....t5.z...S
-00000e60: b3fc 1567 b82c a7cd 8458 d234 e222 9a7a  ...g.,...X.4.".z
-00000e70: 54dd e910 4406 0244 1d2f 24bc 45f6 e14a  T...D..D./$.E..J
-00000e80: 2314 2762 6904 312a 0e95 01c5 892c 2ace  #.'bi.1*.....,*.
-00000e90: ff54 cf9a ac27 6254 6eeb 24b2 2639 6b92  .T...'bTn.$.&9k.
-00000ea0: 1359 29a4 0e37 1527 cda9 e04a 575a 5545  .Y)..7.'...JWZUE
-00000eb0: 5196 5447 eb3a 9941 4df5 ad2c f197 f646  Q.TG.:.AM..,...F
-00000ec0: e586 0c2a 0e46 fabb 5ed3 d3a6 37e4 e33d  ...*.F..^...7..=
-00000ed0: a066 fad1 8650 95d2 9b48 554a f71a 9174  .f...P...HUJ...t
-00000ee0: df90 5155 e969 5371 9041 4d81 da1d 8c9f  ..QU.iSq.AM.....
-00000ef0: 8e83 3b95 e614 054e 95ca 8d7a 8369 a4aa  ..;....N...z.i..
-00000f00: 2804 7731 bda3 6549 74a7 c43b 3d1f ea2d  (.w1..eIt..;=..-
-00000f10: 298a aa4a 2388 a533 280a 0ac1 b791 46a8  )..J#..3(.....F.
-00000f20: 0c30 070a 298a f01d 7cf3 3dca 6fdf a97c  .0..)...|.=.o..|
-00000f30: fea7 b7fb 0d50 4b03 0414 0000 0008 00e5  .....PK.........
-00000f40: 4e68 5697 8abb 1cc0 0000 0013 0200 000b  NhV.............
-00000f50: 0000 005f 7265 6c73 2f2e 7265 6c73 9d92  ..._rels/.rels..
-00000f60: b96e c330 0c40 7fc5 d09e 3007 d021 8833  .n.0.@....0..!.3
-00000f70: 65f1 1604 f901 56a2 0fd8 1205 8a45 9dbf  e.....V......E..
-00000f80: afda a571 900b 1979 3d3c 12dc 1e69 40ed  ...q...y=<...i@.
-00000f90: 38a4 b68b a918 fd10 5269 5ad5 b801 48b6  8.......RiZ...H.
-00000fa0: 258f 69ce 9142 aed4 2c1e 3587 d240 44db  %.i..B..,.5..@D.
-00000fb0: 6343 b05a 2c3e 402e 1966 b7bd 6416 a773  cC.Z,>@..f..d..s
-00000fc0: a457 885c d79d a53d db2f 4f41 6f80 af3a  .W.\...=./OAo..:
-00000fd0: 4c71 4269 484b 330e f0cd d27f 32f7 f30c  LqBiHK3.....2...
-00000fe0: 3545 e54a 2395 5b1a 78d3 e5fe 76e0 49d1  5E.J#.[.x...v.I.
-00000ff0: a122 5816 9a45 c9d3 a21d a57f 1dc7 f690  ."X..E..........
-00001000: d3e9 af63 22b4 7a5b e8f9 7168 540a 8edc  ...c".z[..qhT...
-00001010: 6325 8c71 62b4 fe35 82c9 0fec 7e00 504b  c%.qb..5....~.PK
-00001020: 0304 1400 0000 0800 e54e 6856 6c20 24ba  .........NhVl $.
-00001030: 5501 0000 3b03 0000 0f00 0000 786c 2f77  U...;.......xl/w
-00001040: 6f72 6b62 6f6f 6b2e 786d 6cb5 9251 4bc3  orkbook.xml..QK.
-00001050: 400c c7bf 4ab9 0f60 bb4e 070e bb17 873a  @...J..`.N.....:
-00001060: 101d 4ef6 7e6d d335 ecee 5272 d74d f7e9  ..N.~m.5..Rr.M..
-00001070: 4d3b 8a05 61f8 b2a7 6bfe 09e9 2fff e4e1  M;..a...k.../...
-00001080: 48bc cf89 f6d1 9735 ce67 aa0e a199 c7b1  H......5.g......
-00001090: 2f6a b0da df50 034e 3215 b1d5 4142 dec5  /j...P.N2...AB..
-000010a0: be61 d0a5 af01 8235 719a 24b3 d86a 746a  .a.....5q.$..jtj
-000010b0: f130 f45a 733c 0e28 4011 909c 889d b045  .0.Zs<.(@......E
-000010c0: 38fa df7c 1746 07f4 98a3 c1f0 9da9 fedb  8..|.F..........
-000010d0: 808a 2c3a b478 8232 5389 8a7c 4dc7 1762  ..,:.x.2S..|M..b
-000010e0: 3c91 0bda 6c0a 2663 3235 3927 b6c0 018b  <...l.&c259'....
-000010f0: 3ff2 a683 fcd4 b9ef 95a0 f30f 2d20 999a  ?...........- ..
-00001100: 25d2 b042 f6a1 afe8 fb6b 613c 8014 672a  %..B.....ka<..g*
-00001110: 95a8 0df4 8426 002f 7580 67a6 b641 b7eb  .....&./u.g..A..
-00001120: dac8 14f1 688c de87 e13d 9b38 e7ff d848  ....h....=.8...H
-00001130: 5585 052c a968 2db8 70f6 91c1 7480 ced7  U..,.h-.p...t...
-00001140: d878 1539 6d21 536b dd00 77f3 c80f 56e5  .x.9m!Sk..w...V.
-00001150: 79b6 2050 23a7 788e 92e0 55d9 e35d 0f65  y. P#.x...U..].e
-00001160: 03de 8b36 8249 2fc0 a4d7 85d9 9291 9211  ...6.I/.........
-00001170: cbf4 02cb b4df dbb0 ac12 2a74 50be 491f  ..........*tP.I.
-00001180: 2fba 1c4e b1e6 a87b 7a83 d3db bbc9 bd1c  /..N...{z.......
-00001190: 486b cca3 68ef ee95 7439 ec7e b8db c50f  Hk..h...t9.~....
-000011a0: 504b 0304 1400 0000 0800 e54e 6856 bb6c  PK.........NhV.l
-000011b0: eaec ba00 0000 1a03 0000 1a00 0000 786c  ..............xl
-000011c0: 2f5f 7265 6c73 2f77 6f72 6b62 6f6f 6b2e  /_rels/workbook.
-000011d0: 786d 6c2e 7265 6c73 c593 390e 8330 1045  xml.rels..9..0.E
-000011e0: af82 7c00 8625 4911 0155 1ada 880b 5830  ..|..%I..U....X0
-000011f0: 2c62 b1e5 9928 70fb 1028 c052 8a34 88ca  ,b...(p..(.R.4..
-00001200: fa63 f9fd 578c a327 7692 1b35 50dd 6872  .c..W..'v..5P.hr
-00001210: c6be 1b28 1635 b3be 0350 5e63 2fc9 551a  ...(.5...P^c/.U.
-00001220: 87f9 a654 a697 3c47 5381 9679 2b2b 84c0  ...T..<GS..y++..
-00001230: f36e 60f6 0c91 447b a693 4d1a ff21 aab2  .n`...D{..M..!..
-00001240: 6c72 7ca8 fcd5 e3c0 3fc0 f056 a6a5 1a91  lr|.....?..V....
-00001250: 8593 4953 21c7 02c6 6e1b 132c 87ef ce64  ..IS!...n..,...d
-00001260: e1a4 452c 4c5a f802 ce16 0a2c a1e0 7ca1  ..E,LZ.....,..|.
-00001270: d012 0a0f 1422 9e3a a4cd 66cd 56fd e5c0  .....".:..f.V...
-00001280: 7a9e dfe2 d6be c475 682f c9f5 eb00 d657  z......uh/.....W
-00001290: 483e 504b 0304 1400 0000 0800 e54e 6856  H>PK.........NhV
-000012a0: a6fc 4a5b 2301 0000 df04 0000 1300 0000  ..J[#...........
-000012b0: 5b43 6f6e 7465 6e74 5f54 7970 6573 5d2e  [Content_Types].
-000012c0: 786d 6ccd 94cf 4ec3 300c c65f a5ea 756a  xml...N.0.._..uj
-000012d0: 3286 c401 adbb 0057 d881 1708 8dbb 46cd  2......W......F.
-000012e0: 3fc5 dee8 de1e b7dd 2681 46c5 3424 b834  ?.......&.F.4$.4
-000012f0: 6a6c 7f3f c79f 92e5 eb3e 0266 9db3 1ecb  jl.?.....>.f....
-00001300: bc21 8af7 5262 d580 5328 4204 cf91 3a24  .!..Rb..S(B...:$
-00001310: a788 7fd3 4646 55b5 6a03 7231 9fdf c92a  ....FFU.j.r1...*
-00001320: 7802 4f05 f51a f96a f908 b5da 5aca 9e3a  x.O....j....Z..:
-00001330: de46 137c 9927 b098 670f 6362 cf2a 7315  .F.|.'..g.cb.*s.
-00001340: a335 9522 8ecb 9dd7 5f28 c581 20b8 72c8  .5."...._(.. .r.
-00001350: c1c6 449c 7142 2ecf 12fa c8f7 8043 ddcb  ..D.qB.......C..
-00001360: 0e52 321a b2b5 4af4 ac1c 67c9 ce4a a4bd  .R2...J...g..J..
-00001370: 0514 d312 677a 0c75 6d2a d0a1 da3a 2e11  ....gz.um*...:..
-00001380: 1813 288d 0d00 392b 46d1 d934 9978 c230  ..(...9+F..4.x.0
-00001390: 7e6f aee6 0f32 5340 ce5c a710 911d 4b70  ~o...2S@.\....Kp
-000013a0: 39ee 6849 5f5d 4416 8244 66fa 8827 224b  9.hI_]D..Df..'"K
-000013b0: 5f7d 3ee8 ddd6 a07f c8e6 f1be 87d4 0e7e  _}>............~
-000013c0: a01c 96eb 67fc d9e3 93fe 857d 2cfe 491f  ....g......},.I.
-000013d0: b77f d8c7 5b08 ed6f 5fb9 7e15 4e19 7fe4  ....[..o_.~.N...
-000013e0: cbe1 5d5b 7d00 504b 0102 1403 1400 0000  ..][}.PK........
-000013f0: 0800 e54e 6856 0741 4d62 8100 0000 b100  ...NhV.AMb......
-00001400: 0000 1000 0000 0000 0000 0000 0000 8001  ................
-00001410: 0000 0000 646f 6350 726f 7073 2f61 7070  ....docProps/app
-00001420: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00001430: e54e 6856 fbf6 23b2 ef00 0000 2b02 0000  .NhV..#.....+...
-00001440: 1100 0000 0000 0000 0000 0000 8001 af00  ................
-00001450: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
-00001460: 786d 6c50 4b01 0214 0314 0000 0008 00e5  xmlPK...........
-00001470: 4e68 5699 5c9c 2310 0600 009c 2700 0013  NhV.\.#.....'...
-00001480: 0000 0000 0000 0000 0000 0080 01cd 0100  ................
-00001490: 0078 6c2f 7468 656d 652f 7468 656d 6531  .xl/theme/theme1
+000000e0: c14a c430 1086 5f45 726f 2749 6191 d0cd  .J.0.._Ero'Ia...
+000000f0: 45f1 a420 b8a0 780b c9ec 6eb0 4943 32d2  E.. ..x...n.IC2.
+00000100: eedb dbd6 dd2e a20f e031 337f bef9 06a6  .........13.....
+00000110: b549 d93e e373 ee13 66f2 586e c6d0 c5a2  .I.>.s..f.Xn....
+00000120: 6cda b223 5152 00c5 1e31 9852 4f89 3835  l..#QR...1.RO.85
+00000130: f77d 0e86 a667 3e40 32f6 c31c 1024 e71b  .}...g>@2....$..
+00000140: 0848 c619 3230 03ab b412 996e 9d55 36a3  .H..20.....n.U6.
+00000150: a13e 9ff1 ceae f8f4 99bb 05e6 2c60 8701  .>..........,`..
+00000160: 2315 10b5 00a6 e789 e934 762d 5c01 338c  #........4v-\.3.
+00000170: 3087 f25d 40b7 1297 ea9f d8a5 03ec 9c1c  0..]@...........
+00000180: 8b5f 53c3 30d4 43b3 e4a6 1d04 bc3d 3dbe  ._S.0.C......==.
+00000190: 2ceb 563e 1632 d1e2 f4ab 7845 a784 5b76  ,.V>.2....xE..[v
+000001a0: 99fc dadc ddef 1e98 965c 3615 6f2a d9ec  .........\6.o*..
+000001b0: f846 c95b 25c4 fbec fac3 ef2a 1c7a e7f7  .F.[%......*.z..
+000001c0: fe1f 1b5f 0475 0bbf ee42 7f01 504b 0304  ..._.u...B..PK..
+000001d0: 1400 0000 0800 853b 7756 995c 9c23 1006  .......;wV.\.#..
+000001e0: 0000 9c27 0000 1300 0000 786c 2f74 6865  ...'......xl/the
+000001f0: 6d65 2f74 6865 6d65 312e 786d 6ced 5a5b  me/theme1.xml.Z[
+00000200: 73da 3814 7eef afd0 7867 f66d 0bc6 3681  s.8.~...xg.m..6.
+00000210: b6b4 1373 6976 dbb4 9984 ed4e 1f85 1158  ...siv.....N...X
+00000220: 8d6c 7964 9184 7fbf 4736 10cb 960d ed92  .lyd....G6......
+00000230: 4dba 9b3c 042c e9fb ce45 47e7 e838 79f3  M..<.,...EG..8y.
+00000240: ee2e 62e8 8688 94f2 7860 d92f dbd6 bbb7  ..b.....x`./....
+00000250: 2fde e057 3224 1141 3019 a7af f0c0 0aa5  /..W2$.A0.......
+00000260: 4c5e b55a 6900 c338 7dc9 1312 c3dc 828b  L^.Zi..8}.......
+00000270: 084b 7814 cbd6 5ce0 5b1a 2f23 d6ea b4db  .Kx...\.[./#....
+00000280: dd56 8469 6ca1 1847 6460 7d5e 2c68 40d0  .V.il..Gd`}^,h@.
+00000290: 5451 5a6f 5f20 b4e5 1f33 f815 cb54 8d65  TQZo_ ...3...T.e
+000002a0: a301 1357 4126 b988 b4f2 f96c c5fc dade  ...WA&.....l....
+000002b0: 3e65 cfe9 3a1d 3281 6e30 1b58 207f ce6f  >e..:.2.n0.X ..o
+000002c0: a7e4 4e5a 88e1 54c2 c4c0 6a67 3f56 6bc7  ..NZ..T...jg?Vk.
+000002d0: d1d2 4880 82c9 7d94 05ba 49f6 a3d3 1508  ..H...}...I.....
+000002e0: 320d 3b3a 9d58 ce76 7cf6 c4ed 9f8c cada  2.;:.X.v|.......
+000002f0: 7434 6d1a e0e3 f178 38b6 cbd2 8b70 1c04  t4m....x8....p..
+00000300: e051 bb9e c29d f46c bfa4 4109 b4a3 69d0  .Q.....l..A...i.
+00000310: 64d8 f6da ae91 a6aa 8d53 4fd3 f77d dfeb  d........SO..}..
+00000320: 9b68 9c0a 8d5b 4fd3 6b77 ddd3 8e89 c6ad  .h...[O.kw......
+00000330: d078 0dbe f14f 87c3 ae89 c6ab d074 eb69  .x...O.......t.i
+00000340: 2627 fdae 6ba4 e916 6842 46e3 eb7a 1215  &'..k...hBF..z..
+00000350: b5e5 40d3 2000 5870 76d6 ccd2 0396 5e29  ..@. .Xpv.....^)
+00000360: fa75 941a d91d bbdd 415c f058 ee39 8911  .u......A\.X.9..
+00000370: fec6 c504 d669 d219 9634 4672 9d90 050e  .....i...4Fr....
+00000380: 0037 c4d1 4c50 7caf 41b6 8ae0 c292 d25c  .7..LP|.A......\
+00000390: 90d6 cf29 b550 1a08 9ac8 81f5 4782 21c5  ...).P......G.!.
+000003a0: dcaf fdf5 97bb c9a4 337a 9d7d 3ace 6b94  ........3z.}:.k.
+000003b0: 7f69 ab01 a7ed bb9b cf93 fc73 e8e4 9fa7  .i.........s....
+000003c0: 93d7 4d42 ce70 bc2c 09f1 fb23 5b61 8727  ..MB.p.,...#[a.'
+000003d0: 6e3b 1372 3a1c 6742 7ccf f6f6 91a5 2532  n;.r:.gB|.....%2
+000003e0: cfef f90a eb4e 3c67 1f56 96b0 5dcf cfe4  .....N<g.V..]...
+000003f0: 9e8c 7223 bbdd f658 7df6 4f47 6e23 d7a9  ..r#...X}.OGn#..
+00000400: c0b3 22d7 9446 2445 9fc8 2dba e411 38b5  .."..F$E..-...8.
+00000410: 490d 3213 3f08 9d86 986a 501c 02a4 0931  I.2.?....jP....1
+00000420: 96a1 86f8 b4c6 ac11 e013 7db7 be08 c8df  ..........}.....
+00000430: 8d88 f7ab 6f9a 3d57 a158 49da 84f8 1046  ....o.=W.XI....F
+00000440: 1ae2 9c73 e673 d16c fb07 a546 d1f6 55bc  ...s.s.l...F..U.
+00000450: dca3 9758 1501 9718 df34 aa35 2cc5 d678  ...X.....4.5,..x
+00000460: 95c0 f1ad 9c3c 1d13 12cd 940b 0641 8697  .....<.......A..
+00000470: 2426 12a9 397e 4d48 13fe 2ba5 dafe 9cd3  $&..9~MH..+.....
+00000480: 40f0 942f 24fa 4a91 8f69 b323 a774 26cd  @../$.J..i.#.t&.
+00000490: e833 1ac1 46af 1b75 8768 d23c 7afe 05f9  .3..F..u.h.<z...
+000004a0: 9c35 0a1c 911b 1d02 671b b346 2184 69bb  .5......g..F!.i.
+000004b0: f01e af24 8e9a adc2 112b 423e 6219 361a  ...$.....+B>b.6.
+000004c0: 72b5 1681 b671 a984 605a 12c6 d178 4ed2  r....q..`Z...xN.
+000004d0: b411 fc59 ac35 933e 60c8 eccd 9175 ced6  ...Y.5.>`....u..
+000004e0: 910e 1192 5e37 423e 62ce 8b90 11bf 1e86  ....^7B>b.......
+000004f0: 384a 9aed a271 5804 fd9e 5ec3 49c1 e882  8J...qX...^.I...
+00000500: cb66 fdb8 7e86 d533 6c2c 8ef7 47d4 174a  .f..~..3l,..G..J
+00000510: e40f 26a7 3fe9 3234 07a3 9a59 09bd 8456  ..&.?.24...Y...V
+00000520: 6a9f aa87 343e a81e 320a 05f1 b91e 3ee5  j...4>..2.....>.
+00000530: 7a78 0a37 96c6 bc50 ae82 7b01 ffd1 da37  zx.7...P..{....7
+00000540: c2ab f882 c039 7f2e 7dcf a5ef b9f4 3da1  .....9..}.....=.
+00000550: d2b7 3723 7d67 c1d3 8b5b de46 6e5b c4fb  ..7#}g...[.Fn[..
+00000560: ae31 dad7 342e 2863 5772 cdc8 c754 af93  .1..4.(cWr...T..
+00000570: 29d8 399f c0ec fd68 3e9e f1ed fad9 2484  ).9....h>.....$.
+00000580: af9a 592d 2316 904b 81b3 4124 b8fc 8bca  ..Y-#..K..A$....
+00000590: f02a c409 e864 5b25 09cb 54d3 6537 8a12  .*...d[%..T.e7..
+000005a0: 9e42 1b6e e953 f54a 95d7 e5af b928 b83c  .B.n.S.J.....(.<
+000005b0: 5be4 e9af a174 3e2c cff9 3c5f e7b4 cd0b  [....t>,..<_....
+000005c0: 3343 b772 4bea b694 beb5 2638 4af4 b1cc  3C.rK.....&8J...
+000005d0: 704e 1ecb 0c3b 673c 921d b677 a01d 35fb  pN...;g<...w..5.
+000005e0: f65d 76e4 23a5 3053 9743 b81a 42be 036d  .]v.#.0S.C..B..m
+000005f0: ba9d dc3a 389e 9891 b90a d352 906f c3f9  ...:8......R.o..
+00000600: e9c5 781a e239 d904 b97d 9857 6de7 d8d1  ..x..9...}.Wm...
+00000610: d1fb e7c1 51b0 a3ef 3c96 1dc7 88f2 a221  ....Q...<......!
+00000620: eea1 8698 cfc3 4387 797b 5f98 6795 c650  ......C.y{_.g..P
+00000630: 3414 6d6c ac24 2c46 b760 b8d7 f12c 14e0  4.ml.$,F.`...,..
+00000640: 6460 2da0 0783 af51 02f2 5255 6031 5bc6  d`-....Q..RU`1[.
+00000650: 032b 90a2 7c4c 8c45 e870 e797 5c5f e3d1  .+..|L.E.p..\_..
+00000660: 92e3 dba6 65b5 6eaf 2977 196d 2252 39c2  ....e.n.)w.m"R9.
+00000670: 6998 1367 abca de65 b1c1 551d cf55 5bf2  i..g...e..U..U[.
+00000680: b0be 6a3d b415 4ecf fe59 adc8 9f0c 114e  ..j=..N..Y.....N
+00000690: 160b 1248 6394 17a6 4aa2 f319 53be e72b  ...Hc...J...S..+
+000006a0: 49c4 5538 bf45 33b6 1297 18bc e3e6 c771  I.U8.E3........q
+000006b0: 4e53 b812 76b6 0f02 32b9 bb39 a97a 6531  NS..v...2..9.ze1
+000006c0: 67a6 f2df 2d0c 092c 5b88 5912 e24d 5ded  g...-..,[.Y..M].
+000006d0: d5e7 9b9c ae7a 2276 fa97 77c1 60f2 fd70  .....z"v..w.`..p
+000006e0: c947 0fe5 3be7 5ff4 5d43 ae7e f6dd e3fa  .G..;._.]C.~....
+000006f0: 6e93 3b48 4c9c 79c5 1101 7445 0223 951c  n.;HL.y...tE.#..
+00000700: 0616 1732 e450 ee92 9006 1301 cd94 c944  ...2.P.........D
+00000710: f002 8264 a61c 8098 fa0b bdf2 0cb9 2915  ...d..........).
+00000720: cead 3e39 7f45 2c83 864e 5ed2 2512 148a  ..>9.E,..N^.%...
+00000730: b00c 0521 1772 e3ef ef93 6a77 8cd7 fa2c  ...!.r....jw...,
+00000740: 816d 8454 3264 d517 ca43 89c1 3d33 7243  .m.T2d...C..=3rC
+00000750: d854 25f3 aeda 260b 85db e254 cdbb 1abe  .T%...&....T....
+00000760: 2660 4bc3 7a6e 9d2d 27ff db5e d43d b417  &`K.zn.-'..^.=..
+00000770: 3d46 f3a3 99e0 1eb3 8773 9b7a b8c2 45ac  =F.......s.z..E.
+00000780: ff58 d61e f932 df39 70db 3ade 035e e613  .X...2.9p.:..^..
+00000790: 2c43 a47e c17d 8a8a 8011 ab62 beba af4f  ,C.~.}.....b...O
+000007a0: f925 9c3b b47b f181 209b fcd6 dba4 f6dd  .%.;.{.. .......
+000007b0: e00c 7cd4 ab5a a564 2b11 3f4b 077c 1f92  ..|..Z.d+.?K.|..
+000007c0: 0663 8c5b f434 5f8f 1462 ada6 b1ad c6da  .c.[.4_..b......
+000007d0: 310c 7980 58f3 0ca1 6638 df87 459a 1a33  1.y.X...f8..E..3
+000007e0: d58b ac39 8d0a 6f41 d540 e53f dbd4 0d68  ...9..oA.@.?...h
+000007f0: f60d 341c 9105 5e31 99b6 36a3 e44e 0a3c  ..4...^1..6..N.<
+00000800: dcfe ef0d b0c2 c48e e1ed 8bbf 0150 4b03  .............PK.
+00000810: 0414 0000 0008 0085 3b77 569c 88b2 b791  ........;wV.....
+00000820: 0100 00d1 0300 0018 0000 0078 6c2f 776f  ...........xl/wo
+00000830: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
+00000840: 786d 6c75 53ed 6adc 3010 7c15 a307 887c  xmluS.j.0.|....|
+00000850: 8534 25d8 86e6 9234 0914 8e84 b6bf 657b  .4%....4......e{
+00000860: 7d16 2769 d5d5 ba6e debe 92ef 8350 ac5f  }.'i...n.....P._
+00000870: de5d cdcc eec8 ab6a 463a 8411 808b bfd6  .].....jF:......
+00000880: b850 8b91 d9df 4a19 ba11 ac0a 57e8 c1c5  .P....J.....W...
+00000890: 9301 c92a 8e29 ed65 f004 aa5f 48d6 c84f  ...*.).e..._H..O
+000008a0: 65f9 595a a59d 68aa a5b6 a3a6 c289 8d76  e.YZ..h........v
+000008b0: b0a3 224c d62a 7abf 0383 732d 36e2 5c78  .."L.*z...s-6.\x
+000008c0: d5fb 9153 4136 9557 7b78 03fe e177 1433  ...SA6.W{x...w.3
+000008d0: 7951 e9b5 0517 34ba 8260 a8c5 d7cd edcb  yQ....4..`......
+000008e0: 825f 003f 35cc e143 5c24 272d e221 25cf  ._.?5..C\$'-.!%.
+000008f0: 7d2d ca34 1018 e838 29a8 f8f9 035b 3026  }-.4...8)....[0&
+00000900: 09c5 317e 9f34 c5a5 6522 7e8c cfea 8f8b  ..1~.4..e"~.....
+00000910: f7e8 a555 01b6 687e e99e c75a 7c11 450f  ...U..h~...Z|.E.
+00000920: 839a 0cbf e2fc 0427 3fd7 9701 ef15 aba6  .......'?.......
+00000930: 229c 0b4a 3e9b aa4b 41ea 1d71 daa5 fb79  "..J>..KA..q...y
+00000940: 638a 751d 1b71 e326 db02 5592 e308 a922  c.u..q.&..U...."
+00000950: bb13 e32e c750 1da1 7bb7 2b94 6d8e 32eb  .....P..{.+.m.2.
+00000960: 83ee e35c ba5f 61dd e758 acd9 c00a e121  ...\._a..X.....!
+00000970: 47e8 2174 a47d baf8 15da 638e 3691 5981  G.!t.}....c.6.Y.
+00000980: 7fcb 7651 bc36 d553 16df 1abf 827f cee1  ..vQ.6.S........
+00000990: 0f9b d29b 29ac 505e f20e fe33 2ce3 ff3f  ....).P^...3,..?
+000009a0: efd4 7121 d2b2 7f57 b4d7 2e14 0686 2853  ..q!...W......(S
+000009b0: 5edd 5c8b 828e 0b74 4c18 fdf2 585a 6446  ^.\....tL...XZdF
+000009c0: bb84 637c 7340 0910 cf07 443e 2769 7f2f  ..c|s@....D>'i./
+000009d0: afb8 f907 504b 0304 1400 0000 0800 853b  ....PK.........;
+000009e0: 7756 f502 844e 4601 0000 4002 0000 1800  wV...NF...@.....
+000009f0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00000a00: 7368 6565 7432 2e78 6d6c 7552 d14e c330  sheet2.xmluR.N.0
+00000a10: 0cfc 9528 1f40 3aa4 019a d24a 6c08 c103  ...(.@:....Jl...
+00000a20: d2b4 0978 ce5a b78d 96c4 2571 57f8 7b92  ...x.Z....%qW.{.
+00000a30: 6ead 2624 9e62 5fec f39d 1339 a03f 8616  n.&$.b_....9.?..
+00000a40: 80d8 b735 2ee4 bc25 ea56 4284 b205 abc2  ...5...%.VB.....
+00000a50: 0d76 e0e2 4d8d de2a 8aa9 6f44 e83c a86a  .v..M..*..oD.<.j
+00000a60: 6cb2 46dc 66d9 9db0 4a3b 5ec8 11db fa42  l.F.f...J;^....B
+00000a70: 624f 463b d87a 167a 6b95 ff59 83c1 21e7  bOF;.z.zk..Y..!.
+00000a80: 0b3e 013b ddb4 9400 51c8 4e35 b007 7aef  .>.;....Q.N5..z.
+00000a90: b63e 6662 66a9 b405 1734 3ae6 a1ce f9e3  .>fbf....4:.....
+00000aa0: 62b5 1eeb c782 0f0d 43b8 8a59 7272 403c  b.......C..Yrr@<
+00000ab0: a6e4 b5ca 7996 0481 8192 1283 8ac7 0936  ....y..........6
+00000ac0: 604c 228a 32be 2e9c 7c1e 991a afe3 89fd  `L".2...|.......
+00000ad0: 79f4 1ebd 1c54 800d 9a4f 5d51 9bf3 07ce  y....T...O]Q....
+00000ae0: 2aa8 556f 6887 c30b 5cfc 2c67 814f 8a54  *.Uoh...\.,g.O.T
+00000af0: 213d 0ecc 279f 852c 5390 66c7 3aed d27e  !=..'..,S.f.:..~
+00000b00: f6e4 23ae e320 2a48 9301 2928 2a48 8028  ..#.. *H..)(*H.(
+00000b10: 2f0d ebff 1a4e 687a fba7 43c4 7193 85f3  /....Nhz..C.q...
+00000b20: fcb4 db37 e51b ed02 3350 47a6 ece6 7ec9  ...7....3PG...~.
+00000b30: 993f eb3d 2784 ddf8 3607 2442 3b86 6d7c  .?.='...6.$B;.m|
+00000b40: 62f0 a920 ded7 8834 2569 5df3 a729 7e01  b.. ...4%i]..)~.
+00000b50: 504b 0304 1400 0000 0800 853b 7756 a954  PK.........;wV.T
+00000b60: 77ab 7601 0000 4003 0000 1800 0000 786c  w.v...@.......xl
+00000b70: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00000b80: 7433 2e78 6d6c 7553 db4e c330 0cfd 952a  t3.xmluS.N.0...*
+00000b90: 1fb0 14a4 0142 6d25 18d7 07a4 8969 f09c  .....Bm%.....i..
+00000ba0: 35ee 1a2d a98b e352 f87b 92ee a249 b44f  5..-...R.{...I.O
+00000bb0: b11d 9fe3 63c7 c97a a49d af01 38f9 71b6  ....c..z....8.q.
+00000bc0: f1b9 a899 db5b 297d 5983 537e 862d 34e1  .....[)}Y.S~.-4.
+00000bd0: a642 728a 834b 5be9 5b02 a507 90b3 f232  .Br..K[.[......2
+00000be0: 4daf a453 a611 4536 c496 5464 d8b1 350d  M..S..E6..Td..5.
+00000bf0: 2c29 f19d 738a 7eef c162 9f8b 0b71 0cbc  ,)..s.~..b...q..
+00000c00: 9b6d cd31 208b ac55 5b58 01af db25 054f  .m.1 ..U[X...%.O
+00000c10: 9e58 b471 d078 834d 4250 e5e2 eee2 f679  .X.q.x.MBP.....y
+00000c20: c81f 123e 0cf4 fecc 4e62 271b c45d 745e  ...>....Nb'..]t^
+00000c30: 752e d228 082c 941c 1954 38be 6101 d646  u..(.,...T8.a..F
+00000c40: a220 e3eb c029 4e25 23f0 dc3e b23f 0dbd  . ...)N%#..>.?..
+00000c50: 875e 36ca c302 eda7 d15c e7e2 4624 1a2a  .^6......\..F$.*
+00000c60: d559 7ec7 fe05 0efd cc4f 021f 14ab 2223  .Y~......O...."#
+00000c70: ec13 8a7d 1659 198d 583b e499 26ce 67c5  ...}.Y..X;..&.g.
+00000c80: 14e2 2614 e242 832f c9b4 516c 2639 e888  ..&..B./..Ql&9..
+00000c90: 6159 1e60 f753 30a3 47b2 1753 d9bd d919  aY.`.S0.G..S....
+00000ca0: 1d74 8da2 1ea6 506c d8c2 08e0 710a d0ea  .t....Pl....q...
+00000cb0: 6a4d 7604 f134 85f8 46db b9b1 1acf 5308  jMv..4..F.....S.
+00000cc0: 0fde ff9b 950c e33e 3ee1 7efe 71b7 de14  .......>>.~.q...
+00000cd0: 6d4d e313 0b55 a04a 67d7 7391 d0fe bdf6  mM...U.Jg.s.....
+00000ce0: 0e63 3bec e606 99d1 0d66 1d56 1c28 2684  .c;......f.V.(&.
+00000cf0: fb0a 918f 4e5c 97d3 a729 fe00 504b 0304  ....N\...)..PK..
+00000d00: 1400 0000 0800 853b 7756 7cf3 a3dc 5102  .......;wV|...Q.
+00000d10: 0000 f609 0000 0d00 0000 786c 2f73 7479  ..........xl/sty
+00000d20: 6c65 732e 786d 6cdd 56db 8adb 3010 fd15  les.xml.V...0...
+00000d30: e10f a893 9835 7149 f250 4360 a12d 0bbb  .....5qI.PC`.-..
+00000d40: 0f7d 5562 3911 e8e2 caf2 92f4 eb3b 2339  .}Ub9........;#9
+00000d50: 76b3 ab59 287d ab4d f0cc 1c9d b91b 67d3  v..Y(}.M......g.
+00000d60: fbab 12cf 6721 3cbb 6865 fa6d 76f6 befb  ....g!<.he.mv...
+00000d70: 9ce7 fdf1 2c34 ef3f d94e 1840 5aeb 34f7  ....,4.?.N.@Z.4.
+00000d80: a0ba 53de 774e f0a6 4792 56f9 6ab1 2873  ..S.wN..G.V.j.(s
+00000d90: cda5 c976 1b33 e8bd f63d 3bda c1f8 6db6  ...v.3...=;...m.
+00000da0: c8f2 dda6 b566 b62c b368 80a3 5c0b f6ca  .....f.,.h..\...
+00000db0: d536 abb9 9207 27c3 59ae a5ba 46f3 0a0d  .6....'.Y...F...
+00000dc0: 47ab ac63 1e52 1148 064b ff2b c2cb a861  G..c.R.H.K.+...a
+00000dd0: 96a3 1f2d 8d75 68cc 6384 f0e8 c1a9 546a  ...-.uh.c.....Tj
+00000de0: 4a60 9545 c36e d371 ef85 337b 5002 2718  J`.E.n.q..3{P.'.
+00000df0: df41 6c94 5fae 1d64 7072 fcba 5c3d 6433  .Al._..dpr..\=d3
+00000e00: 213c 20c8 c1ba 46b8 bb3a a369 b751 a2f5  !< ...F..:.i.Q..
+00000e10: 4070 f274 c6a7 b75d 8ea0 f756 83d0 487e  @p.t...]...V..H~
+00000e20: b286 871c 6e8c 5100 b747 a1d4 338e e847  ....n.Q..G..3..G
+00000e30: 7be7 fbd2 b2d8 ebc7 06db ccb0 d49b 0809  {...............
+00000e40: 8d62 7413 15f4 ffa7 b7e8 fb9f ddb2 4ebe  .bt...........N.
+00000e50: 5aff 6580 6a4c d07f 0ed6 8b27 275a 7909  Z.e.jL.....''Zy.
+00000e60: faa5 bd8f 3f85 0e89 dc45 9fac 0c97 639b  ....?....E....c.
+00000e70: 7dc7 9d53 b30b 7618 a4f2 d28c da59 368d  }..S..v......Y6.
+00000e80: 30ef 6a03 f79e 1f60 a9ef fcc3 f946 b47c  0.j....`.....F.|
+00000e90: 50fe 6502 b7d9 2c7f 138d 1c74 359d 7ac2  P.e...,....t5.z.
+00000ea0: b2c6 53b3 fc15 67b8 2ca7 cd84 58d2 34e2  ..S...g.,...X.4.
+00000eb0: 229a 7a54 dde9 1044 0602 441d 2f24 bc45  ".zT...D..D./$.E
+00000ec0: f6e1 4a23 1427 6269 0431 2a0e 9501 c589  ..J#.'bi.1*.....
+00000ed0: 2c2a ceff 54cf 9aac 2762 546e eb24 b226  ,*..T...'bTn.$.&
+00000ee0: 396b 9213 5929 a40e 3715 27cd a9e0 4a57  9k..Y)..7.'...JW
+00000ef0: 5a55 4551 9654 47eb 3a99 414d f5ad 2cf1  ZUEQ.TG.:.AM..,.
+00000f00: 97f6 46e5 860c 2a0e 46fa bb5e d3d3 a637  ..F...*.F..^...7
+00000f10: e4e3 3da0 66fa d186 5095 d29b 4855 4af7  ..=.f...P...HUJ.
+00000f20: 1a91 74df 9051 55e9 6953 7190 414d 81da  ..t..QU.iSq.AM..
+00000f30: 1d8c 9f8e 833b 95e6 1405 4e95 ca8d 7a83  .....;....N...z.
+00000f40: 69a4 aa28 0477 31bd a365 4974 a7c4 3b3d  i..(.w1..eIt..;=
+00000f50: 1fea 2d29 8aaa 4a23 88a5 3328 0a0a c1b7  ..-)..J#..3(....
+00000f60: 9146 a80c 3007 0a29 8af0 1d7c f33d ca6f  .F..0..)...|.=.o
+00000f70: dfa9 7cfe a7b7 fb0d 504b 0304 1400 0000  ..|.....PK......
+00000f80: 0800 853b 7756 978a bb1c c000 0000 1302  ...;wV..........
+00000f90: 0000 0b00 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
+00000fa0: 739d 92b9 6ec3 300c 407f c5d0 9e30 07d0  s...n.0.@....0..
+00000fb0: 2188 3365 f116 04f9 0156 a20f d812 058a  !.3e.....V......
+00000fc0: 459d bfaf daa5 7190 0b19 793d 3c12 dc1e  E.....q...y=<...
+00000fd0: 6940 ed38 a4b6 8ba9 18fd 1052 695a d5b8  i@.8.......RiZ..
+00000fe0: 0148 b625 8f69 ce91 42ae d42c 1e35 87d2  .H.%.i..B..,.5..
+00000ff0: 4044 db63 43b0 5a2c 3e40 2e19 66b7 bd64  @D.cC.Z,>@..f..d
+00001000: 16a7 73a4 5788 5cd7 9da5 3ddb 2f4f 416f  ..s.W.\...=./OAo
+00001010: 80af 3a4c 7142 6948 4b33 0ef0 cdd2 7f32  ..:LqBiHK3.....2
+00001020: f7f3 0c35 45e5 4a23 955b 1a78 d3e5 fe76  ...5E.J#.[.x...v
+00001030: e049 d1a1 2258 169a 45c9 d3a2 1da5 7f1d  .I.."X..E.......
+00001040: c7f6 90d3 e9af 6322 b47a 5be8 f971 6854  ......c".z[..qhT
+00001050: 0a8e dc63 258c 7162 b4fe 3582 c90f ec7e  ...c%.qb..5....~
+00001060: 0050 4b03 0414 0000 0008 0085 3b77 56da  .PK.........;wV.
+00001070: 9b20 0f53 0100 003b 0300 000f 0000 0078  . .S...;.......x
+00001080: 6c2f 776f 726b 626f 6f6b 2e78 6d6c b592  l/workbook.xml..
+00001090: 514b c340 0cc7 bf4a b90f 60bb 4d07 0ebb  QK.@...J..`.M...
+000010a0: 1787 3a10 1d4e f67e 6dd3 35ec ee52 72d7  ..:..N.~m.5..Rr.
+000010b0: 4df7 e94d 5b8a 0561 f8b2 a76b fe09 e92f  M..M[..a...k.../
+000010c0: ffe4 e144 7cc8 880e d197 35ce a7aa 0aa1  ...D|.....5.....
+000010d0: 5ec4 b1cf 2bb0 dadf 500d 4e32 25b1 d541  ^...+...P.N2%..A
+000010e0: 42de c7be 66d0 85af 0082 35f1 3449 e6b1  B...f.....5.4I..
+000010f0: d5e8 d4f2 61e8 b5e1 781c 5080 3c20 3911  ....a...x.P.< 9.
+00001100: 5b61 8770 f2bf f936 8c8e e831 4383 e13b  [a.p...6...1C..;
+00001110: 55dd b701 1559 7468 f10c 45aa 1215 f98a  U....Yth..E.....
+00001120: 4e2f c478 2617 b4d9 e64c c6a4 6ad2 2776  N/.x&....L..j.'v
+00001130: c001 f33f f2b6 85fc d499 ef94 a0b3 0f2d  ...?...........-
+00001140: 20a9 9a27 d2b0 44f6 a1ab e8fa 6b61 3c82   ..'..D.....ka<.
+00001150: 14f7 5113 e809 4d00 5ee9 00cf 4c4d 8d6e  ..Q...M.^...LM.n
+00001160: dfb6 9129 e2d1 189d 0fc3 db9b b8e0 ffd8  ...)............
+00001170: 4865 8939 ac28 6f2c b8d0 fbc8 605a 40e7  He.9.(o,....`Z@.
+00001180: 2bac bd8a 9cb6 90aa 1d19 2969 0792 3fac  +.........)i..?.
+00001190: 8b7e b820 5423 ab78 8192 e075 d1f1 5d8f  .~. T#.x...u..].
+000011a0: 650b de8b 3682 995e 8099 5e17 66a3 6be0  e...6..^..^.f.k.
+000011b0: 11ca ec02 caac dbdb b0ac 024a 7450 bc49  ...........JtP.I
+000011c0: 1b2f ba1c 4ebe e1a8 7d3a 7fa7 b777 937b  ./..N...}:...w.{
+000011d0: 3990 c698 47d1 dedd 2be9 62d8 fd70 b7cb  9...G...+.b..p..
+000011e0: 1f50 4b03 0414 0000 0008 0085 3b77 56bb  .PK.........;wV.
+000011f0: 6cea ecba 0000 001a 0300 001a 0000 0078  l..............x
+00001200: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+00001210: 2e78 6d6c 2e72 656c 73c5 9339 0e83 3010  .xml.rels..9..0.
+00001220: 45af 827c 0086 2549 1101 551a da88 0b58  E..|..%I..U....X
+00001230: 302c 62b1 e599 2870 fb10 28c0 528a 3488  0,b...(p..(.R.4.
+00001240: cafa 63f9 fd57 8ca3 2776 921b 3550 dd68  ..c..W..'v..5P.h
+00001250: 72c6 be1b 2816 35b3 be03 505e 632f c955  r...(.5...P^c/.U
+00001260: 1a87 f9a6 54a6 973c 4753 8196 792b 2b84  ....T..<GS..y++.
+00001270: c0f3 6e60 f60c 9144 7ba6 934d 1aff 21aa  ..n`...D{..M..!.
+00001280: b26c 727c a8fc d5e3 c03f c0f0 56a6 a51a  .lr|.....?..V...
+00001290: 9185 9349 5321 c702 c66e 1b13 2c87 efce  ...IS!...n..,...
+000012a0: 64e1 a445 2c4c 5af8 02ce 160a 2ca1 e07c  d..E,LZ.....,..|
+000012b0: a1d0 120a 0f14 229e 3aa4 cd66 cd56 fde5  ......".:..f.V..
+000012c0: c07a 9edf e2d6 bec4 7568 2fc9 f5eb 00d6  .z......uh/.....
+000012d0: 5748 3e50 4b03 0414 0000 0008 0085 3b77  WH>PK.........;w
+000012e0: 56a6 fc4a 5b23 0100 00df 0400 0013 0000  V..J[#..........
+000012f0: 005b 436f 6e74 656e 745f 5479 7065 735d  .[Content_Types]
+00001300: 2e78 6d6c cd94 cf4e c330 0cc6 5fa5 ea75  .xml...N.0.._..u
+00001310: 6a32 86c4 01ad bb00 57d8 8117 088d bb46  j2......W......F
+00001320: cd3f c5de e8de 1eb7 dd26 8146 c534 24b8  .?.......&.F.4$.
+00001330: 346a 6c7f 3fc7 9f92 e5eb 3e02 669d b31e  4jl.?.....>.f...
+00001340: cbbc 218a f752 62d5 8053 2842 04cf 913a  ..!..Rb..S(B...:
+00001350: 24a7 887f d346 4655 b56a 0372 319f dfc9  $....FFU.j.r1...
+00001360: 2a78 024f 05f5 1af9 6af9 08b5 da5a ca9e  *x.O....j....Z..
+00001370: 3ade 4613 7c99 27b0 9867 0f63 62cf 2a73  :.F.|.'..g.cb.*s
+00001380: 15a3 3595 228e cb9d d75f 28c5 8120 b872  ..5."...._(.. .r
+00001390: c8c1 c644 9c71 422e cf12 fac8 f780 43dd  ...D.qB.......C.
+000013a0: cb0e 5232 1ab2 b54a f4ac 1c67 c9ce 4aa4  ..R2...J...g..J.
+000013b0: bd05 14d3 1267 7a0c 756d 2ad0 a1da 3a2e  .....gz.um*...:.
+000013c0: 1118 1328 8d0d 0039 2b46 d1d9 3499 78c2  ...(...9+F..4.x.
+000013d0: 307e 6fae e60f 3253 40ce 5ca7 1091 1d4b  0~o...2S@.\....K
+000013e0: 7039 ee68 495f 5d44 1682 4466 fa88 2722  p9.hI_]D..Df..'"
+000013f0: 4b5f 7d3e e8dd d6a0 7fc8 e6f1 be87 d40e  K_}>............
+00001400: 7ea0 1c96 eb67 fcd9 e393 fe85 7d2c fe49  ~....g......},.I
+00001410: 1fb7 7fd8 c75b 08ed 6f5f b97e 154e 197f  .....[..o_.~.N..
+00001420: e4cb e15d 5b7d 0050 4b01 0214 0314 0000  ...][}.PK.......
+00001430: 0008 0085 3b77 5607 414d 6281 0000 00b1  ....;wV.AMb.....
+00001440: 0000 0010 0000 0000 0000 0000 0000 0080  ................
+00001450: 0100 0000 0064 6f63 5072 6f70 732f 6170  .....docProps/ap
+00001460: 702e 786d 6c50 4b01 0214 0314 0000 0008  p.xmlPK.........
+00001470: 0085 3b77 5614 9990 e0ee 0000 002b 0200  ..;wV........+..
+00001480: 0011 0000 0000 0000 0000 0000 0080 01af  ................
+00001490: 0000 0064 6f63 5072 6f70 732f 636f 7265  ...docProps/core
 000014a0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-000014b0: e54e 6856 695e 91e4 7101 0000 3003 0000  .NhVi^..q...0...
-000014c0: 1800 0000 0000 0000 0000 0000 8081 0e08  ................
-000014d0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-000014e0: 7368 6565 7431 2e78 6d6c 504b 0102 1403  sheet1.xmlPK....
-000014f0: 1400 0000 0800 e54e 6856 39d0 d6e8 4c01  .......NhV9...L.
-00001500: 0000 5202 0000 1800 0000 0000 0000 0000  ..R.............
-00001510: 0000 8081 b509 0000 786c 2f77 6f72 6b73  ........xl/works
-00001520: 6865 6574 732f 7368 6565 7432 2e78 6d6c  heets/sheet2.xml
-00001530: 504b 0102 1403 1400 0000 0800 e54e 6856  PK...........NhV
-00001540: 1f23 f767 4c01 0000 5002 0000 1800 0000  .#.gL...P.......
-00001550: 0000 0000 0000 0000 8081 370b 0000 786c  ..........7...xl
-00001560: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00001570: 7433 2e78 6d6c 504b 0102 1403 1400 0000  t3.xmlPK........
-00001580: 0800 e54e 6856 7cf3 a3dc 5102 0000 f609  ...NhV|...Q.....
-00001590: 0000 0d00 0000 0000 0000 0000 0000 8001  ................
-000015a0: b90c 0000 786c 2f73 7479 6c65 732e 786d  ....xl/styles.xm
-000015b0: 6c50 4b01 0214 0314 0000 0008 00e5 4e68  lPK...........Nh
-000015c0: 5697 8abb 1cc0 0000 0013 0200 000b 0000  V...............
-000015d0: 0000 0000 0000 0000 0080 0135 0f00 005f  ...........5..._
-000015e0: 7265 6c73 2f2e 7265 6c73 504b 0102 1403  rels/.relsPK....
-000015f0: 1400 0000 0800 e54e 6856 6c20 24ba 5501  .......NhVl $.U.
-00001600: 0000 3b03 0000 0f00 0000 0000 0000 0000  ..;.............
-00001610: 0000 8001 1e10 0000 786c 2f77 6f72 6b62  ........xl/workb
-00001620: 6f6f 6b2e 786d 6c50 4b01 0214 0314 0000  ook.xmlPK.......
-00001630: 0008 00e5 4e68 56bb 6cea ecba 0000 001a  ....NhV.l.......
-00001640: 0300 001a 0000 0000 0000 0000 0000 0080  ................
-00001650: 01a0 1100 0078 6c2f 5f72 656c 732f 776f  .....xl/_rels/wo
-00001660: 726b 626f 6f6b 2e78 6d6c 2e72 656c 7350  rkbook.xml.relsP
-00001670: 4b01 0214 0314 0000 0008 00e5 4e68 56a6  K...........NhV.
-00001680: fc4a 5b23 0100 00df 0400 0013 0000 0000  .J[#............
-00001690: 0000 0000 0000 0080 0192 1200 005b 436f  .............[Co
-000016a0: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-000016b0: 504b 0506 0000 0000 0b00 0b00 ca02 0000  PK..............
-000016c0: e613 0000 0000                           ......
+000014b0: 853b 7756 995c 9c23 1006 0000 9c27 0000  .;wV.\.#.....'..
+000014c0: 1300 0000 0000 0000 0000 0000 8001 cc01  ................
+000014d0: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
+000014e0: 312e 786d 6c50 4b01 0214 0314 0000 0008  1.xmlPK.........
+000014f0: 0085 3b77 569c 88b2 b791 0100 00d1 0300  ..;wV...........
+00001500: 0018 0000 0000 0000 0000 0000 0080 810d  ................
+00001510: 0800 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00001520: 2f73 6865 6574 312e 786d 6c50 4b01 0214  /sheet1.xmlPK...
+00001530: 0314 0000 0008 0085 3b77 56f5 0284 4e46  ........;wV...NF
+00001540: 0100 0040 0200 0018 0000 0000 0000 0000  ...@............
+00001550: 0000 0080 81d4 0900 0078 6c2f 776f 726b  .........xl/work
+00001560: 7368 6565 7473 2f73 6865 6574 322e 786d  sheets/sheet2.xm
+00001570: 6c50 4b01 0214 0314 0000 0008 0085 3b77  lPK...........;w
+00001580: 56a9 5477 ab76 0100 0040 0300 0018 0000  V.Tw.v...@......
+00001590: 0000 0000 0000 0000 0080 8150 0b00 0078  ...........P...x
+000015a0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+000015b0: 6574 332e 786d 6c50 4b01 0214 0314 0000  et3.xmlPK.......
+000015c0: 0008 0085 3b77 567c f3a3 dc51 0200 00f6  ....;wV|...Q....
+000015d0: 0900 000d 0000 0000 0000 0000 0000 0080  ................
+000015e0: 01fc 0c00 0078 6c2f 7374 796c 6573 2e78  .....xl/styles.x
+000015f0: 6d6c 504b 0102 1403 1400 0000 0800 853b  mlPK...........;
+00001600: 7756 978a bb1c c000 0000 1302 0000 0b00  wV..............
+00001610: 0000 0000 0000 0000 0000 8001 780f 0000  ............x...
+00001620: 5f72 656c 732f 2e72 656c 7350 4b01 0214  _rels/.relsPK...
+00001630: 0314 0000 0008 0085 3b77 56da 9b20 0f53  ........;wV.. .S
+00001640: 0100 003b 0300 000f 0000 0000 0000 0000  ...;............
+00001650: 0000 0080 0161 1000 0078 6c2f 776f 726b  .....a...xl/work
+00001660: 626f 6f6b 2e78 6d6c 504b 0102 1403 1400  book.xmlPK......
+00001670: 0000 0800 853b 7756 bb6c eaec ba00 0000  .....;wV.l......
+00001680: 1a03 0000 1a00 0000 0000 0000 0000 0000  ................
+00001690: 8001 e111 0000 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
+000016a0: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
+000016b0: 504b 0102 1403 1400 0000 0800 853b 7756  PK...........;wV
+000016c0: a6fc 4a5b 2301 0000 df04 0000 1300 0000  ..J[#...........
+000016d0: 0000 0000 0000 0000 8001 d312 0000 5b43  ..............[C
+000016e0: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
+000016f0: 6c50 4b05 0600 0000 000b 000b 00ca 0200  lPK.............
+00001700: 0027 1400 0000 00                        .'.....
```

### Comparing `pymetamodel-0.2.7/examples/ceur-ws/ceur-ws.yaml` & `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -9,99 +9,78 @@
     prefix_reference: CeurwsSchema/
   xsd:
     prefix_prefix: xsd
     prefix_reference: http://www.w3.org/2001/XMLSchema#
   shex:
     prefix_prefix: shex
     prefix_reference: http://www.w3.org/ns/shex#
-  schema:
-    prefix_prefix: schema
-    prefix_reference: http://schema.org/
 default_prefix: CeurwsSchema
 default_range: string
 types:
   string:
     name: string
     description: A character string
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Text
     base: str
     uri: xsd:string
   integer:
     name: integer
     description: An integer
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Integer
     base: int
     uri: xsd:integer
   boolean:
     name: boolean
     description: A binary (true or false) value
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Boolean
     base: Bool
     uri: xsd:boolean
     repr: bool
   float:
     name: float
     description: A real number that conforms to the xsd:float specification
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Float
     base: float
     uri: xsd:float
   double:
     name: double
     description: A real number that conforms to the xsd:double specification
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:Float
     base: float
     uri: xsd:double
   decimal:
     name: decimal
     description: A real number with arbitrary precision that conforms to the xsd:decimal
       specification
     from_schema: https://w3id.org/linkml/types
-    broad_mappings:
-    - schema:Number
     base: Decimal
     uri: xsd:decimal
   time:
     name: time
     description: A time object represents a (local) time of day, independent of any
       particular day
     notes:
-    - URI is dateTime because OWL reasoners do not work with straight date or time
+    - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Time
     base: XSDTime
     uri: xsd:dateTime
     repr: str
   date:
     name: date
     description: a date (year, month and day) in an idealized calendar
     notes:
     - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Date
     base: XSDDate
     uri: xsd:date
     repr: str
   datetime:
     name: datetime
     description: The combination of a date and time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:DateTime
     base: XSDDateTime
     uri: xsd:dateTime
     repr: str
   date_or_datetime:
     name: date_or_datetime
     description: Either a date or a datetime
     from_schema: https://w3id.org/linkml/types
@@ -111,36 +90,18 @@
   uriorcurie:
     name: uriorcurie
     description: a URI or a CURIE
     from_schema: https://w3id.org/linkml/types
     base: URIorCURIE
     uri: xsd:anyURI
     repr: str
-  curie:
-    name: curie
-    conforms_to: https://www.w3.org/TR/curie/
-    description: a compact URI
-    comments:
-    - in RDF serializations this MUST be expanded to a URI
-    - in non-RDF serializations MAY be serialized as the compact representation
-    from_schema: https://w3id.org/linkml/types
-    base: Curie
-    uri: xsd:string
-    repr: str
   uri:
     name: uri
-    conforms_to: https://www.ietf.org/rfc/rfc3987.txt
     description: a complete URI
-    comments:
-    - in RDF serializations a slot with range of uri is treated as a literal or type
-      xsd:anyURI unless it is an identifier or a reference to an identifier, in which
-      case it is translated directly to a node
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:URL
     base: URI
     uri: xsd:anyURI
     repr: str
   ncname:
     name: ncname
     description: Prefix part of CURIE
     from_schema: https://w3id.org/linkml/types
@@ -165,35 +126,71 @@
     repr: str
 slots:
   number:
     name: number
     description: The number Volume
     from_schema: CeurwsSchema
     range: double
+  acronym:
+    name: acronym
+    description: The official acronym/short name of the Volume
+    from_schema: CeurwsSchema
+    range: string
+  wikidataid:
+    name: wikidataid
+    description: The wikidataid of the volume,The wikidataid of the paper
+    from_schema: CeurwsSchema
+    range: string
   title:
     name: title
     description: The title of the Volume,The title of the Session,The title of the
       Paper
     from_schema: CeurwsSchema
     range: string
+  description:
+    name: description
+    description: A wikidata compatible description of the volume,A wikidata compatible
+      description of the paper
+    from_schema: CeurwsSchema
+    range: string
+  url:
+    name: url
+    description: The url of the volume
+    from_schema: CeurwsSchema
+    range: string
+  date:
+    name: date
+    description: The publication date of the volume
+    from_schema: CeurwsSchema
+    range: date
+  dblp:
+    name: dblp
+    description: The dblp publication id of the volume
+    from_schema: CeurwsSchema
+    range: string
+  k10plus:
+    name: k10plus
+    description: The k10 plus PPN id of the volume
+    from_schema: CeurwsSchema
+    range: string
+  urn:
+    name: urn
+    description: The URN-NBN id of the volume
+    from_schema: CeurwsSchema
+    range: string
   volume:
     name: volume
     description: volume,volume
     from_schema: CeurwsSchema
     range: Volume
   id:
     name: id
     description: The id (filename) of the Paper
     from_schema: CeurwsSchema
     range: string
-  authors:
-    name: authors
-    description: authors of the Paper
-    from_schema: CeurwsSchema
-    range: string
   pdfUrl:
     name: pdfUrl
     description: the url for the pdf of this paper
     from_schema: CeurwsSchema
     range: uri
   session:
     name: session
@@ -208,20 +205,61 @@
     from_schema: CeurwsSchema
     attributes:
       number:
         name: number
         description: The number Volume
         from_schema: CeurwsSchema
         range: double
+      acronym:
+        name: acronym
+        description: The official acronym/short name of the Volume
+        from_schema: CeurwsSchema
+        range: string
+      wikidataid:
+        name: wikidataid
+        description: The wikidataid of the volume,The wikidataid of the paper
+        from_schema: CeurwsSchema
+        range: string
       title:
         name: title
         description: The title of the Volume,The title of the Session,The title of
           the Paper
         from_schema: CeurwsSchema
         range: string
+      description:
+        name: description
+        description: A wikidata compatible description of the volume,A wikidata compatible
+          description of the paper
+        from_schema: CeurwsSchema
+        range: string
+      url:
+        name: url
+        description: The url of the volume
+        from_schema: CeurwsSchema
+        range: string
+      date:
+        name: date
+        description: The publication date of the volume
+        from_schema: CeurwsSchema
+        range: date
+      dblp:
+        name: dblp
+        description: The dblp publication id of the volume
+        from_schema: CeurwsSchema
+        range: string
+      k10plus:
+        name: k10plus
+        description: The k10 plus PPN id of the volume
+        from_schema: CeurwsSchema
+        range: string
+      urn:
+        name: urn
+        description: The URN-NBN id of the volume
+        from_schema: CeurwsSchema
+        range: string
   Session:
     name: Session
     description: A Session is a a collection of papers as part of a Volume
     from_schema: CeurwsSchema
     attributes:
       title:
         name: title
@@ -235,30 +273,36 @@
         from_schema: CeurwsSchema
         range: Volume
   Paper:
     name: Paper
     description: A paper is e.g. a scholarly article
     from_schema: CeurwsSchema
     attributes:
+      description:
+        name: description
+        description: A wikidata compatible description of the volume,A wikidata compatible
+          description of the paper
+        from_schema: CeurwsSchema
+        range: string
       id:
         name: id
         description: The id (filename) of the Paper
         from_schema: CeurwsSchema
         range: string
+      wikidataid:
+        name: wikidataid
+        description: The wikidataid of the volume,The wikidataid of the paper
+        from_schema: CeurwsSchema
+        range: string
       title:
         name: title
         description: The title of the Volume,The title of the Session,The title of
           the Paper
         from_schema: CeurwsSchema
         range: string
-      authors:
-        name: authors
-        description: authors of the Paper
-        from_schema: CeurwsSchema
-        range: string
       pdfUrl:
         name: pdfUrl
         description: the url for the pdf of this paper
         from_schema: CeurwsSchema
         range: uri
       volume:
         name: volume
```

### Comparing `pymetamodel-0.2.7/examples/ceur-ws/ceur-ws_puml.txt` & `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws_puml.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 @startuml
 package CeurwsSchema {
   class Volume {
     number:Number
+    acronym:text
+    wikidataid:External identifier
     title:Text
+    description:text
+    url:text
+    date:Date
+    dblp:External identifier
+    k10plus:External identifier
+    urn:External identifier
   }
 Note top of Volume
 A Volume is a collection of papers mostly documenting the results of an academic event
 End note
   class Session {
     title:Text
   }
 Note top of Session
 A Session is a a collection of papers as part of a Volume
 End note
   class Paper {
     id:Text
+    wikidataid:External identifier
+    description:text
     title:Text
-    authors:Text
     pdfUrl:URL
   }
 Note top of Paper
 A paper is e.g. a scholarly article
 End note
 }
 Volume "volume 1" -- "sessions *" Session
 Volume "volume 1" -- "papers *" Paper
+Volume "volumes *" -- "editors *" Scholar
 Session "session 1" -- "papers *" Paper
+Paper "papers *" -- "authors *" Scholar
 
 ' BITPlan Corporate identity skin params
 ' Copyright (c) 2015-2023 BITPlan GmbH
 ' see http://wiki.bitplan.com/PlantUmlSkinParams#BITPlanCI
 ' skinparams generated by com.bitplan.restmodelmanager
 skinparam note {
   BackGroundColor #FFFFFF
```

### Comparing `pymetamodel-0.2.7/examples/city/city.py` & `pymetamodel-0.3.0/examples/city/city.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from city.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-08T09:54:31
+# Generation date: 2023-03-23T07:27:49
 # Schema: GeneralContext
 #
 # id: GeneralContext
 # description:
 # license:
 
 import dataclasses
@@ -18,26 +18,25 @@
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
 from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
 from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.metamodelcore import Bool, Curie, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
+from linkml_runtime.utils.metamodelcore import Bool, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
 GENERALCONTEXT = CurieNamespace('GeneralContext', 'GeneralContext/')
 LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
-SCHEMA = CurieNamespace('schema', 'http://schema.org/')
 SHEX = CurieNamespace('shex', 'http://www.w3.org/ns/shex#')
 XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = GENERALCONTEXT
 
 
 # Types
 class String(str):
@@ -124,22 +123,14 @@
     """ a URI or a CURIE """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uriorcurie"
     type_model_uri = GENERALCONTEXT.Uriorcurie
 
 
-class Curie(Curie):
-    """ a compact URI """
-    type_class_uri = XSD.string
-    type_class_curie = "xsd:string"
-    type_name = "curie"
-    type_model_uri = GENERALCONTEXT.Curie
-
-
 class Uri(URI):
     """ a complete URI """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uri"
     type_model_uri = GENERALCONTEXT.Uri
```

### Comparing `pymetamodel-0.2.7/examples/city/city.sidif` & `pymetamodel-0.3.0/examples/city/city.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/city/city.xlsx` & `pymetamodel-0.3.0/examples/city/city.xlsx`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 504b 0304 1400 0000 0800 d04e 6856 0741  PK.........NhV.A
+00000000: 504b 0304 1400 0000 0800 783b 7756 0741  PK........x;wV.A
 00000010: 4d62 8100 0000 b100 0000 1000 0000 646f  Mb............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 3d0b 0231 1044 ffca 71bd b741 c142 6240  =..1.D..q..A.Bb@
 00000040: d052 b0b2 0f7b 1b2f 9064 43b2 427e be39  .R...{./.dC.B~.9
 00000050: c18f 6e1e 6f18 46df 0a67 2ae2 a90e 2d86  ..n.o.F..g*...-.
 00000060: 548f e322 920f 0015 178a b64e 5da7 6e1c  T..".......N].n.
 00000070: 9768 a563 7900 3be7 91ce 8ccf 4849 60ab  .h.cy.;.....HI`.
 00000080: d41e a809 a599 e64d fe0e 8e46 9f72 0e1e  .......M...F.r..
 00000090: ad78 4ee6 eab1 7065 27c3 a521 050d ff72  .xN...pe'..!...r
 000000a0: 6dde a9d4 35ef 26f5 961f d6f0 3b69 5e50  m...5.&.....;i^P
-000000b0: 4b03 0414 0000 0008 00d0 4e68 569f ef9c  K.........NhV...
-000000c0: 05ef 0000 002b 0200 0011 0000 0064 6f63  .....+.......doc
+000000b0: 4b03 0414 0000 0008 0078 3b77 56c5 f282  K........x;wV...
+000000c0: 33ef 0000 002b 0200 0011 0000 0064 6f63  3....+.......doc
 000000d0: 5072 6f70 732f 636f 7265 2e78 6d6c cd92  Props/core.xml..
-000000e0: db4a 0331 1086 5f45 72bf 3b7b 5029 619b  .J.1.._Er.;{P)a.
-000000f0: 1b4b af14 040b 8a77 2199 b6c1 cd81 6464  .K.....w!.....dd
-00000100: b76f 6f76 6db7 883e 8090 9bcc fcf9 e61b  .oovm..>........
-00000110: 48a7 0257 3ee2 73f4 0123 194c 37a3 ed5d  H..W>.s..#.L7..]
-00000120: e22a acd9 9128 7080 a48e 6865 2a73 c2e5  .*...(p...he*s..
-00000130: e6de 472b 295f e301 8254 1ff2 80d0 54d5  ..G+)_...T....T.
-00000140: 3d58 24a9 2549 9880 4558 884c 745a 7115  =X$.%I..EX.LtZq.
-00000150: 5192 8f67 bc56 0b3e 7cc6 7e86 6905 d8a3  Q..g.V.>|.~.i...
-00000160: 4547 09ea b206 26a6 89e1 34f6 1d5c 0113  EG....&...4..\..
-00000170: 8c30 daf4 5d40 bd10 e7ea 9fd8 b903 ec9c  .0..]@..........
-00000180: 1c93 5952 c330 9443 3be7 f20e 35bc 3d3d  ..YR.0.C;...5.==
-00000190: becc eb16 c625 924e 617e 950c a753 c035  .....%.Na~...S.5
-000001a0: bb4c 7e6d 1f36 bb2d 134d d5b4 4595 cf6a  .L~m.6.-.M..E..j
-000001b0: 57ad f8dd 2d6f 9bf7 c9f5 87df 55d8 7a6d  W...-o......U.zm
-000001c0: f6e6 1f1b 5f04 4507 bffe 85f8 0250 4b03  ...._.E......PK.
-000001d0: 0414 0000 0008 00d0 4e68 5699 5c9c 2310  ........NhV.\.#.
+000000e0: 514b c330 10c7 bf8a e4bd bd34 9589 a1eb  QK.0.......4....
+000000f0: 8b63 4f0a 8203 c5b7 90dc b660 d386 e4a4  .cO........`....
+00000100: ddb7 378d 5b87 e807 f031 77ff fcee 7770  ..7.[....1w...wp
+00000110: 8df6 520f 019f c3e0 3190 c578 33b9 ae8f  ..R.....1..x3...
+00000120: 52fb 353b 1279 0910 f511 9d8a 654a f4a9  R.5;.y......eJ..
+00000130: b91f 8253 949e e100 5ee9 0f75 4010 9caf  ...S....^..u@...
+00000140: c021 29a3 48c1 0c2c fc42 646d 63b4 d401  .!).H..,.Bdmc...
+00000150: 150d e18c 377a c1fb cfd0 6598 d180 1d3a  ....7z....e....:
+00000160: ec29 4255 56c0 da79 a23f 4d5d 0357 c00c  .)BUV..y.?M].W..
+00000170: 230c 2e7e 17d0 2cc4 5cfd 139b 3bc0 cec9  #..~..,.\...;...
+00000180: 29da 2535 8e63 39d6 3997 76a8 e0ed e9f1  ).%5.c9.9.v.....
+00000190: 25af 5bd8 3e92 ea35 a65f d14a 3a79 5cb3  %.[.>..5._.J:y\.
+000001a0: cbe4 d7fa 61b3 dbb2 5670 5117 bc2e 44bd  ....a...VpQ...D.
+000001b0: e32b 29ee e4ed fdfb ecfa c3ef 2aec 0663  .+).........*..c
+000001c0: f7f6 1f1b 5f04 db06 7edd 45fb 0550 4b03  ...._...~.E..PK.
+000001d0: 0414 0000 0008 0078 3b77 5699 5c9c 2310  .......x;wV.\.#.
 000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
 000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
 00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
 00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
 00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
 00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
 00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
@@ -123,182 +123,181 @@
 000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
 000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
 000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
 000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
 000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
 000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
 00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
-00000810: 0304 1400 0000 0800 d04e 6856 418d 67d7  .........NhVA.g.
-00000820: 6601 0000 c702 0000 1800 0000 786c 2f77  f...........xl/w
+00000810: 0304 1400 0000 0800 783b 7756 e4d3 dff0  ........x;wV....
+00000820: 6001 0000 af02 0000 1800 0000 786c 2f77  `...........xl/w
 00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00000840: 2e78 6d6c 8552 db6e c230 0cfd 952a 1f40  .xml.R.n.0...*.@
-00000850: 6012 db84 da4a 0334 6d0f 9310 68db 230a  `....J.4m...h.#.
-00000860: ad4b 2392 b84b dc75 fcfd e272 1193 107b  .K#..K.u...r...{
-00000870: aaed f81c fb9c 3aed d0ef 420d 40c9 8f35  ......:...B.@..5
-00000880: 2e64 a226 6a26 5286 a206 abc2 001b 70f1  .d.&j&R.......p.
-00000890: a542 6f15 c5d4 6f65 683c a8b2 0759 23ef  .Bo...oeh<...Y#.
-000008a0: 86c3 7b69 9576 224f fbda c2e7 29b6 64b4  ..{i.v"O....).d.
-000008b0: 8385 4f42 6bad f2fb 2918 ec32 3112 a7c2  ..OBk...)..21...
-000008c0: 526f 6be2 82cc d346 6d61 05f4 de2c 7ccc  Rok....Fma...,|.
-000008d0: e499 a5d4 165c d0e8 120f 5526 9e46 9379  .....\....U&.F.y
-000008e0: dfdf 377c 68e8 c245 9cb0 920d e28e 93d7  ..7|h..E........
-000008f0: 3213 435e 080c 14c4 0c2a 7ebe 6106 c630  2.C^.....*~.a..0
-00000900: 515c e3eb c829 ce23 1978 199f d89f 7bed  Q\...).#.x....{.
-00000910: 51cb 4605 98a1 f9d4 25d5 9978 1449 0995  Q.F.....%..x.I..
-00000920: 6a0d 2db1 7b81 a39e f179 c1b9 2295 a71e  j.-.{....y.."...
-00000930: bbc4 b3ce 3c2d 38e0 d9b1 4f3b f667 453e  ....<-8...O;.gE>
-00000940: d675 1c44 79a1 69bf 5e3b 6521 9514 d7e0  .u.Dy.i.^;e!....
-00000950: aa2c 8ea8 e96d 5407 1bf6 f00a 70f6 0f50  .,...mT.....p..P
-00000960: ef74 03a5 56eb d69b 2bf0 f96d f802 9bd6  .t..V...+..m....
-00000970: 28f6 f72f 5646 d527 270f 36f0 7a6f ca6f  (../VF.''.6.zo.o
-00000980: b50b 8981 2a72 0e07 0f63 91f8 836d 8784  ....*r...c...m..
-00000990: b0e9 4f64 8344 68fb b08e 9706 9e1b e27b  ..Od.Dh........{
-000009a0: 8548 a784 ffda f976 f35f 504b 0304 1400  .H.....v._PK....
-000009b0: 0000 0800 d04e 6856 7cf3 a3dc 5102 0000  .....NhV|...Q...
-000009c0: f609 0000 0d00 0000 786c 2f73 7479 6c65  ........xl/style
-000009d0: 732e 786d 6cdd 56db 8adb 3010 fd15 e10f  s.xml.V...0.....
-000009e0: a893 9835 7149 f250 4360 a12d 0bbb 0f7d  ...5qI.PC`.-...}
-000009f0: 5562 3911 e8e2 caf2 92f4 eb3b 2339 76b3  Ub9........;#9v.
-00000a00: ab59 287d ab4d f0cc 1c9d b91b 67d3 fbab  .Y(}.M......g...
-00000a10: 12cf 6721 3cbb 6865 fa6d 76f6 befb 9ce7  ..g!<.he.mv.....
-00000a20: fdf1 2c34 ef3f d94e 1840 5aeb 34f7 a0ba  ..,4.?.N.@Z.4...
-00000a30: 53de 774e f0a6 4792 56f9 6ab1 2873 cda5  S.wN..G.V.j.(s..
-00000a40: c976 1b33 e8bd f63d 3bda c1f8 6db6 c8f2  .v.3...=;...m...
-00000a50: dda6 b566 b62c b368 80a3 5c0b f6ca d536  ...f.,.h..\....6
-00000a60: abb9 9207 27c3 59ae a5ba 46f3 0a0d 47ab  ....'.Y...F...G.
-00000a70: ac63 1e52 1148 064b ff2b c2cb a861 96a3  .c.R.H.K.+...a..
-00000a80: 1f2d 8d75 68cc 6384 f0e8 c1a9 546a 4a60  .-.uh.c.....TjJ`
-00000a90: 9545 c36e d371 ef85 337b 5002 2718 df41  .E.n.q..3{P.'..A
-00000aa0: 6c94 5fae 1d64 7072 fcba 5c3d 6433 213c  l._..dpr..\=d3!<
-00000ab0: 20c8 c1ba 46b8 bb3a a369 b751 a2f5 4070   ...F..:.i.Q..@p
-00000ac0: f274 c6a7 b75d 8ea0 f756 83d0 487e b286  .t...]...V..H~..
-00000ad0: 871c 6e8c 5100 b747 a1d4 338e e847 7be7  ..n.Q..G..3..G{.
-00000ae0: fbd2 b2d8 ebc7 06db ccb0 d49b 0809 8d62  ...............b
-00000af0: 7413 15f4 ffa7 b7e8 fb9f ddb2 4ebe 5aff  t...........N.Z.
-00000b00: 6580 6a4c d07f 0ed6 8b27 275a 7909 faa5  e.jL.....''Zy...
-00000b10: bd8f 3f85 0e89 dc45 9fac 0c97 639b 7dc7  ..?....E....c.}.
-00000b20: 9d53 b30b 7618 a4f2 d28c da59 368d 30ef  .S..v......Y6.0.
-00000b30: 6a03 f79e 1f60 a9ef fcc3 f946 b47c 50fe  j....`.....F.|P.
-00000b40: 6502 b7d9 2c7f 138d 1c74 359d 7ac2 b2c6  e...,....t5.z...
-00000b50: 53b3 fc15 67b8 2ca7 cd84 58d2 34e2 229a  S...g.,...X.4.".
-00000b60: 7a54 dde9 1044 0602 441d 2f24 bc45 f6e1  zT...D..D./$.E..
-00000b70: 4a23 1427 6269 0431 2a0e 9501 c589 2c2a  J#.'bi.1*.....,*
-00000b80: ceff 54cf 9aac 2762 546e eb24 b226 396b  ..T...'bTn.$.&9k
-00000b90: 9213 5929 a40e 3715 27cd a9e0 4a57 5a55  ..Y)..7.'...JWZU
-00000ba0: 4551 9654 47eb 3a99 414d f5ad 2cf1 97f6  EQ.TG.:.AM..,...
-00000bb0: 46e5 860c 2a0e 46fa bb5e d3d3 a637 e4e3  F...*.F..^...7..
-00000bc0: 3da0 66fa d186 5095 d29b 4855 4af7 1a91  =.f...P...HUJ...
-00000bd0: 74df 9051 55e9 6953 7190 414d 81da 1d8c  t..QU.iSq.AM....
-00000be0: 9f8e 833b 95e6 1405 4e95 ca8d 7a83 69a4  ...;....N...z.i.
-00000bf0: aa28 0477 31bd a365 4974 a7c4 3b3d 1fea  .(.w1..eIt..;=..
-00000c00: 2d29 8aaa 4a23 88a5 3328 0a0a c1b7 9146  -)..J#..3(.....F
-00000c10: a80c 3007 0a29 8af0 1d7c f33d ca6f dfa9  ..0..)...|.=.o..
-00000c20: 7cfe a7b7 fb0d 504b 0304 1400 0000 0800  |.....PK........
-00000c30: d04e 6856 978a bb1c c000 0000 1302 0000  .NhV............
-00000c40: 0b00 0000 5f72 656c 732f 2e72 656c 739d  ...._rels/.rels.
-00000c50: 92b9 6ec3 300c 407f c5d0 9e30 07d0 2188  ..n.0.@....0..!.
-00000c60: 3365 f116 04f9 0156 a20f d812 058a 459d  3e.....V......E.
-00000c70: bfaf daa5 7190 0b19 793d 3c12 dc1e 6940  ....q...y=<...i@
-00000c80: ed38 a4b6 8ba9 18fd 1052 695a d5b8 0148  .8.......RiZ...H
-00000c90: b625 8f69 ce91 42ae d42c 1e35 87d2 4044  .%.i..B..,.5..@D
-00000ca0: db63 43b0 5a2c 3e40 2e19 66b7 bd64 16a7  .cC.Z,>@..f..d..
-00000cb0: 73a4 5788 5cd7 9da5 3ddb 2f4f 416f 80af  s.W.\...=./OAo..
-00000cc0: 3a4c 7142 6948 4b33 0ef0 cdd2 7f32 f7f3  :LqBiHK3.....2..
-00000cd0: 0c35 45e5 4a23 955b 1a78 d3e5 fe76 e049  .5E.J#.[.x...v.I
-00000ce0: d1a1 2258 169a 45c9 d3a2 1da5 7f1d c7f6  .."X..E.........
-00000cf0: 90d3 e9af 6322 b47a 5be8 f971 6854 0a8e  ....c".z[..qhT..
-00000d00: dc63 258c 7162 b4fe 3582 c90f ec7e 0050  .c%.qb..5....~.P
-00000d10: 4b03 0414 0000 0008 00d0 4e68 56d4 b000  K.........NhV...
-00000d20: a232 0100 0021 0200 000f 0000 0078 6c2f  .2...!.......xl/
-00000d30: 776f 726b 626f 6f6b 2e78 6d6c 8d51 d16a  workbook.xml.Q.j
-00000d40: c240 10fc 9570 1fd0 4469 858a f145 692b  .@...p..Di...Ei+
-00000d50: 9456 6af1 fd4c 3666 f1ee 36ec 6db4 f5eb  .Vj..L6f..6.m...
-00000d60: bb49 0815 fad2 a7bd 9d59 8699 b9c5 85f8  .I.......Y......
-00000d70: 7420 3a25 5fde 8598 9b5a a499 a769 2c6a  t :%_....Z...i,j
-00000d80: f036 de51 0341 998a d85b d195 8f69 6c18  .6.Q.A...[...il.
-00000d90: 6c19 6b00 f12e 9d66 d92c f516 8359 2e46  l.k....f.,...Y.F
-00000da0: ad2d a7b7 0b09 1482 1414 ec80 3dc2 25fe  .-..........=.%.
-00000db0: f2dd 9a9c 31e2 011d ca77 6efa b703 9378  ....1....wn....x
-00000dc0: 0ce8 f10a 656e 3293 c49a 2e2f c478 a520  ....en2..../.x. 
-00000dd0: d6ed 0a26 e772 3319 883d b060 f107 de75  ...&.r3..=.`...u
-00000de0: 263f ed21 f688 d8c3 8755 23b9 9965 2a58  &?.!.....U#..e*X
-00000df0: 2147 e92f 7a7d ab1e cfa0 c7c3 d60a 3da1  !G./z}........=.
-00000e00: 13e0 b515 7866 6a1b 0cc7 4e46 53a4 3731  ....xfj...NFS.71
-00000e10: fa1e c639 9438 e7ff d448 5585 05ac a968  ...9.8...HU....h
-00000e20: 3d04 197a 6470 9dc1 106b 6ca2 4982 f590  =..zdp...kl.I...
-00000e30: 9b95 b6d2 c551 fd4d 3944 13f5 7453 14cf  .....Q.M9D..tS..
-00000e40: 5109 de94 83bb d152 0915 0628 df54 252a  Q......R...(.T%*
-00000e50: aef5 145b 4eba d1eb 4cef 1f26 8f5a 43eb  ...[N...L..&.ZC.
-00000e60: dc4a b1f7 f04a b61c 138e bfb3 fc01 504b  .J...J........PK
-00000e70: 0304 1400 0000 0800 d04e 6856 241e 9ba2  .........NhV$...
-00000e80: ad00 0000 f801 0000 1a00 0000 786c 2f5f  ............xl/_
-00000e90: 7265 6c73 2f77 6f72 6b62 6f6f 6b2e 786d  rels/workbook.xm
-00000ea0: 6c2e 7265 6c73 b591 3d0e 8330 0c85 af12  l.rels..=..0....
-00000eb0: e500 3550 a943 054c 5d58 2b2e 1005 f323  ..5P.C.L]X+....#
-00000ec0: 1212 c5ae 0ab7 2f85 0190 3a74 61b2 9e2d  ....../...:ta..-
-00000ed0: 7fef c94e 9f68 1477 6ea0 b6f3 2446 6b06  ...N.h.wn...$Fk.
-00000ee0: ca64 cbec ef00 a45b b48a 2ece e330 4f6a  .d.....[.....0Oj
-00000ef0: 17ac e259 8606 bcd2 bd6a 1092 28ba 41d8  ...Y.....j..(.A.
-00000f00: 3364 9eee 99a2 9c3c fe43 7475 dd69 7c38  3d.....<.Ctu.i|8
-00000f10: fdb2 38f0 0f30 bc5d e8a9 4564 294a 151a  ..8..0.]..Ed)J..
-00000f20: e44c c268 b636 c152 e2cb 4c96 a2a8 3219  .L.h.6.R..L...2.
-00000f30: 8a2a 9670 5a20 e2c9 206d 6956 7db0 4f4e  .*.pZ .. miV}.ON
-00000f40: b4e7 7917 37f7 45ae cde3 09ae df0c 7078  ..y.7.E.......px
-00000f50: 74fe 0150 4b03 0414 0000 0008 00d0 4e68  t..PK.........Nh
-00000f60: 5665 9079 9219 0100 00cf 0300 0013 0000  Ve.y............
-00000f70: 005b 436f 6e74 656e 745f 5479 7065 735d  .[Content_Types]
-00000f80: 2e78 6d6c ad93 4d4e c330 1085 af12 655b  .xml..MN.0....e[
-00000f90: 252e 2c58 a0a6 1b60 0b5d 7001 634f 1aab  %.,X...`.]p.cO..
-00000fa0: fe93 675a d2db 334e da4a a012 1585 4dac  ..gZ..3N.J....M.
-00000fb0: 78de bccf 9e97 acde 8f11 b0e8 9df5 d894  x...............
-00000fc0: 1d51 7c14 0255 074e 621d 2278 aeb4 2139  .Q|..U.Nb."x..!9
-00000fd0: 49fc 9ab6 224a b593 5b10 f7cb e583 50c1  I..."J..[.....P.
-00000fe0: 1378 aa28 7b94 ebd5 33b4 726f a978 e979  .x.({...3.ro.x.y
-00000ff0: 1b4d f04d 99c0 6259 3c8d c2cc 6a4a 19a3  .M.M..bY<...jJ..
-00001000: 354a 12d7 c5c1 eb1f 94ea 44a8 b973 d060  5J........D..s.`
-00001010: 6722 2e58 508a ab84 5cf9 1d70 ea7b 3b40  g".XP...\..p.{;@
-00001020: 4a46 43b1 9189 5ea5 6395 e8ad 403a 5ac0  JFC...^.c...@:Z.
-00001030: 7ada e2ca 1943 db1a 053a a8bd e396 1a63  z....C...:.....c
-00001040: 02a9 b103 2067 ebd1 7431 4d26 9e30 8ccf  .... g..t1M&.0..
-00001050: bbd9 fcc1 660a c8ca 4d0a 1139 b104 7fc7  ....f...M..9....
-00001060: 9d23 c9dd 5564 2348 64a6 af78 21b2 f5ec  .#..Ud#Hd..x!...
-00001070: fb41 4e5b 83be 91cd e3fd 0c69 37e4 8162  .AN[.......i7..b
-00001080: 58e6 cff8 7bc6 17ff 1bce f111 c2ee bf3f  X...{..........?
-00001090: b1bc d64e 1a7f e68b e13f 5e7f 0150 4b01  ...N.....?^..PK.
-000010a0: 0214 0314 0000 0008 00d0 4e68 5607 414d  ..........NhV.AM
-000010b0: 6281 0000 00b1 0000 0010 0000 0000 0000  b...............
-000010c0: 0000 0000 0080 0100 0000 0064 6f63 5072  ...........docPr
-000010d0: 6f70 732f 6170 702e 786d 6c50 4b01 0214  ops/app.xmlPK...
-000010e0: 0314 0000 0008 00d0 4e68 569f ef9c 05ef  ........NhV.....
-000010f0: 0000 002b 0200 0011 0000 0000 0000 0000  ...+............
-00001100: 0000 0080 01af 0000 0064 6f63 5072 6f70  .........docProp
-00001110: 732f 636f 7265 2e78 6d6c 504b 0102 1403  s/core.xmlPK....
-00001120: 1400 0000 0800 d04e 6856 995c 9c23 1006  .......NhV.\.#..
-00001130: 0000 9c27 0000 1300 0000 0000 0000 0000  ...'............
-00001140: 0000 8001 cd01 0000 786c 2f74 6865 6d65  ........xl/theme
-00001150: 2f74 6865 6d65 312e 786d 6c50 4b01 0214  /theme1.xmlPK...
-00001160: 0314 0000 0008 00d0 4e68 5641 8d67 d766  ........NhVA.g.f
-00001170: 0100 00c7 0200 0018 0000 0000 0000 0000  ................
-00001180: 0000 0080 810e 0800 0078 6c2f 776f 726b  .........xl/work
-00001190: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
-000011a0: 6c50 4b01 0214 0314 0000 0008 00d0 4e68  lPK...........Nh
-000011b0: 567c f3a3 dc51 0200 00f6 0900 000d 0000  V|...Q..........
-000011c0: 0000 0000 0000 0000 0080 01aa 0900 0078  ...............x
-000011d0: 6c2f 7374 796c 6573 2e78 6d6c 504b 0102  l/styles.xmlPK..
-000011e0: 1403 1400 0000 0800 d04e 6856 978a bb1c  .........NhV....
-000011f0: c000 0000 1302 0000 0b00 0000 0000 0000  ................
-00001200: 0000 0000 8001 260c 0000 5f72 656c 732f  ......&..._rels/
-00001210: 2e72 656c 7350 4b01 0214 0314 0000 0008  .relsPK.........
-00001220: 00d0 4e68 56d4 b000 a232 0100 0021 0200  ..NhV....2...!..
-00001230: 000f 0000 0000 0000 0000 0000 0080 010f  ................
-00001240: 0d00 0078 6c2f 776f 726b 626f 6f6b 2e78  ...xl/workbook.x
-00001250: 6d6c 504b 0102 1403 1400 0000 0800 d04e  mlPK...........N
-00001260: 6856 241e 9ba2 ad00 0000 f801 0000 1a00  hV$.............
-00001270: 0000 0000 0000 0000 0000 8001 6e0e 0000  ............n...
-00001280: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
-00001290: 6b2e 786d 6c2e 7265 6c73 504b 0102 1403  k.xml.relsPK....
-000012a0: 1400 0000 0800 d04e 6856 6590 7992 1901  .......NhVe.y...
-000012b0: 0000 cf03 0000 1300 0000 0000 0000 0000  ................
-000012c0: 0000 8001 530f 0000 5b43 6f6e 7465 6e74  ....S...[Content
-000012d0: 5f54 7970 6573 5d2e 786d 6c50 4b05 0600  _Types].xmlPK...
-000012e0: 0000 0009 0009 003e 0200 009d 1000 0000  .......>........
-000012f0: 00                                       .
+00000840: 2e78 6d6c 7552 d14e c330 0cfc 952a 1f40  .xmluR.N.0...*.@
+00000850: 36a4 019a da4a 6c13 8207 a469 13f0 88b2  6....Jl....i....
+00000860: d56d a325 7149 5c0a 7f4f dcad d590 b6a7  .m.%qI\..O......
+00000870: dace ddd9 e73a edd0 1f42 0d40 c98f 352e  .....:...B.@..5.
+00000880: 64a2 266a e652 867d 0d56 851b 6cc0 c597  d.&j.R.}.V..l...
+00000890: 12bd 5514 535f c9d0 7850 454f b246 de4e  ..U.S_..xPEO.F.N
+000008a0: 2677 d22a ed44 9ef6 b5b5 cf53 6cc9 6807  &w.*.D.....Sl.h.
+000008b0: 6b9f 84d6 5ae5 7f17 60b0 cbc4 540c 858d  k...Z...`...T...
+000008c0: ae6a e282 ccd3 4655 b005 7a6b d63e 6672  .j....FU..zk.>fr
+000008d0: 5429 b405 1734 bac4 4399 89c7 e97c d5e3  T)...4..C....|..
+000008e0: 7bc0 bb86 2e9c c509 3bd9 211e 3879 2932  {.......;.!.8y)2
+000008f0: 31e1 81c0 c09e 5841 c5cf 372c c118 168a  1.....XA..7,....
+00000900: 637c 9d34 c5d8 9289 e7f1 a0fe d47b 8f5e  c|.4.........{.^
+00000910: 762a c012 cd87 2ea8 cec4 8348 0a28 556b  v*.........H.(Uk
+00000920: 6883 dd33 9cfc ccc6 0157 8a54 9e7a ec12  h..3.....W.T.z..
+00000930: cf3e f374 cf01 f78e 38ed 783f 5bf2 b1ae  .>.t....8.x?[...
+00000940: 6323 ca9d b290 4a8a 0370 2ef7 27fc e21a  c#....J..p..'...
+00000950: be83 1def ed02 6579 95a2 0fba 8142 abcf  ......ey.....B..
+00000960: d69b 0bc4 d535 e21a 9bd6 28de e37f 968c  .....5....(.....
+00000970: ee86 8d1d edf2 48af ca57 da85 c440 19d5  ......H..W...@..
+00000980: 2637 f733 91f8 e37a 8e09 61d3 9fc2 0e89  &7.3...z..a.....
+00000990: d0f6 611d 2f0a 3c03 e27b 8948 43c2 7f67  ..a./.<..{.HC..g
+000009a0: bcd1 fc0f 504b 0304 1400 0000 0800 783b  ....PK........x;
+000009b0: 7756 7cf3 a3dc 5102 0000 f609 0000 0d00  wV|...Q.........
+000009c0: 0000 786c 2f73 7479 6c65 732e 786d 6cdd  ..xl/styles.xml.
+000009d0: 56db 8adb 3010 fd15 e10f a893 9835 7149  V...0........5qI
+000009e0: f250 4360 a12d 0bbb 0f7d 5562 3911 e8e2  .PC`.-...}Ub9...
+000009f0: caf2 92f4 eb3b 2339 76b3 ab59 287d ab4d  .....;#9v..Y(}.M
+00000a00: f0cc 1c9d b91b 67d3 fbab 12cf 6721 3cbb  ......g.....g!<.
+00000a10: 6865 fa6d 76f6 befb 9ce7 fdf1 2c34 ef3f  he.mv.......,4.?
+00000a20: d94e 1840 5aeb 34f7 a0ba 53de 774e f0a6  .N.@Z.4...S.wN..
+00000a30: 4792 56f9 6ab1 2873 cda5 c976 1b33 e8bd  G.V.j.(s...v.3..
+00000a40: f63d 3bda c1f8 6db6 c8f2 dda6 b566 b62c  .=;...m......f.,
+00000a50: b368 80a3 5c0b f6ca d536 abb9 9207 27c3  .h..\....6....'.
+00000a60: 59ae a5ba 46f3 0a0d 47ab ac63 1e52 1148  Y...F...G..c.R.H
+00000a70: 064b ff2b c2cb a861 96a3 1f2d 8d75 68cc  .K.+...a...-.uh.
+00000a80: 6384 f0e8 c1a9 546a 4a60 9545 c36e d371  c.....TjJ`.E.n.q
+00000a90: ef85 337b 5002 2718 df41 6c94 5fae 1d64  ..3{P.'..Al._..d
+00000aa0: 7072 fcba 5c3d 6433 213c 20c8 c1ba 46b8  pr..\=d3!< ...F.
+00000ab0: bb3a a369 b751 a2f5 4070 f274 c6a7 b75d  .:.i.Q..@p.t...]
+00000ac0: 8ea0 f756 83d0 487e b286 871c 6e8c 5100  ...V..H~....n.Q.
+00000ad0: b747 a1d4 338e e847 7be7 fbd2 b2d8 ebc7  .G..3..G{.......
+00000ae0: 06db ccb0 d49b 0809 8d62 7413 15f4 ffa7  .........bt.....
+00000af0: b7e8 fb9f ddb2 4ebe 5aff 6580 6a4c d07f  ......N.Z.e.jL..
+00000b00: 0ed6 8b27 275a 7909 faa5 bd8f 3f85 0e89  ...''Zy.....?...
+00000b10: dc45 9fac 0c97 639b 7dc7 9d53 b30b 7618  .E....c.}..S..v.
+00000b20: a4f2 d28c da59 368d 30ef 6a03 f79e 1f60  .....Y6.0.j....`
+00000b30: a9ef fcc3 f946 b47c 50fe 6502 b7d9 2c7f  .....F.|P.e...,.
+00000b40: 138d 1c74 359d 7ac2 b2c6 53b3 fc15 67b8  ...t5.z...S...g.
+00000b50: 2ca7 cd84 58d2 34e2 229a 7a54 dde9 1044  ,...X.4.".zT...D
+00000b60: 0602 441d 2f24 bc45 f6e1 4a23 1427 6269  ..D./$.E..J#.'bi
+00000b70: 0431 2a0e 9501 c589 2c2a ceff 54cf 9aac  .1*.....,*..T...
+00000b80: 2762 546e eb24 b226 396b 9213 5929 a40e  'bTn.$.&9k..Y)..
+00000b90: 3715 27cd a9e0 4a57 5a55 4551 9654 47eb  7.'...JWZUEQ.TG.
+00000ba0: 3a99 414d f5ad 2cf1 97f6 46e5 860c 2a0e  :.AM..,...F...*.
+00000bb0: 46fa bb5e d3d3 a637 e4e3 3da0 66fa d186  F..^...7..=.f...
+00000bc0: 5095 d29b 4855 4af7 1a91 74df 9051 55e9  P...HUJ...t..QU.
+00000bd0: 6953 7190 414d 81da 1d8c 9f8e 833b 95e6  iSq.AM.......;..
+00000be0: 1405 4e95 ca8d 7a83 69a4 aa28 0477 31bd  ..N...z.i..(.w1.
+00000bf0: a365 4974 a7c4 3b3d 1fea 2d29 8aaa 4a23  .eIt..;=..-)..J#
+00000c00: 88a5 3328 0a0a c1b7 9146 a80c 3007 0a29  ..3(.....F..0..)
+00000c10: 8af0 1d7c f33d ca6f dfa9 7cfe a7b7 fb0d  ...|.=.o..|.....
+00000c20: 504b 0304 1400 0000 0800 783b 7756 978a  PK........x;wV..
+00000c30: bb1c c000 0000 1302 0000 0b00 0000 5f72  .............._r
+00000c40: 656c 732f 2e72 656c 739d 92b9 6ec3 300c  els/.rels...n.0.
+00000c50: 407f c5d0 9e30 07d0 2188 3365 f116 04f9  @....0..!.3e....
+00000c60: 0156 a20f d812 058a 459d bfaf daa5 7190  .V......E.....q.
+00000c70: 0b19 793d 3c12 dc1e 6940 ed38 a4b6 8ba9  ..y=<...i@.8....
+00000c80: 18fd 1052 695a d5b8 0148 b625 8f69 ce91  ...RiZ...H.%.i..
+00000c90: 42ae d42c 1e35 87d2 4044 db63 43b0 5a2c  B..,.5..@D.cC.Z,
+00000ca0: 3e40 2e19 66b7 bd64 16a7 73a4 5788 5cd7  >@..f..d..s.W.\.
+00000cb0: 9da5 3ddb 2f4f 416f 80af 3a4c 7142 6948  ..=./OAo..:LqBiH
+00000cc0: 4b33 0ef0 cdd2 7f32 f7f3 0c35 45e5 4a23  K3.....2...5E.J#
+00000cd0: 955b 1a78 d3e5 fe76 e049 d1a1 2258 169a  .[.x...v.I.."X..
+00000ce0: 45c9 d3a2 1da5 7f1d c7f6 90d3 e9af 6322  E.............c"
+00000cf0: b47a 5be8 f971 6854 0a8e dc63 258c 7162  .z[..qhT...c%.qb
+00000d00: b4fe 3582 c90f ec7e 0050 4b03 0414 0000  ..5....~.PK.....
+00000d10: 0008 0078 3b77 56d4 b000 a232 0100 0021  ...x;wV....2...!
+00000d20: 0200 000f 0000 0078 6c2f 776f 726b 626f  .......xl/workbo
+00000d30: 6f6b 2e78 6d6c 8d51 d16a c240 10fc 9570  ok.xml.Q.j.@...p
+00000d40: 1fd0 4469 858a f145 692b 9456 6af1 fd4c  ..Di...Ei+.Vj..L
+00000d50: 3666 f1ee 36ec 6db4 f5eb bb49 0815 fad2  6f..6.m....I....
+00000d60: a7bd 9d59 8699 b9c5 85f8 7420 3a25 5fde  ...Y......t :%_.
+00000d70: 8598 9b5a a499 a769 2c6a f036 de51 0341  ...Z...i,j.6.Q.A
+00000d80: 998a d85b d195 8f69 6c18 6c19 6b00 f12e  ...[...il.l.k...
+00000d90: 9d66 d92c f516 8359 2e46 ad2d a7b7 0b09  .f.,...Y.F.-....
+00000da0: 1482 1414 ec80 3dc2 25fe f2dd 9a9c 31e2  ......=.%.....1.
+00000db0: 011d ca77 6efa b703 9378 0ce8 f10a 656e  ...wn....x....en
+00000dc0: 3293 c49a 2e2f c478 a520 d6ed 0a26 e772  2..../.x. ...&.r
+00000dd0: 3319 883d b060 f107 de75 263f ed21 f688  3..=.`...u&?.!..
+00000de0: d8c3 8755 23b9 9965 2a58 2147 e92f 7a7d  ...U#..e*X!G./z}
+00000df0: ab1e cfa0 c7c3 d60a 3da1 13e0 b515 7866  ........=.....xf
+00000e00: 6a1b 0cc7 4e46 53a4 3731 fa1e c639 9438  j...NFS.71...9.8
+00000e10: e7ff d448 5585 05ac a968 3d04 197a 6470  ...HU....h=..zdp
+00000e20: 9dc1 106b 6ca2 4982 f590 9b95 b6d2 c551  ...kl.I........Q
+00000e30: fd4d 3944 13f5 7453 14cf 5109 de94 83bb  .M9D..tS..Q.....
+00000e40: d152 0915 0628 df54 252a aef5 145b 4eba  .R...(.T%*...[N.
+00000e50: d1eb 4cef 1f26 8f5a 43eb dc4a b1f7 f04a  ..L..&.ZC..J...J
+00000e60: b61c 138e bfb3 fc01 504b 0304 1400 0000  ........PK......
+00000e70: 0800 783b 7756 241e 9ba2 ad00 0000 f801  ..x;wV$.........
+00000e80: 0000 1a00 0000 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
+00000e90: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
+00000ea0: b591 3d0e 8330 0c85 af12 e500 3550 a943  ..=..0......5P.C
+00000eb0: 054c 5d58 2b2e 1005 f323 1212 c5ae 0ab7  .L]X+....#......
+00000ec0: 2f85 0190 3a74 61b2 9e2d 7fef c94e 9f68  /...:ta..-...N.h
+00000ed0: 1477 6ea0 b6f3 2446 6b06 ca64 cbec ef00  .wn...$Fk..d....
+00000ee0: a45b b48a 2ece e330 4f6a 17ac e259 8606  .[.....0Oj...Y..
+00000ef0: bcd2 bd6a 1092 28ba 41d8 3364 9eee 99a2  ...j..(.A.3d....
+00000f00: 9c3c fe43 7475 dd69 7c38 fdb2 38f0 0f30  .<.Ctu.i|8..8..0
+00000f10: bc5d e8a9 4564 294a 151a e44c c268 b636  .]..Ed)J...L.h.6
+00000f20: c152 e2cb 4c96 a2a8 3219 8a2a 9670 5a20  .R..L...2..*.pZ 
+00000f30: e2c9 206d 6956 7db0 4f4e b4e7 7917 37f7  .. miV}.ON..y.7.
+00000f40: 45ae cde3 09ae df0c 7078 74fe 0150 4b03  E.......pxt..PK.
+00000f50: 0414 0000 0008 0078 3b77 5665 9079 9219  .......x;wVe.y..
+00000f60: 0100 00cf 0300 0013 0000 005b 436f 6e74  ...........[Cont
+00000f70: 656e 745f 5479 7065 735d 2e78 6d6c ad93  ent_Types].xml..
+00000f80: 4d4e c330 1085 af12 655b 252e 2c58 a0a6  MN.0....e[%.,X..
+00000f90: 1b60 0b5d 7001 634f 1aab fe93 675a d2db  .`.]p.cO....gZ..
+00000fa0: 334e da4a a012 1585 4dac 78de bccf 9e97  3N.J....M.x.....
+00000fb0: acde 8f11 b0e8 9df5 d894 1d51 7c14 0255  ...........Q|..U
+00000fc0: 074e 621d 2278 aeb4 2139 49fc 9ab6 224a  .Nb."x..!9I..."J
+00000fd0: b593 5b10 f7cb e583 50c1 1378 aa28 7b94  ..[.....P..x.({.
+00000fe0: ebd5 33b4 726f a978 e979 1b4d f04d 99c0  ..3.ro.x.y.M.M..
+00000ff0: 6259 3c8d c2cc 6a4a 19a3 354a 12d7 c5c1  bY<...jJ..5J....
+00001000: eb1f 94ea 44a8 b973 d060 6722 2e58 508a  ....D..s.`g".XP.
+00001010: ab84 5cf9 1d70 ea7b 3b40 4a46 43b1 9189  ..\..p.{;@JFC...
+00001020: 5ea5 6395 e8ad 403a 5ac0 7ada e2ca 1943  ^.c...@:Z.z....C
+00001030: db1a 053a a8bd e396 1a63 02a9 b103 2067  ...:.....c.... g
+00001040: ebd1 7431 4d26 9e30 8ccf bbd9 fcc1 660a  ..t1M&.0......f.
+00001050: c8ca 4d0a 1139 b104 7fc7 9d23 c9dd 5564  ..M..9.....#..Ud
+00001060: 2348 64a6 af78 21b2 f5ec fb41 4e5b 83be  #Hd..x!....AN[..
+00001070: 91cd e3fd 0c69 37e4 8162 58e6 cff8 7bc6  .....i7..bX...{.
+00001080: 17ff 1bce f111 c2ee bf3f b1bc d64e 1a7f  .........?...N..
+00001090: e68b e13f 5e7f 0150 4b01 0214 0314 0000  ...?^..PK.......
+000010a0: 0008 0078 3b77 5607 414d 6281 0000 00b1  ...x;wV.AMb.....
+000010b0: 0000 0010 0000 0000 0000 0000 0000 0080  ................
+000010c0: 0100 0000 0064 6f63 5072 6f70 732f 6170  .....docProps/ap
+000010d0: 702e 786d 6c50 4b01 0214 0314 0000 0008  p.xmlPK.........
+000010e0: 0078 3b77 56c5 f282 33ef 0000 002b 0200  .x;wV...3....+..
+000010f0: 0011 0000 0000 0000 0000 0000 0080 01af  ................
+00001100: 0000 0064 6f63 5072 6f70 732f 636f 7265  ...docProps/core
+00001110: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00001120: 783b 7756 995c 9c23 1006 0000 9c27 0000  x;wV.\.#.....'..
+00001130: 1300 0000 0000 0000 0000 0000 8001 cd01  ................
+00001140: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
+00001150: 312e 786d 6c50 4b01 0214 0314 0000 0008  1.xmlPK.........
+00001160: 0078 3b77 56e4 d3df f060 0100 00af 0200  .x;wV....`......
+00001170: 0018 0000 0000 0000 0000 0000 0080 810e  ................
+00001180: 0800 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00001190: 2f73 6865 6574 312e 786d 6c50 4b01 0214  /sheet1.xmlPK...
+000011a0: 0314 0000 0008 0078 3b77 567c f3a3 dc51  .......x;wV|...Q
+000011b0: 0200 00f6 0900 000d 0000 0000 0000 0000  ................
+000011c0: 0000 0080 01a4 0900 0078 6c2f 7374 796c  .........xl/styl
+000011d0: 6573 2e78 6d6c 504b 0102 1403 1400 0000  es.xmlPK........
+000011e0: 0800 783b 7756 978a bb1c c000 0000 1302  ..x;wV..........
+000011f0: 0000 0b00 0000 0000 0000 0000 0000 8001  ................
+00001200: 200c 0000 5f72 656c 732f 2e72 656c 7350   ..._rels/.relsP
+00001210: 4b01 0214 0314 0000 0008 0078 3b77 56d4  K..........x;wV.
+00001220: b000 a232 0100 0021 0200 000f 0000 0000  ...2...!........
+00001230: 0000 0000 0000 0080 0109 0d00 0078 6c2f  .............xl/
+00001240: 776f 726b 626f 6f6b 2e78 6d6c 504b 0102  workbook.xmlPK..
+00001250: 1403 1400 0000 0800 783b 7756 241e 9ba2  ........x;wV$...
+00001260: ad00 0000 f801 0000 1a00 0000 0000 0000  ................
+00001270: 0000 0000 8001 680e 0000 786c 2f5f 7265  ......h...xl/_re
+00001280: 6c73 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e  ls/workbook.xml.
+00001290: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
+000012a0: 783b 7756 6590 7992 1901 0000 cf03 0000  x;wVe.y.........
+000012b0: 1300 0000 0000 0000 0000 0000 8001 4d0f  ..............M.
+000012c0: 0000 5b43 6f6e 7465 6e74 5f54 7970 6573  ..[Content_Types
+000012d0: 5d2e 786d 6c50 4b05 0600 0000 0009 0009  ].xmlPK.........
+000012e0: 003e 0200 0097 1000 0000 00              .>.........
```

### Comparing `pymetamodel-0.2.7/examples/city/city.yaml` & `pymetamodel-0.3.0/examples/city/city.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -9,99 +9,78 @@
     prefix_reference: GeneralContext/
   xsd:
     prefix_prefix: xsd
     prefix_reference: http://www.w3.org/2001/XMLSchema#
   shex:
     prefix_prefix: shex
     prefix_reference: http://www.w3.org/ns/shex#
-  schema:
-    prefix_prefix: schema
-    prefix_reference: http://schema.org/
 default_prefix: GeneralContext
 default_range: string
 types:
   string:
     name: string
     description: A character string
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Text
     base: str
     uri: xsd:string
   integer:
     name: integer
     description: An integer
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Integer
     base: int
     uri: xsd:integer
   boolean:
     name: boolean
     description: A binary (true or false) value
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Boolean
     base: Bool
     uri: xsd:boolean
     repr: bool
   float:
     name: float
     description: A real number that conforms to the xsd:float specification
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Float
     base: float
     uri: xsd:float
   double:
     name: double
     description: A real number that conforms to the xsd:double specification
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:Float
     base: float
     uri: xsd:double
   decimal:
     name: decimal
     description: A real number with arbitrary precision that conforms to the xsd:decimal
       specification
     from_schema: https://w3id.org/linkml/types
-    broad_mappings:
-    - schema:Number
     base: Decimal
     uri: xsd:decimal
   time:
     name: time
     description: A time object represents a (local) time of day, independent of any
       particular day
     notes:
-    - URI is dateTime because OWL reasoners do not work with straight date or time
+    - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Time
     base: XSDTime
     uri: xsd:dateTime
     repr: str
   date:
     name: date
     description: a date (year, month and day) in an idealized calendar
     notes:
     - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Date
     base: XSDDate
     uri: xsd:date
     repr: str
   datetime:
     name: datetime
     description: The combination of a date and time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:DateTime
     base: XSDDateTime
     uri: xsd:dateTime
     repr: str
   date_or_datetime:
     name: date_or_datetime
     description: Either a date or a datetime
     from_schema: https://w3id.org/linkml/types
@@ -111,36 +90,18 @@
   uriorcurie:
     name: uriorcurie
     description: a URI or a CURIE
     from_schema: https://w3id.org/linkml/types
     base: URIorCURIE
     uri: xsd:anyURI
     repr: str
-  curie:
-    name: curie
-    conforms_to: https://www.w3.org/TR/curie/
-    description: a compact URI
-    comments:
-    - in RDF serializations this MUST be expanded to a URI
-    - in non-RDF serializations MAY be serialized as the compact representation
-    from_schema: https://w3id.org/linkml/types
-    base: Curie
-    uri: xsd:string
-    repr: str
   uri:
     name: uri
-    conforms_to: https://www.ietf.org/rfc/rfc3987.txt
     description: a complete URI
-    comments:
-    - in RDF serializations a slot with range of uri is treated as a literal or type
-      xsd:anyURI unless it is an identifier or a reference to an identifier, in which
-      case it is translated directly to a node
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:URL
     base: URI
     uri: xsd:anyURI
     repr: str
   ncname:
     name: ncname
     description: Prefix part of CURIE
     from_schema: https://w3id.org/linkml/types
```

### Comparing `pymetamodel-0.2.7/examples/family/FamilyContext.mermaid` & `pymetamodel-0.3.0/examples/family/FamilyContext.mermaid`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/family/FamilyContext.puml` & `pymetamodel-0.3.0/examples/family/FamilyContext.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/family/FamilyContext.py` & `pymetamodel-0.3.0/examples/family/FamilyContext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from FamilyContext.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-08T09:54:40
+# Generation date: 2023-03-23T07:27:54
 # Schema: FamilyContext
 #
 # id: FamilyContext
 # description:
 # license:
 
 import dataclasses
@@ -18,26 +18,25 @@
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
 from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
 from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.metamodelcore import Bool, Curie, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
+from linkml_runtime.utils.metamodelcore import Bool, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
 FAMILYCONTEXT = CurieNamespace('FamilyContext', 'FamilyContext/')
 LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
-SCHEMA = CurieNamespace('schema', 'http://schema.org/')
 SHEX = CurieNamespace('shex', 'http://www.w3.org/ns/shex#')
 XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = FAMILYCONTEXT
 
 
 # Types
 class String(str):
@@ -124,22 +123,14 @@
     """ a URI or a CURIE """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uriorcurie"
     type_model_uri = FAMILYCONTEXT.Uriorcurie
 
 
-class Curie(Curie):
-    """ a compact URI """
-    type_class_uri = XSD.string
-    type_class_curie = "xsd:string"
-    type_name = "curie"
-    type_model_uri = FAMILYCONTEXT.Curie
-
-
 class Uri(URI):
     """ a complete URI """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uri"
     type_model_uri = FAMILYCONTEXT.Uri
```

### Comparing `pymetamodel-0.2.7/examples/family/FamilyContext.sidif` & `pymetamodel-0.3.0/examples/family/FamilyContext.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/family/FamilyContext.xlsx` & `pymetamodel-0.3.0/examples/family/FamilyContext.xlsx`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 504b 0304 1400 0000 0800 d44e 6856 0741  PK.........NhV.A
+00000000: 504b 0304 1400 0000 0800 7b3b 7756 0741  PK........{;wV.A
 00000010: 4d62 8100 0000 b100 0000 1000 0000 646f  Mb............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 3d0b 0231 1044 ffca 71bd b741 c142 6240  =..1.D..q..A.Bb@
 00000040: d052 b0b2 0f7b 1b2f 9064 43b2 427e be39  .R...{./.dC.B~.9
 00000050: c18f 6e1e 6f18 46df 0a67 2ae2 a90e 2d86  ..n.o.F..g*...-.
 00000060: 548f e322 920f 0015 178a b64e 5da7 6e1c  T..".......N].n.
 00000070: 9768 a563 7900 3be7 91ce 8ccf 4849 60ab  .h.cy.;.....HI`.
 00000080: d41e a809 a599 e64d fe0e 8e46 9f72 0e1e  .......M...F.r..
 00000090: ad78 4ee6 eab1 7065 27c3 a521 050d ff72  .xN...pe'..!...r
 000000a0: 6dde a9d4 35ef 26f5 961f d6f0 3b69 5e50  m...5.&.....;i^P
-000000b0: 4b03 0414 0000 0008 00d4 4e68 5625 b4c1  K.........NhV%..
-000000c0: 96ef 0000 002b 0200 0011 0000 0064 6f63  .....+.......doc
+000000b0: 4b03 0414 0000 0008 007b 3b77 5680 76fe  K........{;wV.v.
+000000c0: 74ef 0000 002b 0200 0011 0000 0064 6f63  t....+.......doc
 000000d0: 5072 6f70 732f 636f 7265 2e78 6d6c cd92  Props/core.xml..
-000000e0: 514b c330 10c7 bf8a e4bd bdb4 9d32 42d7  QK.0.........2B.
-000000f0: 17c5 2705 c181 e25b 486e 5b58 9386 e4a4  ..'....[Hn[X....
-00000100: ddb7 378d 5b87 e807 10f2 92bb 7f7e f73b  ..7.[........~.;
-00000110: 48ab bc50 43c0 9730 780c 6430 de4c b677  H..PC..0x.d0.L.w
-00000120: 5128 bf61 0722 2f00 a23a a095 b14c 0997  Q(.a."/..:...L..
-00000130: 9abb 2158 49e9 1af6 e0a5 3aca 3d42 cdf9  ..!XI.....:.=B..
-00000140: 1d58 24a9 2549 9881 855f 88ac 6bb5 122a  .X$.%I..._..k..*
-00000150: a0a4 219c f15a 2d78 ff19 fa0c d30a b047  ..!..Z-x.......G
-00000160: 8b8e 2254 6505 ac9b 27fa d3d4 b770 05cc  .."Te...'....p..
-00000170: 30c2 60e3 7701 f542 ccd5 3fb1 b903 ec9c  0.`.w..B..?.....
-00000180: 9ca2 5952 e338 9663 9373 6987 0ade 9f9f  ..YR.8.c.si.....
-00000190: 5ef3 ba85 7191 a453 985e 4523 e8e4 71c3  ^...q..S.^E#..q.
-000001a0: 2e93 df9a fb87 ed23 eb6a 5e37 054f 67bd  .......#.j^7.Og.
-000001b0: e56b 71bb 12ab ea63 76fd e177 15b6 8336  .kq....cv..w...6
-000001c0: 3bf3 8f8d 2f82 5d0b bffe 45f7 0550 4b03  ;.../.]...E..PK.
-000001d0: 0414 0000 0008 00d4 4e68 5699 5c9c 2310  ........NhV.\.#.
+000000e0: cf4a 0331 1087 5f45 72df 9dfd a315 c236  .J.1.._Er......6
+000000f0: 174b 4f0a 8205 c55b 48a6 6d70 930d c9c8  .KO....[H.mp....
+00000100: 6edf de6c 6cb7 883e 80c7 ccfc f2cd 3730  n..ll..>......70
+00000110: 9df2 5c0d 019f c3e0 3190 c178 33d9 de45  ..\.....1..x3..E
+00000120: aefc 9a1d 893c 0788 ea88 56c6 3225 5c6a  .....<....V.2%\j
+00000130: ee87 6025 a567 3880 97ea 431e 109a aa5a  ..`%.g8...C....Z
+00000140: 8145 925a 9284 1958 f885 c844 a715 5701  .E.Z...X...D..W.
+00000150: 250d e18c d76a c1fb cfd0 6798 5680 3d5a  %....j....g.V.=Z
+00000160: 7414 a12e 6b60 629e e84f 53df c115 30c3  t...k`b..OS...0.
+00000170: 0883 8ddf 05d4 0b31 57ff c4e6 0eb0 7372  .......1W.....sr
+00000180: 8a66 498d e358 8e6d cea5 1d6a 787b 7a7c  .fI..X.m...jx{z|
+00000190: c9eb 16c6 4592 4e61 fa15 0da7 93c7 35bb  ....E.Na......5.
+000001a0: 4c7e 6d1f 36bb 2d13 4dd5 b445 d516 4dbb  L~m.6.-.M..E..M.
+000001b0: ab56 bcb9 e777 b7ef b3eb 0fbf abb0 1db4  .V...w..........
+000001c0: d99b 7f6c 7c11 141d fcba 0bf1 0550 4b03  ...l|........PK.
+000001d0: 0414 0000 0008 007b 3b77 5699 5c9c 2310  .......{;wV.\.#.
 000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
 000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
 00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
 00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
 00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
 00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
 00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
@@ -123,224 +123,223 @@
 000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
 000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
 000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
 000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
 000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
 000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
 00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
-00000810: 0304 1400 0000 0800 d44e 6856 fd24 4c60  .........NhV.$L`
-00000820: 8d01 0000 c603 0000 1800 0000 786c 2f77  ............xl/w
+00000810: 0304 1400 0000 0800 7b3b 7756 34f8 2c6d  ........{;wV4.,m
+00000820: 8301 0000 8603 0000 1800 0000 786c 2f77  ............xl/w
 00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00000840: 2e78 6d6c 8d93 db4e e430 0c86 5fa5 ca03  .xml...N.0.._...
-00000850: 9061 250e 426d 2518 0eb3 172b 4620 964b  .a%.Bm%....+F .K
-00000860: 9469 dc36 2289 8be3 a1cc db93 740e 42a8  .i.6".......t.B.
-00000870: a85c d576 fcfd b653 27ef 915e 430b c0d9  .\.v...S'..^C...
-00000880: 87b3 3e14 a265 ee2e a40c 550b 4e85 23ec  ..>..e....U.N.#.
-00000890: c0c7 931a c929 8e2e 3532 7404 4a0f 90b3  .....)..52t.J...
-000008a0: f2cf 6c76 2a9d 325e 94f9 105b 5299 e39a  ..lv*.2^...[R...
-000008b0: adf1 b0a4 2cac 9d53 b4b9 028b 7d21 8ec5  ....,..S....}!..
-000008c0: 3ef0 609a 9653 4096 79a7 1a78 047e ea96  >.`..S@.y..x.~..
-000008d0: 143d 7950 d1c6 810f 067d 4650 17e2 f2f8  .=yP.....}FP....
-000008e0: 6231 e40f 09ff 0df4 e18b 9da5 4956 88af  b1..........IV..
-000008f0: c9f9 ab0b 314b 0d81 858a 9382 8a9f 7798  ....1K........w.
-00000900: 83b5 4928 b6f1 b6d3 1487 9209 fc6a efd5  ..I(.........j..
-00000910: 6f87 d9e3 2c2b 1560 8ef6 d968 6e0b 712e  o...,+.`...hn.q.
-00000920: 320d b55a 5b7e c07e 01bb 794e 0e0d 5e2b  2..Z[~.~..yN..^+
-00000930: 5665 4ed8 6794 e62c f32a 19a9 76cc 333e  VeN.g..,.*..v.3>
-00000940: ddcf 2353 8c9b 5888 cb5a 3963 372f 2f5e  ..#S..X..Z9c7//^
-00000950: 39c8 25c7 4652 5c56 3bee 6a8a eb41 6be3  9.%.FR\V;.j..Ak.
-00000960: 9b58 750c 9fff 125f 5a55 8df1 d753 fc06  .Xu...._ZU...S..
-00000970: 14fd 5344 06f4 087e 3385 3bf4 dcfe ccdf  ..SD...~3.;.....
-00000980: 4ef1 dabc 2355 a3ec dd14 dbae c34a 797d  N...#U.......Jy}
-00000990: 5f8f c08b c97b 3335 7c27 65fc e9fb 45da  _....{35|'e...E.
-000009a0: 6e41 daf0 385d 637c c82c d451 7176 7476  nA..8]c|.,.Qqvtv
-000009b0: 2232 da6e cdd6 61ec 8617 b242 6674 83d9  "2.n..a....Bft..
-000009c0: c687 0694 12e2 798d c87b 272d ede1 e996  ......y..{'-....
-000009d0: 9f50 4b03 0414 0000 0008 00d4 4e68 567a  .PK.........NhVz
-000009e0: efc8 e9e3 0100 003d 0600 0018 0000 0078  .......=.......x
-000009f0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00000a00: 6574 322e 786d 6c8d 95db 6ee2 3010 865f  et2.xml...n.0.._
-00000a10: 25ca 0334 b452 f750 8548 05b6 5b76 db6d  %..4.R.P.H..[v.m
-00000a20: 16f6 7059 9964 422c 6c4f 3a1e 36e5 ed6b  ..pY.dB,lO:.6..k
-00000a30: a780 aa95 2b73 c5cc d8df 9c64 fee4 3dd2  ....+s.....d..=.
-00000a40: c6b6 009c 3c6b 65ec 386d 99bb ab2c b355  ....<ke.8m...,.U
-00000a50: 0b5a d833 ecc0 b893 0649 0b76 2ead 33db  .Z.3.....I.v..3.
-00000a60: 1188 7a80 b4ca 2e46 a30f 9916 d2a4 453e  ..z....F......E>
-00000a70: c44a 2a72 dcb2 9206 4a4a ec56 6b41 bb09  .J*r....JJ.VkA..
-00000a80: 28ec c7e9 797a 082c e4ba 651f c88a bc13  (...yz.,..e.....
-00000a90: 6b58 02ff ee4a 725e 76cc 524b 0dc6 4a34  kX...Jr^v.RK..J4
-00000aa0: 0941 334e afcf af96 c3fd e1c2 1f09 bd7d  .A3N...........}
-00000ab0: 6327 7e92 15e2 c63b f37a 9c8e 7c43 a0a0  c'~....;.z..|C..
-00000ac0: 629f 41b8 9f7f 3005 a57c 22d7 c6d3 3e67  b.A...0..|"...>g
-00000ad0: 7a2c e9c1 b7f6 21fb cd30 bb9b 6525 2c4c  z,....!..0..e%,L
-00000ae0: 51fd 9535 b7e3 f453 9ad4 d088 ade2 05f6  Q..5...S........
-00000af0: b7b0 9fe7 f2d8 e04c b028 72c2 3e21 3f67  .......L.(r.>!?g
-00000b00: 9157 def0 b5dd 3d69 fc7e 964c 2e2e 5d21  .W....=i.~.L..]!
-00000b10: 2e3a 208b e6f1 f149 d679 c6ae 0f1f ceaa  .: ....I.y......
-00000b20: 3d36 8961 843b a13e 5f04 e169 0c36 4243  =6.a.;.>_..i.6BC
-00000b30: 809b 4539 5c29 f825 5985 e82f 31ba 9315  ..E9\).%Y../1...
-00000b40: 6f29 84de c450 0bcf 01ec 6b0c 5b21 9900  o)...P....k.[!..
-00000b50: 771b e376 2068 1266 e731 56a3 e1f6 1df8  w..v h.f.1V.....
-00000b60: 5bb4 6149 dc96 4a54 a12d 7d8f d1b5 84d0  [.aI..JT.-}.....
-00000b70: 73b8 3b85 bbe6 0079 7fca a266 e1aa 3f4e  s.;....y...f..?N
-00000b80: 5ad4 3bf0 43fc 25ce cd9d 3b0b b065 8ced  Z.;.C.%...;..e..
-00000b90: e546 9650 4b11 807f c6e0 aa95 aa7e 6802  .F.PK........~h.
-00000ba0: e822 fafe 0581 e120 bb8c fe01 3adc daff  ."..... ....:...
-00000bb0: a6cd 9cd6 1cf4 eb55 7cbc b0de 0b5a 4b63  .......U|....ZKc
-00000bc0: 1305 8dcb 383a fb78 9926 f42a 56af 0e63  ....8:.x.&.*V..c
-00000bd0: 3708 f30a 9951 0f66 ebf4 1dc8 5f70 e70d  7....Q.f...._p..
-00000be0: 221f 1caf 95c7 2f46 f102 504b 0304 1400  "...../F..PK....
-00000bf0: 0000 0800 d44e 6856 7cf3 a3dc 5102 0000  .....NhV|...Q...
-00000c00: f609 0000 0d00 0000 786c 2f73 7479 6c65  ........xl/style
-00000c10: 732e 786d 6cdd 56db 8adb 3010 fd15 e10f  s.xml.V...0.....
-00000c20: a893 9835 7149 f250 4360 a12d 0bbb 0f7d  ...5qI.PC`.-...}
-00000c30: 5562 3911 e8e2 caf2 92f4 eb3b 2339 76b3  Ub9........;#9v.
-00000c40: ab59 287d ab4d f0cc 1c9d b91b 67d3 fbab  .Y(}.M......g...
-00000c50: 12cf 6721 3cbb 6865 fa6d 76f6 befb 9ce7  ..g!<.he.mv.....
-00000c60: fdf1 2c34 ef3f d94e 1840 5aeb 34f7 a0ba  ..,4.?.N.@Z.4...
-00000c70: 53de 774e f0a6 4792 56f9 6ab1 2873 cda5  S.wN..G.V.j.(s..
-00000c80: c976 1b33 e8bd f63d 3bda c1f8 6db6 c8f2  .v.3...=;...m...
-00000c90: dda6 b566 b62c b368 80a3 5c0b f6ca d536  ...f.,.h..\....6
-00000ca0: abb9 9207 27c3 59ae a5ba 46f3 0a0d 47ab  ....'.Y...F...G.
-00000cb0: ac63 1e52 1148 064b ff2b c2cb a861 96a3  .c.R.H.K.+...a..
-00000cc0: 1f2d 8d75 68cc 6384 f0e8 c1a9 546a 4a60  .-.uh.c.....TjJ`
-00000cd0: 9545 c36e d371 ef85 337b 5002 2718 df41  .E.n.q..3{P.'..A
-00000ce0: 6c94 5fae 1d64 7072 fcba 5c3d 6433 213c  l._..dpr..\=d3!<
-00000cf0: 20c8 c1ba 46b8 bb3a a369 b751 a2f5 4070   ...F..:.i.Q..@p
-00000d00: f274 c6a7 b75d 8ea0 f756 83d0 487e b286  .t...]...V..H~..
-00000d10: 871c 6e8c 5100 b747 a1d4 338e e847 7be7  ..n.Q..G..3..G{.
-00000d20: fbd2 b2d8 ebc7 06db ccb0 d49b 0809 8d62  ...............b
-00000d30: 7413 15f4 ffa7 b7e8 fb9f ddb2 4ebe 5aff  t...........N.Z.
-00000d40: 6580 6a4c d07f 0ed6 8b27 275a 7909 faa5  e.jL.....''Zy...
-00000d50: bd8f 3f85 0e89 dc45 9fac 0c97 639b 7dc7  ..?....E....c.}.
-00000d60: 9d53 b30b 7618 a4f2 d28c da59 368d 30ef  .S..v......Y6.0.
-00000d70: 6a03 f79e 1f60 a9ef fcc3 f946 b47c 50fe  j....`.....F.|P.
-00000d80: 6502 b7d9 2c7f 138d 1c74 359d 7ac2 b2c6  e...,....t5.z...
-00000d90: 53b3 fc15 67b8 2ca7 cd84 58d2 34e2 229a  S...g.,...X.4.".
-00000da0: 7a54 dde9 1044 0602 441d 2f24 bc45 f6e1  zT...D..D./$.E..
-00000db0: 4a23 1427 6269 0431 2a0e 9501 c589 2c2a  J#.'bi.1*.....,*
-00000dc0: ceff 54cf 9aac 2762 546e eb24 b226 396b  ..T...'bTn.$.&9k
-00000dd0: 9213 5929 a40e 3715 27cd a9e0 4a57 5a55  ..Y)..7.'...JWZU
-00000de0: 4551 9654 47eb 3a99 414d f5ad 2cf1 97f6  EQ.TG.:.AM..,...
-00000df0: 46e5 860c 2a0e 46fa bb5e d3d3 a637 e4e3  F...*.F..^...7..
-00000e00: 3da0 66fa d186 5095 d29b 4855 4af7 1a91  =.f...P...HUJ...
-00000e10: 74df 9051 55e9 6953 7190 414d 81da 1d8c  t..QU.iSq.AM....
-00000e20: 9f8e 833b 95e6 1405 4e95 ca8d 7a83 69a4  ...;....N...z.i.
-00000e30: aa28 0477 31bd a365 4974 a7c4 3b3d 1fea  .(.w1..eIt..;=..
-00000e40: 2d29 8aaa 4a23 88a5 3328 0a0a c1b7 9146  -)..J#..3(.....F
-00000e50: a80c 3007 0a29 8af0 1d7c f33d ca6f dfa9  ..0..)...|.=.o..
-00000e60: 7cfe a7b7 fb0d 504b 0304 1400 0000 0800  |.....PK........
-00000e70: d44e 6856 978a bb1c c000 0000 1302 0000  .NhV............
-00000e80: 0b00 0000 5f72 656c 732f 2e72 656c 739d  ...._rels/.rels.
-00000e90: 92b9 6ec3 300c 407f c5d0 9e30 07d0 2188  ..n.0.@....0..!.
-00000ea0: 3365 f116 04f9 0156 a20f d812 058a 459d  3e.....V......E.
-00000eb0: bfaf daa5 7190 0b19 793d 3c12 dc1e 6940  ....q...y=<...i@
-00000ec0: ed38 a4b6 8ba9 18fd 1052 695a d5b8 0148  .8.......RiZ...H
-00000ed0: b625 8f69 ce91 42ae d42c 1e35 87d2 4044  .%.i..B..,.5..@D
-00000ee0: db63 43b0 5a2c 3e40 2e19 66b7 bd64 16a7  .cC.Z,>@..f..d..
-00000ef0: 73a4 5788 5cd7 9da5 3ddb 2f4f 416f 80af  s.W.\...=./OAo..
-00000f00: 3a4c 7142 6948 4b33 0ef0 cdd2 7f32 f7f3  :LqBiHK3.....2..
-00000f10: 0c35 45e5 4a23 955b 1a78 d3e5 fe76 e049  .5E.J#.[.x...v.I
-00000f20: d1a1 2258 169a 45c9 d3a2 1da5 7f1d c7f6  .."X..E.........
-00000f30: 90d3 e9af 6322 b47a 5be8 f971 6854 0a8e  ....c".z[..qhT..
-00000f40: dc63 258c 7162 b4fe 3582 c90f ec7e 0050  .c%.qb..5....~.P
-00000f50: 4b03 0414 0000 0008 00d4 4e68 56b4 8801  K.........NhV...
-00000f60: 5d47 0100 00af 0200 000f 0000 0078 6c2f  ]G...........xl/
-00000f70: 776f 726b 626f 6f6b 2e78 6d6c b552 d16a  workbook.xml.R.j
-00000f80: c330 0cfc 95e0 0f58 dab2 1556 9abd ac74  .0.....X...V...t
-00000f90: 2b8c adac a3ef 4ea2 34a2 b615 64a7 5dfb  +.....N.4...d.].
-00000fa0: f553 1cc2 0283 b197 3dd9 ba13 f2dd c9cb  .S......=.......
-00000fb0: 33f1 3127 3a26 9fd6 389f a93a 8466 91a6  3.1':&..8..:.f..
-00000fc0: bea8 c16a 7f43 0d38 612a 62ab 8394 7c48  ...j.C.8a*b...|H
-00000fd0: 7dc3 a04b 5f03 046b d2d9 6432 4fad 46a7  }..K_..k..d2O.F.
-00000fe0: 1e96 c3ac 2da7 e382 0214 01c9 09d8 017b  ....-..........{
-00000ff0: 84b3 ffe6 bb32 39a1 c71c 0d86 4ba6 e2dd  .....29.....K...
-00001000: 804a 2c3a b478 8532 5313 95f8 9ace cfc4  .J,:.x.2S.......
-00001010: 7825 17b4 d915 4cc6 646a da13 7be0 80c5  x%....L.dj..{...
-00001020: 0f78 d789 fcd0 b98f 48d0 f9bb 1621 999a  .x......H....!..
-00001030: 4f64 6085 ec43 ec88 f3b5 683c 8134 c75e  Od`..C....h<.4.^
-00001040: dd06 5aa3 09c0 2b1d e089 a96d d01d 3a4a  ..Z...+....m..:J
-00001050: 5ca4 231b 3187 e1ec 435c f05f 62a4 aac2  \.#.1...C\._b...
-00001060: 0256 54b4 165c e873 6430 9d40 e76b 6cbc  .VT..\.sd0.@.kl.
-00001070: 4a9c b690 a9b5 b668 2e9d 2179 6153 f6e6  J......h..!yaS..
-00001080: 82a8 1a45 c50b 1482 3765 d4f7 7f5a b6c0  ...E....7e...Z..
-00001090: 9edc 48cb ec17 2db3 98d5 1050 0915 3a28  ..H...-....P..:(
-000010a0: 5f65 8e17 5c96 556c 39e9 8ee8 6976 7b37  _e..\.Ul9...iv{7
-000010b0: bd97 a5b4 c63c 0af6 e65e 4897 43de c35f  .....<...^H.C.._
-000010c0: 79f8 0250 4b03 0414 0000 0008 00d4 4e68  y..PK.........Nh
-000010d0: 568d f72c 5ab4 0000 0089 0200 001a 0000  V..,Z...........
-000010e0: 0078 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
-000010f0: 6f6b 2e78 6d6c 2e72 656c 73c5 924d 0a83  ok.xml.rels..M..
-00001100: 3010 46af 1272 808e dad2 4551 57dd b82d  0.F..r....EQW..-
-00001110: 5e20 e8f8 83d1 84cc 94ea ed6b 75a1 812e  ^ .........ku...
-00001120: ba91 aec2 3721 ef7b 3089 1fa8 15b7 66a0  ....7!.{0.....f.
-00001130: a6b5 24c6 5e0f 94c8 86d9 de00 a868 b057  ..$.^........h.W
-00001140: 7432 1687 f9a6 32ae 573c 4757 8355 45a7  t2....2.W<GW.UE.
-00001150: 6a84 2808 aee0 f60c 99c6 7ba6 c827 8bbf  j.(.......{..'..
-00001160: 104d 55b5 05de 4df1 ec71 e02f 6078 19d7  .MU...M..q./`x..
-00001170: 5183 c852 e4ca d5c8 8984 516f 6382 e508  Q..R......Qoc...
-00001180: 4f33 598a ac4c a4cb ca50 c2bf 8522 4f28  O3Y..L...P..."O(
-00001190: 3a50 8878 d248 9bcd 9abd faf3 81f5 3cbf  :P.x.H........<.
-000011a0: c5ad 7d89 ebd0 dfc9 e5e3 00de cf4b df50  ..}..........K.P
-000011b0: 4b03 0414 0000 0008 00d4 4e68 566e a724  K.........NhVn.$
-000011c0: bc1e 0100 0057 0400 0013 0000 005b 436f  .....W.......[Co
-000011d0: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-000011e0: c594 cf4e c330 0cc6 5fa5 ca75 6a32 76e0  ...N.0.._..uj2v.
-000011f0: 80d6 5d80 2bec c00b 84d6 5da3 e69f 626f  ..].+.....]...bo
-00001200: 746f 8fdb 6e93 40a3 622a 1297 468d edef  to..n.@.b*..F...
-00001210: e7f8 8bb2 7e3b 46c0 ac73 d663 211a a2f8  ....~;F..s.c!...
-00001220: a014 960d 388d 3244 f01c a943 729a f837  ....8.2D...Cr..7
-00001230: ed54 d465 ab77 a056 cbe5 bd2a 8327 f094  .T.e.w.V...*.'..
-00001240: 53af 2136 eb27 a8f5 de52 f6dc f136 9ae0  S.!6.'...R...6..
-00001250: 0b91 c0a2 c81e c7c4 9e55 081d a335 a526  .........U...5.&
-00001260: 8eab 83af be51 f213 4172 e590 838d 89b8  .....Q..Ar......
-00001270: e004 a1ae 12fa c8cf 8053 ddeb 0152 3215  .........S...R2.
-00001280: 645b 9de8 453b ce52 9d55 4847 0b28 a725  d[..E;.R.UHG.(.%
-00001290: aef4 18ea da94 5085 72ef b844 624c a02b  ......P.r..DbL.+
-000012a0: 6c00 c859 398a 2ea6 c9c4 1386 f17b 379b  l..Y9........{7.
-000012b0: 3fc8 4c01 3973 9b42 4476 2cc1 edb8 b325  ?.L.9s.BDv,....%
-000012c0: 7d75 1e59 0812 99e9 235e 882c 3dfb 7cd0  }u.Y....#^.,=.|.
-000012d0: bb5d 41f5 4b36 8ff7 23a4 76f0 03d5 b0cc  .]A.K6..#.v.....
-000012e0: 9ff1 578f 2ffa 37f6 b1fa c73e de43 68ff  ..W./.7....>.Ch.
-000012f0: faaa f7ab 74da f833 5f0d efc9 e613 504b  ....t..3_.....PK
-00001300: 0102 1403 1400 0000 0800 d44e 6856 0741  ...........NhV.A
-00001310: 4d62 8100 0000 b100 0000 1000 0000 0000  Mb..............
-00001320: 0000 0000 0000 8001 0000 0000 646f 6350  ............docP
-00001330: 726f 7073 2f61 7070 2e78 6d6c 504b 0102  rops/app.xmlPK..
-00001340: 1403 1400 0000 0800 d44e 6856 25b4 c196  .........NhV%...
-00001350: ef00 0000 2b02 0000 1100 0000 0000 0000  ....+...........
-00001360: 0000 0000 8001 af00 0000 646f 6350 726f  ..........docPro
-00001370: 7073 2f63 6f72 652e 786d 6c50 4b01 0214  ps/core.xmlPK...
-00001380: 0314 0000 0008 00d4 4e68 5699 5c9c 2310  ........NhV.\.#.
-00001390: 0600 009c 2700 0013 0000 0000 0000 0000  ....'...........
-000013a0: 0000 0080 01cd 0100 0078 6c2f 7468 656d  .........xl/them
-000013b0: 652f 7468 656d 6531 2e78 6d6c 504b 0102  e/theme1.xmlPK..
-000013c0: 1403 1400 0000 0800 d44e 6856 fd24 4c60  .........NhV.$L`
-000013d0: 8d01 0000 c603 0000 1800 0000 0000 0000  ................
-000013e0: 0000 0000 8081 0e08 0000 786c 2f77 6f72  ..........xl/wor
-000013f0: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
-00001400: 6d6c 504b 0102 1403 1400 0000 0800 d44e  mlPK...........N
-00001410: 6856 7aef c8e9 e301 0000 3d06 0000 1800  hVz.......=.....
-00001420: 0000 0000 0000 0000 0000 8081 d109 0000  ................
-00001430: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00001440: 6565 7432 2e78 6d6c 504b 0102 1403 1400  eet2.xmlPK......
-00001450: 0000 0800 d44e 6856 7cf3 a3dc 5102 0000  .....NhV|...Q...
-00001460: f609 0000 0d00 0000 0000 0000 0000 0000  ................
-00001470: 8001 ea0b 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
-00001480: 786d 6c50 4b01 0214 0314 0000 0008 00d4  xmlPK...........
-00001490: 4e68 5697 8abb 1cc0 0000 0013 0200 000b  NhV.............
-000014a0: 0000 0000 0000 0000 0000 0080 0166 0e00  .............f..
-000014b0: 005f 7265 6c73 2f2e 7265 6c73 504b 0102  ._rels/.relsPK..
-000014c0: 1403 1400 0000 0800 d44e 6856 b488 015d  .........NhV...]
-000014d0: 4701 0000 af02 0000 0f00 0000 0000 0000  G...............
-000014e0: 0000 0000 8001 4f0f 0000 786c 2f77 6f72  ......O...xl/wor
-000014f0: 6b62 6f6f 6b2e 786d 6c50 4b01 0214 0314  kbook.xmlPK.....
-00001500: 0000 0008 00d4 4e68 568d f72c 5ab4 0000  ......NhV..,Z...
-00001510: 0089 0200 001a 0000 0000 0000 0000 0000  ................
-00001520: 0080 01c3 1000 0078 6c2f 5f72 656c 732f  .......xl/_rels/
-00001530: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
-00001540: 7350 4b01 0214 0314 0000 0008 00d4 4e68  sPK...........Nh
-00001550: 566e a724 bc1e 0100 0057 0400 0013 0000  Vn.$.....W......
-00001560: 0000 0000 0000 0000 0080 01af 1100 005b  ...............[
-00001570: 436f 6e74 656e 745f 5479 7065 735d 2e78  Content_Types].x
-00001580: 6d6c 504b 0506 0000 0000 0a00 0a00 8402  mlPK............
-00001590: 0000 fe12 0000 0000                      ........
+00000840: 2e78 6d6c 8593 db4e c330 0c40 7fa5 ca07  .xml...N.0.@....
+00000850: 9081 c445 a8ad c4c6 653c 2026 10f0 9c35  ...E....e< &...5
+00000860: 6e1b 91c4 c5f1 28fc 3d49 7711 42ad 788a  n.....(.=Iw.B.x.
+00000870: edf8 f812 3b79 8ff4 1e5a 00ce be9c f5a1  ....;y...Z......
+00000880: 102d 7377 2965 a85a 702a 1c61 073e ded4  .-sw)e.Zp*.a.>..
+00000890: 484e 7154 a991 a123 507a 809c 9527 b3d9  HNqT...#Pz...'..
+000008a0: 9974 ca78 51e6 836d 4565 8e1b b6c6 c38a  .t.xQ..mEe......
+000008b0: b2b0 714e d1f7 1c2c f685 3816 7bc3 9369  ..qN...,..8.{..i
+000008c0: 5a4e 0659 e69d 6ae0 19f8 a55b 51d4 e421  ZN.Y..j....[Q..!
+000008d0: 8a36 0e7c 30e8 3382 ba10 57c7 97cb c17f  .6.|0.3...W.....
+000008e0: 7078 35d0 875f 7296 3a59 23be 27e5 5e17  px5.._r.:Y#.'.^.
+000008f0: 6296 0a02 0b15 a708 2a1e 9fb0 006b 53a0  b.......*....kS.
+00000900: 58c6 c72e a638 a44c e06f 791f fd76 e83d  X....8.L.oy..v.=
+00000910: f6b2 5601 1668 df8c e6b6 1017 22d3 50ab  ..V..h......".P.
+00000920: 8de5 27ec 97b0 ebe7 f450 e0b5 6255 e684  ..'......P..bU..
+00000930: 7d46 a9cf 32af 9290 7247 3fe3 d3fb 3c33  }F..2...rG?...<3
+00000940: 45bb 8989 b8f4 ca41 2e39 1690 7459 edfc  E......A.9..tY..
+00000950: e753 fe3d 686d 7c13 b38c 618b 7fb0 9555  .S.=hm|...a....U
+00000960: d518 773d c57d 83a2 0745 6440 8f60 3753  ..w=.}...Ed@.`7S
+00000970: 9843 cfed 3477 3bc5 69f3 8954 8d32 7753  .C..4w;.i..T.2wS
+00000980: 4cbb 096b e5f5 633d 022d 27df c3d4 f097  L..k..c=.-'.....
+00000990: 9071 68fb 45d8 4e31 6d68 eca2 313e 6416  .qh.E.N1mh..1>d.
+000009a0: ea18 6976 747e 2a32 da4e 7dab 3076 c386  ..ivt~*2.N}.0v..
+000009b0: af91 19dd 20b6 f1a3 0025 8778 5f23 f25e  .... ....%.x_#.^
+000009c0: 494b 77f8 7ae5 0f50 4b03 0414 0000 0008  IKw.z..PK.......
+000009d0: 007b 3b77 56c7 95a8 9bdb 0100 00a5 0500  .{;wV...........
+000009e0: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+000009f0: 7473 2f73 6865 6574 322e 786d 6c7d 94db  ts/sheet2.xml}..
+00000a00: 6edb 300c 865f c5f0 03d4 6981 ee50 3806  n.0.._....i..P8.
+00000a10: 9a64 5db3 b5ab 97ac ddb5 62d3 b110 4974  .d].......b...It
+00000a20: 2966 6ede be92 7340 3148 b9b2 48fd 1f0f  )fn...s@1H..H...
+00000a30: b2c4 bc47 dad8 1680 9337 ad8c 1da7 2d73  ...G.....7....-s
+00000a40: 7793 65b6 6a41 0b7b 811d 18b7 d320 69c1  w.e.jA.{..... i.
+00000a50: cea4 7566 3b02 510f 9056 d9d5 68f4 29d3  ..uf;.Q..V..h.).
+00000a60: 429a b4c8 075f 4945 8e5b 56d2 4049 89dd  B...._IE.[V.@I..
+00000a70: 6a2d 6837 0185 fd38 bd4c 8f8e 855c b7ec  j-h7...8.L...\..
+00000a80: 1d59 9177 620d 4be0 e7ae 2467 65a7 28b5  .Y.wb.K...$ge.(.
+00000a90: d460 ac44 9310 34e3 f4f6 f266 39e8 07c1  .`.D..4....f9...
+00000aa0: 8b84 de7e 5827 be93 15e2 c61b f37a 9c8e  ...~X'.......z..
+00000ab0: 7c41 a0a0 621f 41b8 cf3f 9882 523e 902b  |A..b.A..?..R>.+
+00000ac0: e3f5 1033 3da5 f4e0 c7f5 31fa ddd0 bbeb  ...3=.....1.....
+00000ad0: 6525 2c4c 51fd 9535 b7e3 f44b 9ad4 d088  e%,LQ..5...K....
+00000ae0: ade2 05f6 f770 e8e7 fa54 e04c b028 72c2  .....p...T.L.(r.
+00000af0: 3e21 df67 9157 7ee1 733b 9d34 fe7c 964c  >!.g.W~.s;.4.|.L
+00000b00: ce2f 5d22 2e5e 659d 67ec f27b 33ab 0ef2  ./]".^e.g..{3...
+00000b10: 494c 4eb8 13ea eb55 109a c620 2334 04f4  ILN....U... #4..
+00000b20: b3a8 1e57 0afe 4856 21ea 5b8c ea64 c55b  ...W..HV!.[..d.[
+00000b30: 0a21 7731 c4c2 5b40 fe3d 265f 2199 80fe  .!w1..[@.=&_!...
+00000b40: 3ea6 df81 a049 9899 c718 8d86 db08 f423  >....I.........#
+00000b50: 5a98 246e 4b25 aa50 f73f 6354 2d21 f41b  Z.$nK%.P.?cT-!..
+00000b60: 1fce e96f 3940 3c9e 3b80 5938 cbaf b307  ...o9@<.;.Y8....
+00000b70: 1081 9ee2 3766 6e1e 9c2f c094 31a6 971b  ....7fn../..1...
+00000b80: 5942 2d45 00fa 1d83 aa56 aafa a909 208b  YB-E.....V.... .
+00000b90: e8bd 1404 8683 cc32 7a31 3bdc daff bac9  .......2z1;.....
+00000ba0: dc9b 3ece 89fd 23f7 03ec 51d0 5a1a 9b28  ..>...#...Q.Z..(
+00000bb0: 685c a4d1 c5e7 eb34 a1fd 50d8 1b8c dd30  h\.....4..P....0
+00000bc0: 0057 c88c 7a58 b66e 8e02 7981 db6f 10f9  .W..zX.n..y..o..
+00000bd0: 68f8 9974 9acc c53b 504b 0304 1400 0000  h..t...;PK......
+00000be0: 0800 7b3b 7756 7cf3 a3dc 5102 0000 f609  ..{;wV|...Q.....
+00000bf0: 0000 0d00 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
+00000c00: 786d 6cdd 56db 8adb 3010 fd15 e10f a893  xml.V...0.......
+00000c10: 9835 7149 f250 4360 a12d 0bbb 0f7d 5562  .5qI.PC`.-...}Ub
+00000c20: 3911 e8e2 caf2 92f4 eb3b 2339 76b3 ab59  9........;#9v..Y
+00000c30: 287d ab4d f0cc 1c9d b91b 67d3 fbab 12cf  (}.M......g.....
+00000c40: 6721 3cbb 6865 fa6d 76f6 befb 9ce7 fdf1  g!<.he.mv.......
+00000c50: 2c34 ef3f d94e 1840 5aeb 34f7 a0ba 53de  ,4.?.N.@Z.4...S.
+00000c60: 774e f0a6 4792 56f9 6ab1 2873 cda5 c976  wN..G.V.j.(s...v
+00000c70: 1b33 e8bd f63d 3bda c1f8 6db6 c8f2 dda6  .3...=;...m.....
+00000c80: b566 b62c b368 80a3 5c0b f6ca d536 abb9  .f.,.h..\....6..
+00000c90: 9207 27c3 59ae a5ba 46f3 0a0d 47ab ac63  ..'.Y...F...G..c
+00000ca0: 1e52 1148 064b ff2b c2cb a861 96a3 1f2d  .R.H.K.+...a...-
+00000cb0: 8d75 68cc 6384 f0e8 c1a9 546a 4a60 9545  .uh.c.....TjJ`.E
+00000cc0: c36e d371 ef85 337b 5002 2718 df41 6c94  .n.q..3{P.'..Al.
+00000cd0: 5fae 1d64 7072 fcba 5c3d 6433 213c 20c8  _..dpr..\=d3!< .
+00000ce0: c1ba 46b8 bb3a a369 b751 a2f5 4070 f274  ..F..:.i.Q..@p.t
+00000cf0: c6a7 b75d 8ea0 f756 83d0 487e b286 871c  ...]...V..H~....
+00000d00: 6e8c 5100 b747 a1d4 338e e847 7be7 fbd2  n.Q..G..3..G{...
+00000d10: b2d8 ebc7 06db ccb0 d49b 0809 8d62 7413  .............bt.
+00000d20: 15f4 ffa7 b7e8 fb9f ddb2 4ebe 5aff 6580  ..........N.Z.e.
+00000d30: 6a4c d07f 0ed6 8b27 275a 7909 faa5 bd8f  jL.....''Zy.....
+00000d40: 3f85 0e89 dc45 9fac 0c97 639b 7dc7 9d53  ?....E....c.}..S
+00000d50: b30b 7618 a4f2 d28c da59 368d 30ef 6a03  ..v......Y6.0.j.
+00000d60: f79e 1f60 a9ef fcc3 f946 b47c 50fe 6502  ...`.....F.|P.e.
+00000d70: b7d9 2c7f 138d 1c74 359d 7ac2 b2c6 53b3  ..,....t5.z...S.
+00000d80: fc15 67b8 2ca7 cd84 58d2 34e2 229a 7a54  ..g.,...X.4.".zT
+00000d90: dde9 1044 0602 441d 2f24 bc45 f6e1 4a23  ...D..D./$.E..J#
+00000da0: 1427 6269 0431 2a0e 9501 c589 2c2a ceff  .'bi.1*.....,*..
+00000db0: 54cf 9aac 2762 546e eb24 b226 396b 9213  T...'bTn.$.&9k..
+00000dc0: 5929 a40e 3715 27cd a9e0 4a57 5a55 4551  Y)..7.'...JWZUEQ
+00000dd0: 9654 47eb 3a99 414d f5ad 2cf1 97f6 46e5  .TG.:.AM..,...F.
+00000de0: 860c 2a0e 46fa bb5e d3d3 a637 e4e3 3da0  ..*.F..^...7..=.
+00000df0: 66fa d186 5095 d29b 4855 4af7 1a91 74df  f...P...HUJ...t.
+00000e00: 9051 55e9 6953 7190 414d 81da 1d8c 9f8e  .QU.iSq.AM......
+00000e10: 833b 95e6 1405 4e95 ca8d 7a83 69a4 aa28  .;....N...z.i..(
+00000e20: 0477 31bd a365 4974 a7c4 3b3d 1fea 2d29  .w1..eIt..;=..-)
+00000e30: 8aaa 4a23 88a5 3328 0a0a c1b7 9146 a80c  ..J#..3(.....F..
+00000e40: 3007 0a29 8af0 1d7c f33d ca6f dfa9 7cfe  0..)...|.=.o..|.
+00000e50: a7b7 fb0d 504b 0304 1400 0000 0800 7b3b  ....PK........{;
+00000e60: 7756 978a bb1c c000 0000 1302 0000 0b00  wV..............
+00000e70: 0000 5f72 656c 732f 2e72 656c 739d 92b9  .._rels/.rels...
+00000e80: 6ec3 300c 407f c5d0 9e30 07d0 2188 3365  n.0.@....0..!.3e
+00000e90: f116 04f9 0156 a20f d812 058a 459d bfaf  .....V......E...
+00000ea0: daa5 7190 0b19 793d 3c12 dc1e 6940 ed38  ..q...y=<...i@.8
+00000eb0: a4b6 8ba9 18fd 1052 695a d5b8 0148 b625  .......RiZ...H.%
+00000ec0: 8f69 ce91 42ae d42c 1e35 87d2 4044 db63  .i..B..,.5..@D.c
+00000ed0: 43b0 5a2c 3e40 2e19 66b7 bd64 16a7 73a4  C.Z,>@..f..d..s.
+00000ee0: 5788 5cd7 9da5 3ddb 2f4f 416f 80af 3a4c  W.\...=./OAo..:L
+00000ef0: 7142 6948 4b33 0ef0 cdd2 7f32 f7f3 0c35  qBiHK3.....2...5
+00000f00: 45e5 4a23 955b 1a78 d3e5 fe76 e049 d1a1  E.J#.[.x...v.I..
+00000f10: 2258 169a 45c9 d3a2 1da5 7f1d c7f6 90d3  "X..E...........
+00000f20: e9af 6322 b47a 5be8 f971 6854 0a8e dc63  ..c".z[..qhT...c
+00000f30: 258c 7162 b4fe 3582 c90f ec7e 0050 4b03  %.qb..5....~.PK.
+00000f40: 0414 0000 0008 007b 3b77 5696 13f2 7246  .......{;wV...rF
+00000f50: 0100 00af 0200 000f 0000 0078 6c2f 776f  ...........xl/wo
+00000f60: 726b 626f 6f6b 2e78 6d6c b552 d16a c330  rkbook.xml.R.j.0
+00000f70: 0cfc 95e0 0f58 d2b0 1556 9abd ac74 2b8c  .....X...V...t+.
+00000f80: adac a3ef 4ea2 34a2 b615 64a5 5dfb f573  ....N.4...d.]..s
+00000f90: 12c2 0283 b197 3dc9 3a89 f3dd d9cb 33f1  ......=.:.....3.
+00000fa0: 3127 3a46 9fd6 389f a95a a459 c4b1 2f6a  1':F..8..Z.Y../j
+00000fb0: b0da df50 032e 4c2a 62ab 25b4 7c88 7dc3  ...P..L*b.%.|.}.
+00000fc0: a04b 5f03 8835 719a 24f3 d86a 74ea 6139  .K_..5q.$..jt.a9
+00000fd0: 726d 399e 3624 5008 920b 6007 ec11 cefe  rm9.6$P...`.....
+00000fe0: 7bde b5d1 093d e668 502e 99ea cf06 5464  {....=.hP.....Td
+00000ff0: d1a1 c52b 9499 4a54 e46b 3a3f 13e3 959c  ...+..JT.k:?....
+00001000: 68b3 2b98 8cc9 d46c 18ec 8105 8b1f f0ae  h.+....l........
+00001010: 13f9 a173 df23 a2f3 771d 8464 6a9e 04c2  ...s.#..w..dj...
+00001020: 0ad9 4bbf d1f3 eba0 f104 6179 e85a a135  ..K.......ay.Z.5
+00001030: 1a01 5e69 8127 a6b6 4177 e868 828b 7862  ..^i.'..Aw.h..xb
+00001040: a3cf 61ac 4388 0bfe 4b8c 5455 58c0 8a8a  ..a.C...K.TUX...
+00001050: d682 9321 4706 d309 74be c6c6 abc8 690b  ...!G...t.....i.
+00001060: 995a 6b8b e6d2 190a 376c cac1 9c04 5593  .Zk.....7l....U.
+00001070: a878 8161 c09b b2d7 f77f 5ab6 c09e dc44  .x.a......Z....D
+00001080: 4bfa 8b96 b4cf 6a0c a884 0a1d 94af 81c7  K.....j.........
+00001090: 073c 3c56 b1e5 a82b bda7 f4f6 6e76 1f1e  .<<V...+....nv..
+000010a0: a535 e631 606f ee85 7439 e63d fe95 872f  .5.1`o..t9.=.../
+000010b0: 504b 0304 1400 0000 0800 7b3b 7756 8df7  PK........{;wV..
+000010c0: 2c5a b400 0000 8902 0000 1a00 0000 786c  ,Z............xl
+000010d0: 2f5f 7265 6c73 2f77 6f72 6b62 6f6f 6b2e  /_rels/workbook.
+000010e0: 786d 6c2e 7265 6c73 c592 4d0a 8330 1046  xml.rels..M..0.F
+000010f0: af12 7280 8eda d245 5157 ddb8 2d5e 20e8  ..r....EQW..-^ .
+00001100: f883 d184 cc94 eaed 6b75 a181 2eba 91ae  ........ku......
+00001110: c237 21ef 7b30 891f a815 b766 a0a6 b524  .7!.{0.....f...$
+00001120: c65e 0f94 c886 d9de 00a8 68b0 5774 3216  .^........h.Wt2.
+00001130: 87f9 a632 ae57 3c47 5783 5545 a76a 8428  ...2.W<GW.UE.j.(
+00001140: 08ae e0f6 0c99 c67b a6c8 278b bf10 4d55  .......{..'...MU
+00001150: b505 de4d f1ec 71e0 2f60 7819 d751 83c8  ...M..q./`x..Q..
+00001160: 52e4 cad5 c889 8451 6f63 82e5 084f 3359  R......Qoc...O3Y
+00001170: 8aac 4ca4 cbca 50c2 bf85 224f 283a 5088  ..L...P..."O(:P.
+00001180: 78d2 489b cd9a bdfa f381 f53c bfc5 ad7d  x.H........<...}
+00001190: 89eb d0df c9e5 e300 decf 4bdf 504b 0304  ..........K.PK..
+000011a0: 1400 0000 0800 7b3b 7756 6ea7 24bc 1e01  ......{;wVn.$...
+000011b0: 0000 5704 0000 1300 0000 5b43 6f6e 7465  ..W.......[Conte
+000011c0: 6e74 5f54 7970 6573 5d2e 786d 6cc5 94cf  nt_Types].xml...
+000011d0: 4ec3 300c c65f a5ca 756a 3276 e080 d65d  N.0.._..uj2v...]
+000011e0: 802b ecc0 0b84 d65d a3e6 9f62 6f74 6f8f  .+.....]...boto.
+000011f0: db6e 9340 a362 2a12 9746 8ded efe7 f88b  .n.@.b*..F......
+00001200: b27e 3b46 c0ac 73d6 6321 1aa2 f8a0 1496  .~;F..s.c!......
+00001210: 0d38 8d32 44f0 1ca9 4372 9af8 37ed 54d4  .8.2D...Cr..7.T.
+00001220: 65ab 77a0 56cb e5bd 2a83 27f0 9453 af21  e.w.V...*.'..S.!
+00001230: 36eb 27a8 f5de 52f6 dcf1 369a e00b 91c0  6.'...R...6.....
+00001240: a2c8 1ec7 c49e 5508 1da3 35a5 268e ab83  ......U...5.&...
+00001250: afbe 51f2 1341 72e5 9083 8d89 b8e0 04a1  ..Q..Ar.........
+00001260: ae12 fac8 cf80 53dd eb01 5232 1564 5b9d  ......S...R2.d[.
+00001270: e845 3bce 529d 5548 470b 28a7 25ae f418  .E;.R.UHG.(.%...
+00001280: eada 9450 8572 efb8 4462 4ca0 2b6c 00c8  ...P.r..DbL.+l..
+00001290: 5939 8a2e a6c9 c413 86f1 7b37 9b3f c84c  Y9........{7.?.L
+000012a0: 0139 739b 4244 762c c1ed b8b3 257d 751e  .9s.BDv,....%}u.
+000012b0: 5908 1299 e923 5e88 2c3d fb7c d0bb 5d41  Y....#^.,=.|..]A
+000012c0: f54b 368f f723 a476 f003 d5b0 cc9f f157  .K6..#.v.......W
+000012d0: 8f2f fa37 f6b1 fac7 3ede 4368 fffa aaf7  ./.7....>.Ch....
+000012e0: ab74 daf8 335f 0def c9e6 1350 4b01 0214  .t..3_.....PK...
+000012f0: 0314 0000 0008 007b 3b77 5607 414d 6281  .......{;wV.AMb.
+00001300: 0000 00b1 0000 0010 0000 0000 0000 0000  ................
+00001310: 0000 0080 0100 0000 0064 6f63 5072 6f70  .........docProp
+00001320: 732f 6170 702e 786d 6c50 4b01 0214 0314  s/app.xmlPK.....
+00001330: 0000 0008 007b 3b77 5680 76fe 74ef 0000  .....{;wV.v.t...
+00001340: 002b 0200 0011 0000 0000 0000 0000 0000  .+..............
+00001350: 0080 01af 0000 0064 6f63 5072 6f70 732f  .......docProps/
+00001360: 636f 7265 2e78 6d6c 504b 0102 1403 1400  core.xmlPK......
+00001370: 0000 0800 7b3b 7756 995c 9c23 1006 0000  ....{;wV.\.#....
+00001380: 9c27 0000 1300 0000 0000 0000 0000 0000  .'..............
+00001390: 8001 cd01 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
+000013a0: 6865 6d65 312e 786d 6c50 4b01 0214 0314  heme1.xmlPK.....
+000013b0: 0000 0008 007b 3b77 5634 f82c 6d83 0100  .....{;wV4.,m...
+000013c0: 0086 0300 0018 0000 0000 0000 0000 0000  ................
+000013d0: 0080 810e 0800 0078 6c2f 776f 726b 7368  .......xl/worksh
+000013e0: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
+000013f0: 4b01 0214 0314 0000 0008 007b 3b77 56c7  K..........{;wV.
+00001400: 95a8 9bdb 0100 00a5 0500 0018 0000 0000  ................
+00001410: 0000 0000 0000 0080 81c7 0900 0078 6c2f  .............xl/
+00001420: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00001430: 322e 786d 6c50 4b01 0214 0314 0000 0008  2.xmlPK.........
+00001440: 007b 3b77 567c f3a3 dc51 0200 00f6 0900  .{;wV|...Q......
+00001450: 000d 0000 0000 0000 0000 0000 0080 01d8  ................
+00001460: 0b00 0078 6c2f 7374 796c 6573 2e78 6d6c  ...xl/styles.xml
+00001470: 504b 0102 1403 1400 0000 0800 7b3b 7756  PK..........{;wV
+00001480: 978a bb1c c000 0000 1302 0000 0b00 0000  ................
+00001490: 0000 0000 0000 0000 8001 540e 0000 5f72  ..........T..._r
+000014a0: 656c 732f 2e72 656c 7350 4b01 0214 0314  els/.relsPK.....
+000014b0: 0000 0008 007b 3b77 5696 13f2 7246 0100  .....{;wV...rF..
+000014c0: 00af 0200 000f 0000 0000 0000 0000 0000  ................
+000014d0: 0080 013d 0f00 0078 6c2f 776f 726b 626f  ...=...xl/workbo
+000014e0: 6f6b 2e78 6d6c 504b 0102 1403 1400 0000  ok.xmlPK........
+000014f0: 0800 7b3b 7756 8df7 2c5a b400 0000 8902  ..{;wV..,Z......
+00001500: 0000 1a00 0000 0000 0000 0000 0000 8001  ................
+00001510: b010 0000 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
+00001520: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 504b  kbook.xml.relsPK
+00001530: 0102 1403 1400 0000 0800 7b3b 7756 6ea7  ..........{;wVn.
+00001540: 24bc 1e01 0000 5704 0000 1300 0000 0000  $.....W.........
+00001550: 0000 0000 0000 8001 9c11 0000 5b43 6f6e  ............[Con
+00001560: 7465 6e74 5f54 7970 6573 5d2e 786d 6c50  tent_Types].xmlP
+00001570: 4b05 0600 0000 000a 000a 0084 0200 00eb  K...............
+00001580: 1200 0000 00                             .....
```

### Comparing `pymetamodel-0.2.7/examples/family/FamilyContext.yaml` & `pymetamodel-0.3.0/examples/family/FamilyContext.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -9,99 +9,78 @@
     prefix_reference: FamilyContext/
   xsd:
     prefix_prefix: xsd
     prefix_reference: http://www.w3.org/2001/XMLSchema#
   shex:
     prefix_prefix: shex
     prefix_reference: http://www.w3.org/ns/shex#
-  schema:
-    prefix_prefix: schema
-    prefix_reference: http://schema.org/
 default_prefix: FamilyContext
 default_range: string
 types:
   string:
     name: string
     description: A character string
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Text
     base: str
     uri: xsd:string
   integer:
     name: integer
     description: An integer
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Integer
     base: int
     uri: xsd:integer
   boolean:
     name: boolean
     description: A binary (true or false) value
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Boolean
     base: Bool
     uri: xsd:boolean
     repr: bool
   float:
     name: float
     description: A real number that conforms to the xsd:float specification
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Float
     base: float
     uri: xsd:float
   double:
     name: double
     description: A real number that conforms to the xsd:double specification
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:Float
     base: float
     uri: xsd:double
   decimal:
     name: decimal
     description: A real number with arbitrary precision that conforms to the xsd:decimal
       specification
     from_schema: https://w3id.org/linkml/types
-    broad_mappings:
-    - schema:Number
     base: Decimal
     uri: xsd:decimal
   time:
     name: time
     description: A time object represents a (local) time of day, independent of any
       particular day
     notes:
-    - URI is dateTime because OWL reasoners do not work with straight date or time
+    - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Time
     base: XSDTime
     uri: xsd:dateTime
     repr: str
   date:
     name: date
     description: a date (year, month and day) in an idealized calendar
     notes:
     - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Date
     base: XSDDate
     uri: xsd:date
     repr: str
   datetime:
     name: datetime
     description: The combination of a date and time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:DateTime
     base: XSDDateTime
     uri: xsd:dateTime
     repr: str
   date_or_datetime:
     name: date_or_datetime
     description: Either a date or a datetime
     from_schema: https://w3id.org/linkml/types
@@ -111,36 +90,18 @@
   uriorcurie:
     name: uriorcurie
     description: a URI or a CURIE
     from_schema: https://w3id.org/linkml/types
     base: URIorCURIE
     uri: xsd:anyURI
     repr: str
-  curie:
-    name: curie
-    conforms_to: https://www.w3.org/TR/curie/
-    description: a compact URI
-    comments:
-    - in RDF serializations this MUST be expanded to a URI
-    - in non-RDF serializations MAY be serialized as the compact representation
-    from_schema: https://w3id.org/linkml/types
-    base: Curie
-    uri: xsd:string
-    repr: str
   uri:
     name: uri
-    conforms_to: https://www.ietf.org/rfc/rfc3987.txt
     description: a complete URI
-    comments:
-    - in RDF serializations a slot with range of uri is treated as a literal or type
-      xsd:anyURI unless it is an identifier or a reference to an identifier, in which
-      case it is translated directly to a node
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:URL
     base: URI
     uri: xsd:anyURI
     repr: str
   ncname:
     name: ncname
     description: Prefix part of CURIE
     from_schema: https://w3id.org/linkml/types
```

### Comparing `pymetamodel-0.2.7/examples/family/FamilyContext_puml.txt` & `pymetamodel-0.3.0/examples/family/FamilyContext_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/metamodel/metamodel.mermaid` & `pymetamodel-0.3.0/examples/metamodel/metamodel.mermaid`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/metamodel/metamodel.puml` & `pymetamodel-0.3.0/examples/metamodel/metamodel.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/metamodel/metamodel.py` & `pymetamodel-0.3.0/examples/metamodel/metamodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from metamodel.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-08T09:55:01
+# Generation date: 2023-03-23T07:28:05
 # Schema: MetaModel
 #
 # id: MetaModel
 # description:
 # license:
 
 import dataclasses
@@ -18,26 +18,25 @@
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
 from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
 from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.metamodelcore import Bool, Curie, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
+from linkml_runtime.utils.metamodelcore import Bool, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
 METAMODEL = CurieNamespace('MetaModel', 'MetaModel/')
 LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
-SCHEMA = CurieNamespace('schema', 'http://schema.org/')
 SHEX = CurieNamespace('shex', 'http://www.w3.org/ns/shex#')
 XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = METAMODEL
 
 
 # Types
 class String(str):
@@ -124,22 +123,14 @@
     """ a URI or a CURIE """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uriorcurie"
     type_model_uri = METAMODEL.Uriorcurie
 
 
-class Curie(Curie):
-    """ a compact URI """
-    type_class_uri = XSD.string
-    type_class_curie = "xsd:string"
-    type_name = "curie"
-    type_model_uri = METAMODEL.Curie
-
-
 class Uri(URI):
     """ a complete URI """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uri"
     type_model_uri = METAMODEL.Uri
```

### Comparing `pymetamodel-0.2.7/examples/metamodel/metamodel.sidif` & `pymetamodel-0.3.0/examples/metamodel/metamodel.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/metamodel/metamodel.yaml` & `pymetamodel-0.3.0/examples/metamodel/metamodel.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,99 +9,78 @@
     prefix_reference: MetaModel/
   xsd:
     prefix_prefix: xsd
     prefix_reference: http://www.w3.org/2001/XMLSchema#
   shex:
     prefix_prefix: shex
     prefix_reference: http://www.w3.org/ns/shex#
-  schema:
-    prefix_prefix: schema
-    prefix_reference: http://schema.org/
 default_prefix: MetaModel
 default_range: string
 types:
   string:
     name: string
     description: A character string
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Text
     base: str
     uri: xsd:string
   integer:
     name: integer
     description: An integer
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Integer
     base: int
     uri: xsd:integer
   boolean:
     name: boolean
     description: A binary (true or false) value
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Boolean
     base: Bool
     uri: xsd:boolean
     repr: bool
   float:
     name: float
     description: A real number that conforms to the xsd:float specification
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Float
     base: float
     uri: xsd:float
   double:
     name: double
     description: A real number that conforms to the xsd:double specification
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:Float
     base: float
     uri: xsd:double
   decimal:
     name: decimal
     description: A real number with arbitrary precision that conforms to the xsd:decimal
       specification
     from_schema: https://w3id.org/linkml/types
-    broad_mappings:
-    - schema:Number
     base: Decimal
     uri: xsd:decimal
   time:
     name: time
     description: A time object represents a (local) time of day, independent of any
       particular day
     notes:
-    - URI is dateTime because OWL reasoners do not work with straight date or time
+    - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Time
     base: XSDTime
     uri: xsd:dateTime
     repr: str
   date:
     name: date
     description: a date (year, month and day) in an idealized calendar
     notes:
     - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Date
     base: XSDDate
     uri: xsd:date
     repr: str
   datetime:
     name: datetime
     description: The combination of a date and time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:DateTime
     base: XSDDateTime
     uri: xsd:dateTime
     repr: str
   date_or_datetime:
     name: date_or_datetime
     description: Either a date or a datetime
     from_schema: https://w3id.org/linkml/types
@@ -111,36 +90,18 @@
   uriorcurie:
     name: uriorcurie
     description: a URI or a CURIE
     from_schema: https://w3id.org/linkml/types
     base: URIorCURIE
     uri: xsd:anyURI
     repr: str
-  curie:
-    name: curie
-    conforms_to: https://www.w3.org/TR/curie/
-    description: a compact URI
-    comments:
-    - in RDF serializations this MUST be expanded to a URI
-    - in non-RDF serializations MAY be serialized as the compact representation
-    from_schema: https://w3id.org/linkml/types
-    base: Curie
-    uri: xsd:string
-    repr: str
   uri:
     name: uri
-    conforms_to: https://www.ietf.org/rfc/rfc3987.txt
     description: a complete URI
-    comments:
-    - in RDF serializations a slot with range of uri is treated as a literal or type
-      xsd:anyURI unless it is an identifier or a reference to an identifier, in which
-      case it is translated directly to a node
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:URL
     base: URI
     uri: xsd:anyURI
     repr: str
   ncname:
     name: ncname
     description: Prefix part of CURIE
     from_schema: https://w3id.org/linkml/types
```

### Comparing `pymetamodel-0.2.7/examples/metamodel/metamodel_puml.txt` & `pymetamodel-0.3.0/examples/metamodel/metamodel_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/scientific-events/scientific-events.mermaid` & `pymetamodel-0.3.0/examples/scientific-events/scientific-events.mermaid`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/scientific-events/scientific-events.puml` & `pymetamodel-0.3.0/examples/scientific-events/scientific-events.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/scientific-events/scientific-events.py` & `pymetamodel-0.3.0/examples/scientific-events/scientific-events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from scientific-events.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-08T09:54:23
+# Generation date: 2023-03-23T07:27:44
 # Schema: CrSchema
 #
 # id: CrSchema
 # description:
 # license:
 
 import dataclasses
@@ -18,26 +18,25 @@
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
 from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
 from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.metamodelcore import Bool, Curie, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
+from linkml_runtime.utils.metamodelcore import Bool, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
 CRSCHEMA = CurieNamespace('CrSchema', 'CrSchema/')
 LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
-SCHEMA = CurieNamespace('schema', 'http://schema.org/')
 SHEX = CurieNamespace('shex', 'http://www.w3.org/ns/shex#')
 XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = CRSCHEMA
 
 
 # Types
 class String(str):
@@ -124,22 +123,14 @@
     """ a URI or a CURIE """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uriorcurie"
     type_model_uri = CRSCHEMA.Uriorcurie
 
 
-class Curie(Curie):
-    """ a compact URI """
-    type_class_uri = XSD.string
-    type_class_curie = "xsd:string"
-    type_name = "curie"
-    type_model_uri = CRSCHEMA.Curie
-
-
 class Uri(URI):
     """ a complete URI """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uri"
     type_model_uri = CRSCHEMA.Uri
```

### Comparing `pymetamodel-0.2.7/examples/scientific-events/scientific-events.sidif` & `pymetamodel-0.3.0/examples/scientific-events/scientific-events.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/scientific-events/scientific-events.xlsx` & `pymetamodel-0.3.0/examples/teaching/TeachingSchema.xlsx`

 * *Files 27% similar despite different names*

```diff
@@ -1,562 +1,596 @@
-00000000: 504b 0304 1400 0000 0800 cc4e 6856 0741  PK.........NhV.A
+00000000: 504b 0304 1400 0000 0800 803b 7756 0741  PK.........;wV.A
 00000010: 4d62 8100 0000 b100 0000 1000 0000 646f  Mb............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 3d0b 0231 1044 ffca 71bd b741 c142 6240  =..1.D..q..A.Bb@
 00000040: d052 b0b2 0f7b 1b2f 9064 43b2 427e be39  .R...{./.dC.B~.9
 00000050: c18f 6e1e 6f18 46df 0a67 2ae2 a90e 2d86  ..n.o.F..g*...-.
 00000060: 548f e322 920f 0015 178a b64e 5da7 6e1c  T..".......N].n.
 00000070: 9768 a563 7900 3be7 91ce 8ccf 4849 60ab  .h.cy.;.....HI`.
 00000080: d41e a809 a599 e64d fe0e 8e46 9f72 0e1e  .......M...F.r..
 00000090: ad78 4ee6 eab1 7065 27c3 a521 050d ff72  .xN...pe'..!...r
 000000a0: 6dde a9d4 35ef 26f5 961f d6f0 3b69 5e50  m...5.&.....;i^P
-000000b0: 4b03 0414 0000 0008 00cc 4e68 56d1 f9d1  K.........NhV...
-000000c0: 68ef 0000 002b 0200 0011 0000 0064 6f63  h....+.......doc
+000000b0: 4b03 0414 0000 0008 0080 3b77 565d 9571  K.........;wV].q
+000000c0: 93ee 0000 002b 0200 0011 0000 0064 6f63  .....+.......doc
 000000d0: 5072 6f70 732f 636f 7265 2e78 6d6c cd92  Props/core.xml..
-000000e0: 514b c330 10c7 bf8a e4bd bdb4 9d32 4297  QK.0.........2B.
-000000f0: 17c5 2705 c181 e25b 486e 5b58 d386 e4a4  ..'....[Hn[X....
-00000100: ddb7 378d 5b87 e807 10f2 92bb 7f7e f73b  ..7.[........~.;
-00000110: 48ab bdd0 43c0 9730 780c 6431 de4c aeeb  H...C..0x.d1.L..
-00000120: a3d0 7ec3 0e44 5e00 447d 40a7 6299 127d  ..~..D^.D}@.b..}
-00000130: 6aee 86e0 14a5 6bd8 8357 faa8 f608 35e7  j.....k..W....5.
-00000140: 77e0 9094 51a4 6006 167e 2132 d91a 2d74  w...Q.`..~!2..-t
-00000150: 4045 4338 e38d 5ef0 fe33 7419 6634 6087  @EC8..^..3t.f4`.
-00000160: 0e7b 8a50 9515 3039 4ff4 a7a9 6be1 0a98  .{.P..09O...k...
-00000170: 6184 c1c5 ef02 9a85 98ab 7f62 7307 d839  a..........bs..9
-00000180: 3945 bba4 c671 2cc7 26e7 d20e 15bc 3f3f  9E...q,.&.....??
-00000190: bde6 750b db47 52bd c6f4 2a5a 4127 8f1b  ..u..GR...*ZA'..
-000001a0: 7699 fcd6 dc3f 6c1f 99ac 79dd 143c 9df5  v....?l...y..<..
-000001b0: 96af c5ed 4ad4 ab8f d9f5 87df 55d8 0dc6  ....J.......U...
-000001c0: eeec 3f36 be08 ca16 7efd 0bf9 0550 4b03  ..?6....~....PK.
-000001d0: 0414 0000 0008 00cc 4e68 5699 5c9c 2310  ........NhV.\.#.
-000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
-000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
-00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
-00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
-00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
-00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
-00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
-00000250: b72f dee0 5732 2411 4130 19a7 aff0 c00a  ./..W2$.A0......
-00000260: a54c 5eb5 5a69 00c3 387d c913 12c3 dc82  .L^.Zi..8}......
-00000270: 8b08 4b78 14cb d65c e05b 1a2f 23d6 eab4  ..Kx...\.[./#...
-00000280: dbdd 5684 696c a118 4764 607d 5e2c 6840  ..V.il..Gd`}^,h@
-00000290: d054 515a 6f5f 20b4 e51f 33f8 15cb 548d  .TQZo_ ...3...T.
-000002a0: 65a3 0113 5741 26b9 88b4 f2f9 6cc5 fcda  e...WA&.....l...
-000002b0: de3e 65cf e93a 1d32 816e 301b 5820 7fce  .>e..:.2.n0.X ..
-000002c0: 6fa7 e44e 5a88 e154 c2c4 c06a 673f 566b  o..NZ..T...jg?Vk
-000002d0: c7d1 d248 8082 c97d 9405 ba49 f6a3 d315  ...H...}...I....
-000002e0: 0832 0d3b 3a9d 58ce 767c f6c4 ed9f 8cca  .2.;:.X.v|......
-000002f0: da74 346d 1ae0 e3f1 7838 b6cb d28b 701c  .t4m....x8....p.
-00000300: 04e0 51bb 9ec2 9df4 6cbf a441 09b4 a369  ..Q.....l..A...i
-00000310: d064 d8f6 daae 91a6 aa8d 534f d3f7 7ddf  .d........SO..}.
-00000320: eb9b 689c 0a8d 5b4f d36b 77dd d38e 89c6  ..h...[O.kw.....
-00000330: add0 780d bef1 4f87 c3ae 89c6 abd0 74eb  ..x...O.......t.
-00000340: 6926 27fd ae6b a4e9 1668 4246 e3eb 7a12  i&'..k...hBF..z.
-00000350: 15b5 e540 d320 0058 7076 d6cc d203 965e  ...@. .Xpv.....^
-00000360: 29fa 7594 1ad9 1dbb dd41 5cf0 58ee 3989  ).u......A\.X.9.
-00000370: 11fe c6c5 04d6 69d2 1996 3446 729d 9005  ......i...4Fr...
-00000380: 0e00 37c4 d14c 507c af41 b68a e0c2 92d2  ..7..LP|.A......
-00000390: 5c90 d6cf 29b5 501a 089a c881 f547 8221  \...).P......G.!
-000003a0: c5dc affd f597 bbc9 a433 7a9d 7d3a ce6b  .........3z.}:.k
-000003b0: 947f 69ab 01a7 edbb 9bcf 93fc 73e8 e49f  ..i.........s...
-000003c0: a793 d74d 42ce 70bc 2c09 f1fb 235b 6187  ...MB.p.,...#[a.
-000003d0: 276e 3b13 723a 1c67 427c cff6 f691 a525  'n;.r:.gB|.....%
-000003e0: 32cf eff9 0aeb 4e3c 671f 5696 b05d cfcf  2.....N<g.V..]..
-000003f0: e49e 8c72 23bb ddf6 587d f64f 476e 23d7  ...r#...X}.OGn#.
-00000400: a9c0 b322 d794 4624 459f c82d bae4 1138  ..."..F$E..-...8
-00000410: b549 0d32 133f 089d 8698 6a50 1c02 a409  .I.2.?....jP....
-00000420: 3196 a186 f8b4 c6ac 11e0 137d b7be 08c8  1..........}....
-00000430: df8d 88f7 ab6f 9a3d 57a1 5849 da84 f810  .....o.=W.XI....
-00000440: 461a e29c 73e6 73d1 6cfb 07a5 46d1 f655  F...s.s.l...F..U
-00000450: bcdc a397 5815 0197 18df 34aa 352c c5d6  ....X.....4.5,..
-00000460: 7895 c0f1 ad9c 3c1d 1312 cd94 0b06 4186  x.....<.......A.
-00000470: 9724 2612 a939 7e4d 4813 fe2b a5da fe9c  .$&..9~MH..+....
-00000480: d340 f094 2f24 fa4a 918f 69b3 23a7 7426  .@../$.J..i.#.t&
-00000490: cde8 331a c146 af1b 7587 68d2 3c7a fe05  ..3..F..u.h.<z..
-000004a0: f99c 350a 1c91 1b1d 0267 1bb3 4621 8469  ..5......g..F!.i
-000004b0: bbf0 1eaf 248e 9aad c211 2b42 3e62 1936  ....$.....+B>b.6
-000004c0: 1a72 b516 81b6 71a9 8460 5a12 c6d1 784e  .r....q..`Z...xN
-000004d0: d2b4 11fc 59ac 3593 3e60 c8ec cd91 75ce  ....Y.5.>`....u.
-000004e0: d691 0e11 925e 3742 3e62 ce8b 9011 bf1e  .....^7B>b......
-000004f0: 8638 4a9a eda2 7158 04fd 9e5e c349 c1e8  .8J...qX...^.I..
-00000500: 82cb 66fd b87e 86d5 336c 2c8e f747 d417  ..f..~..3l,..G..
-00000510: 4ae4 0f26 a73f e932 3407 a39a 5909 bd84  J..&.?.24...Y...
-00000520: 566a 9faa 8734 3ea8 1e32 0a05 f1b9 1e3e  Vj...4>..2.....>
-00000530: e57a 780a 3796 c6bc 50ae 827b 01ff d1da  .zx.7...P..{....
-00000540: 37c2 abf8 82c0 397f 2e7d cfa5 efb9 f43d  7.....9..}.....=
-00000550: a1d2 b737 237d 67c1 d38b 5bde 466e 5bc4  ...7#}g...[.Fn[.
-00000560: fbae 31da d734 2e28 6357 72cd c8c7 54af  ..1..4.(cWr...T.
-00000570: 9329 d839 9fc0 ecfd 683e 9ef1 edfa d924  .).9....h>.....$
-00000580: 84af 9a59 2d23 1690 4b81 b341 24b8 fc8b  ...Y-#..K..A$...
-00000590: caf0 2ac4 09e8 645b 2509 cb54 d365 378a  ..*...d[%..T.e7.
-000005a0: 129e 421b 6ee9 53f5 4a95 d7e5 afb9 28b8  ..B.n.S.J.....(.
-000005b0: 3c5b e4e9 afa1 743e 2ccf f93c 5fe7 b4cd  <[....t>,..<_...
-000005c0: 0b33 43b7 724b eab6 94be b526 384a f4b1  .3C.rK.....&8J..
-000005d0: cc70 4e1e cb0c 3b67 3c92 1db6 77a0 1d35  .pN...;g<...w..5
-000005e0: fbf6 5d76 e423 a530 5397 43b8 1a42 be03  ..]v.#.0S.C..B..
-000005f0: 6dba 9ddc 3a38 9e98 91b9 0ad3 5290 6fc3  m...:8......R.o.
-00000600: f9e9 c578 1ae2 39d9 04b9 7d98 576d e7d8  ...x..9...}.Wm..
-00000610: d1d1 fbe7 c151 b0a3 ef3c 961d c788 f2a2  .....Q...<......
-00000620: 21ee a186 98cf c343 8779 7b5f 9867 95c6  !......C.y{_.g..
-00000630: 5034 146d 6cac 242c 46b7 60b8 d7f1 2c14  P4.ml.$,F.`...,.
-00000640: e064 602d a007 83af 5102 f252 5560 315b  .d`-....Q..RU`1[
-00000650: c603 2b90 a27c 4c8c 45e8 70e7 975c 5fe3  ..+..|L.E.p..\_.
-00000660: d192 e3db a665 b56e af29 7719 6d22 5239  .....e.n.)w.m"R9
-00000670: c269 9813 67ab cade 65b1 c155 1dcf 555b  .i..g...e..U..U[
-00000680: f2b0 be6a 3db4 154e cffe 59ad c89f 0c11  ...j=..N..Y.....
-00000690: 4e16 0b12 4863 9417 a64a a2f3 1953 bee7  N...Hc...J...S..
-000006a0: 2b49 c455 38bf 4533 b612 9718 bce3 e6c7  +I.U8.E3........
-000006b0: 714e 53b8 1276 b60f 0232 b9bb 39a9 7a65  qNS..v...2..9.ze
-000006c0: 3167 a6f2 df2d 0c09 2c5b 8859 12e2 4d5d  1g...-..,[.Y..M]
-000006d0: edd5 e79b 9cae 7a22 76fa 9777 c160 f2fd  ......z"v..w.`..
-000006e0: 70c9 470f e53b e75f f45d 43ae 7ef6 dde3  p.G..;._.]C.~...
-000006f0: fa6e 933b 484c 9c79 c511 0174 4502 2395  .n.;HL.y...tE.#.
-00000700: 1c06 1617 32e4 50ee 9290 0613 01cd 94c9  ....2.P.........
-00000710: 44f0 0282 64a6 1c80 98fa 0bbd f20c b929  D...d..........)
-00000720: 15ce ad3e 397f 452c 8386 4e5e d225 1214  ...>9.E,..N^.%..
-00000730: 8ab0 0c05 2117 72e3 efef 936a 778c d7fa  ....!.r....jw...
-00000740: 2c81 6d84 5432 64d5 17ca 4389 c13d 3372  ,.m.T2d...C..=3r
-00000750: 43d8 5425 f3ae da26 0b85 dbe2 54cd bb1a  C.T%...&....T...
-00000760: be26 604b c37a 6e9d 2d27 ffdb 5ed4 3db4  .&`K.zn.-'..^.=.
-00000770: 173d 46f3 a399 e01e b387 739b 7ab8 c245  .=F.......s.z..E
-00000780: acff 58d6 1ef9 32df 3970 db3a de03 5ee6  ..X...2.9p.:..^.
-00000790: 132c 43a4 7ec1 7d8a 8a80 11ab 62be baaf  .,C.~.}.....b...
-000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
-000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
-000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
-000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
-000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
-000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
-00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
-00000810: 0304 1400 0000 0800 cc4e 6856 e6d2 6d07  .........NhV..m.
-00000820: 4d01 0000 4f02 0000 1800 0000 786c 2f77  M...O.......xl/w
-00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00000840: 2e78 6d6c 7d52 cd4e c330 0c7e 9528 0fb0  .xml}R.N.0.~.(..
-00000850: 7448 0334 b595 d810 8203 d2b4 0938 4e59  tH.4.........8NY
-00000860: ebb6 d192 b824 1e65 6f4f 92ad 155c 38c5  .....$.eoO...\8.
-00000870: 76ec efc7 493e a03b fa0e 80d8 b7d1 d617  v...I>.;........
-00000880: bc23 ea97 42f8 aa03 23fd 0c7b b0e1 a641  .#..B...#..{...A
-00000890: 6724 85d4 b5c2 f70e 649d 868c 1637 5976  g$......d....7Yv
-000008a0: 2b8c 5496 9779 aa6d 5c99 e389 b4b2 b071  +.T..y.m\......q
-000008b0: cc9f 8c91 eebc 028d 43c1 e77c 2c6c 55db  ........C..|,lU.
-000008c0: 512c 8832 ef65 0b3b a0b7 7ee3 4226 2694  Q,.2.e.;..~.B&&.
-000008d0: 5a19 b05e a165 0e9a 823f cc97 abd4 9f1a  Z..^.e...?......
-000008e0: de15 0cfe 57cc a293 03e2 3126 2f75 c1b3  ....W.....1&/u..
-000008f0: 2808 3454 1411 6438 be60 0d5a 47a0 20e3  (.4T..d8.`.ZG. .
-00000900: f38a c927 ca38 f83b 1ed1 9f92 f7e0 e520  ...'.8.;....... 
-00000910: 3dac 517f a89a ba82 df73 5643 234f 9ab6  =.Q......sVC#O..
-00000920: 383c c3d5 cf62 12f8 2849 96b9 c381 b9e8  8<...b..(I......
-00000930: b3cc ab18 44ee d0a7 6cdc cf8e 5ca8 ab40  ....D...l...\..@
-00000940: 4465 a5e8 bcdf 5b69 2017 1464 c4aa a8ae  De....[i ..d....
-00000950: 53ab ffa7 0675 5475 a053 f5df 5911 d847  S....uTu.S..Y..G
-00000960: 4717 3971 d5af d2b5 ca7a a6a1 0998 d9ec  G.9q.....z......
-00000970: 6ec1 99bb c8bf 2484 7d7a aa03 12a1 4961  n.....$.}z....Ia
-00000980: 175e 1c5c 6c08 f70d 228d 49dc def4 87ca  .^.\l...".I.....
-00000990: 1f50 4b03 0414 0000 0008 00cc 4e68 5624  .PK.........NhV$
-000009a0: 3fa2 5d50 0100 0055 0200 0018 0000 0078  ?.]P...U.......x
-000009b0: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-000009c0: 6574 322e 786d 6c85 52cb 4ec3 3010 fc95  et2.xml.R.N.0...
-000009d0: c81f 50a7 4805 5425 9168 1182 0352 d50a  ..P.H.T%.h...R..
-000009e0: 3856 6eb2 49ac dade b0de 10fa f7d8 6953  8Vn.I.........iS
-000009f0: c189 53f6 35b3 33eb 6403 d2d1 b700 9c7c  ..S.5.3.d......|
-00000a00: 5be3 7c2e 5ae6 6e29 a52f 5bb0 cacf b003  [.|.Z.n)./[.....
-00000a10: 173a 3592 551c 526a a4ef 0854 3582 ac91  .:5.U.Rj...T5...
-00000a20: 3769 7a2b add2 4e14 d958 db50 9161 cf46  7iz+..N..X.P.a.F
-00000a30: 3bd8 50e2 7b6b 159d 5660 70c8 c55c 4c85  ;.P.{k..V`p..\L.
-00000a40: ad6e 5a8e 0559 649d 6a60 07fc d66d 2864  .nZ..Yd.j`...m(d
-00000a50: f2ca 5269 0bce 6b74 0941 9d8b 87f9 7235  ..Ri..kt.A....r5
-00000a60: ce8f 03ef 1a06 ff2b 4ea2 9303 e231 262f  .......+N....1&/
-00000a70: 552e d228 080c 941c 1954 f87c c11a 8c89  U..(.....T.|....
-00000a80: 4441 c6e7 8553 5c57 46e0 ef78 627f 1abd  DA...S\WF..xb...
-00000a90: 072f 07e5 618d e643 57dc e6e2 5e24 15d4  ./..a..CW...^$..
-00000aa0: aa37 bcc5 e119 2e7e 1657 818f 8a55 9111  .7.....~.W...U..
-00000ab0: 0e09 459f 4556 c620 ee0e 73da c5fb ec98  ..E.EV. ..s.....
-00000ac0: 425d 8745 5c94 d83b a6d3 7eef 9485 4c72  B].E\..;..~...Lr
-00000ad0: 5012 1bb2 bc00 57ff 0207 7dd4 5558 aaab  P.....W...}.UX..
-00000ae0: bf70 1934 4cbe cea2 e2c1 5f15 35da f9c4  .p.4L....._.5...
-00000af0: 401d 68d3 d9dd 4224 7436 714e 18bb f1c1  @.h...B$t6qN....
-00000b00: 0ec8 8c76 0cdb f0ee 4071 20f4 6b44 9e92  ...v....@q .kD..
-00000b10: 78c3 eb9f 54fc 0050 4b03 0414 0000 0008  x...T..PK.......
-00000b20: 00cc 4e68 566e 633f 1e92 0100 00e8 0300  ..NhVnc?........
-00000b30: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00000b40: 7473 2f73 6865 6574 332e 786d 6c85 93db  ts/sheet3.xml...
-00000b50: 6ae4 300c 407f 25f8 03ea e942 b7a5 2481  j.0.@.%....B..$.
-00000b60: edf4 360f 0b43 4bbb 8fc5 9328 8919 dbca  ..6..CK....(....
-00000b70: ca9a 66e7 efd7 ca5c 2834 9027 4bb2 8e2c  ..f....\(4.'K..,
-00000b80: c952 3e20 6d63 07c0 d93f ef42 2c54 c7dc  .R> mc...?.B,T..
-00000b90: df6a 1dab 0ebc 8917 d843 4837 0d92 379c  .j.......CH7..7.
-00000ba0: 546a 75ec 094c 3d42 dee9 1f8b c54f ed8d  Tju..L=B.....O..
-00000bb0: 0daa cc47 db9a ca1c 77ec 6c80 3565 71e7  ...G....w.l.5eq.
-00000bc0: bda1 fd1d 381c 0a75 a94e 8617 db76 2c06  ....8..u.N...v,.
-00000bd0: 5de6 bd69 e115 f8ad 5f53 d2f4 394a 6d3d  ]..i...._S..9Jm=
-00000be0: 8468 3164 044d a17e 5dde ae46 ffd1 e1dd  .h1d.M.~]..F....
-00000bf0: c210 bfc8 9954 b241 dc8a b2aa 0bb5 9084  .....T.A........
-00000c00: c041 c512 c1a4 e313 96e0 9c04 4a69 fc3d  .A..........Ji.=
-00000c10: c654 e727 05fc 2a9f a23f 8eb5 a75a 3626  .T.'..*..?...Z6&
-00000c20: c212 dd1f 5b73 57a8 1b95 d5d0 989d e317  ....[sW.........
-00000c30: 1c9e e158 cfd5 39c1 7bc3 a6cc 0987 8ca4  ...X..9.{.......
-00000c40: ce32 af44 90b7 939f 0dd2 9f57 a664 b7e9  .2.D.......W.d..
-00000c50: 212e e113 027f 7c98 8a30 ec7d ae39 a522  !.....|..0.}.9."
-00000c60: 37ba 3a92 7733 640d b122 db4b b513 f472  7.:.w3d..".K...r
-00000c70: 8666 cb0e 26b8 fb19 ae43 0ff2 7f13 e8c3  .f..&....C......
-00000c80: 0c3a d8ad ad53 936c 3d01 3fce c011 c842  .:...S.l=.?....B
-00000c90: 9c00 9f66 c0ca f27e 027b 9ec3 7017 98a6  ...f...~.{..p...
-00000ca0: c8d5 0c49 d07e fb12 9dc6 e234 6a87 3991  ...I.~.....4j.9.
-00000cb0: 1efe 36d4 da10 3307 4d0a b8b8 b8be 5219  ..6...3.M.....R.
-00000cc0: 1de6 eaa0 30f6 e30e 6d90 19fd 2876 6915  ....0...m...(vi.
-00000cd0: 81c4 21dd 3788 7c52 64ac cfcb 5dfe 0750  ..!.7.|Rd...]..P
-00000ce0: 4b03 0414 0000 0008 00cc 4e68 56f1 ce3b  K.........NhV..;
-00000cf0: aa75 0100 0023 0300 0018 0000 0078 6c2f  .u...#.......xl/
-00000d00: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00000d10: 342e 786d 6c8d 53db 4ec3 300c fd95 2a1f  4.xml.S.N.0...*.
-00000d20: 4006 1217 4d6d 25d8 86e0 0169 6202 1e51  @...Mm%....ib..Q
-00000d30: d6ba 6bb4 242e 8e47 e1ef 89bb 8b86 b487  ..k.$..G........
-00000d40: 3dd5 b773 ece3 b879 8fb4 8e2d 0067 3fde  =..s...y...-.g?.
-00000d50: 8558 a896 b91b 6b1d ab16 bc89 17d8 4148  .X....k.......AH
-00000d60: 9906 c91b 4e2e ad74 ec08 4c3d 80bc d357  ....N..t..L=...W
-00000d70: a3d1 8df6 c606 55e6 436c 4e65 8e1b 7636  ......U.ClNe..v6
-00000d80: c09c b2b8 f1de d0ef 0338 ec0b 75a9 f681  .........8..u...
-00000d90: 57bb 6a59 02ba cc3b b382 05f0 5b37 a7e4  W.jY...;....[7..
-00000da0: e903 4b6d 3d84 6831 6404 4da1 ee2f c7b3  ..Km=.h1d.M../..
-00000db0: a17e 2878 b7d0 c723 3b13 254b c4b5 38cf  .~(x...#;.%K..8.
-00000dc0: 75a1 4632 1038 a858 184c fa7c c304 9c13  u.F2.8.X.L.|....
-00000dd0: a234 c6d7 8e53 1d5a 0af0 d8de b33f 0eda  .4...S.Z.....?..
-00000de0: 9396 a589 3041 f761 6b6e 0b75 a7b2 1a1a  ....0A.akn.u....
-00000df0: b371 fc8a fd13 ecf4 5c1f 069c 1a36 654e  .q......\....6eN
-00000e00: d867 243a cbbc 1243 7aa7 3a1b 643f 0ba6  .g$:...Cz.:.d?..
-00000e10: 14b7 a911 97f0 0d81 1740 16e2 e7a7 a908  .........@......
-00000e20: c3af cf35 a781 24af ab1d fee1 2c7c 0db1  ...5..$.....,|..
-00000e30: 22db 89f2 131c 93b3 38d8 b283 13e8 e959  ".......8......Y
-00000e40: e8de ae6d 9d36 60eb 1314 b3b3 285a f420  ...m.6`.....(Z. 
-00000e50: a7f1 9f40 a78d ee5f 69bb 62a9 7931 b4b2  ...@..._i.b.y1..
-00000e60: 2166 0e9a 443c bab8 bd56 196d 9f64 eb30  !f..D<...V.m.d.0
-00000e70: 76c3 f92d 9119 fd60 b6e9 8a81 a420 e51b  v..-...`..... ..
-00000e80: 44de 3b72 1187 ffa2 fc03 504b 0304 1400  D.;r......PK....
-00000e90: 0000 0800 cc4e 6856 7ee8 1a77 7301 0000  .....NhV~..ws...
-00000ea0: 2203 0000 1800 0000 786c 2f77 6f72 6b73  ".......xl/works
-00000eb0: 6865 6574 732f 7368 6565 7435 2e78 6d6c  heets/sheet5.xml
-00000ec0: 8d53 db4e c330 0cfd 952a 1f40 0ad2 004d  .S.N.0...*.@...M
-00000ed0: 6d25 3640 f080 346d 021e 51d6 ba6b b4a4  m%6@..4m..Q..k..
-00000ee0: 2e89 47e1 efb1 bbad 0269 0f7b aa6f e7f8  ..G......i.{.o..
-00000ef0: d84e b31e c336 3600 947c 7bd7 c65c 3544  .N...66..|{..\5D
-00000f00: dd54 eb58 36e0 4dbc c00e 5ace d418 bc21  .T.X6.M...Z....!
-00000f10: 76c3 46c7 2e80 a906 9077 fa2a 4daf b537  v.F......w.*M..7
-00000f20: b655 4536 c416 a1c8 7047 ceb6 b008 49dc  .UE6....pG....I.
-00000f30: 796f c2cf 0c1c f6b9 ba54 c7c0 d26e 1a92  yo.......T...n..
-00000f40: 802e b2ce 6c60 05f4 da2d 027b 7a64 a9ac  ....l`...-.{zd..
-00000f50: 8736 5a6c 9300 75ae ee2e a70f 43fd 50f0  .6Zl..u.....C.P.
-00000f60: 66a1 8f7f ec44 2659 236e c579 ae72 958a  f....D&Y#n.y.r..
-00000f70: 2070 5092 3018 fe7c c11c 9c13 2296 f179   pP.0..|...."..y
-00000f80: e054 634b 01fe b58f ec8f c3ec 3ccb da44  .TcK........<..D
-00000f90: 98a3 7bb7 1535 b9ba 5549 05b5 d939 5a62  ..{..5..UI...9Zb
-00000fa0: ff04 8779 26a3 c07b 43a6 c802 f649 9039  ...y&..{C....I.9
-00000fb0: 8bac 1443 7a73 9d6d 653f 2b0a 1cb7 dc88  ...Czs.me?+.....
-00000fc0: 0adb 46b2 b413 b11f 1f6c 39c8 34b1 1cc9  ..F......l9.4...
-00000fd0: eaf2 809e 9d85 eeed d656 dcdd 5627 28e6  .........V..V'(.
-00000fe0: 6751 34e8 41ce 7282 e0fe 2c82 c847 a6f9  gQ4.A.r...,..G..
-00000ff0: f2e5 f994 8687 f328 ca06 9d09 fff1 9a17  .......(........
-00001000: 7a3c d27e c322 f3c5 840d 6313 0735 f3a6  z<.~."....c..5..
-00001010: 1737 1395 84fd 45f6 0e61 37bc be35 12a1  .7....E..a7..5..
-00001020: 1fcc 861f 3104 29e0 7c8d 4847 471e c4f8  ....1.).|.HGG...
-00001030: 5b14 bf50 4b03 0414 0000 0008 00cc 4e68  [..PK.........Nh
-00001040: 56e6 b41a c574 0100 0038 0300 0018 0000  V....t...8......
-00001050: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00001060: 6865 6574 362e 786d 6c85 935b 4bc3 3014  heet6.xml..[K.0.
-00001070: 80ff 4ac9 0f58 36c1 0ba3 2de8 e6d0 0761  ..J..X6...-....a
-00001080: 28d3 c791 35a7 6b58 d213 4fce acfe 7b93  (...5.kX..O...{.
-00001090: ee82 c2a0 4f3d b7ef dc72 9a77 48bb d000  ....O=...r.wH...
-000010a0: 70f6 ed6c 1b0a d130 fba9 94a1 6ac0 a930  p..l...0....j..0
-000010b0: 420f 6df4 d448 4e71 5469 2b83 2750 ba87  B.m..HNqTi+.'P..
-000010c0: 9c95 57e3 f18d 74ca b4a2 cc7b db92 ca1c  ..W...t....{....
-000010d0: f76c 4d0b 4bca c2de 3945 3f0f 60b1 2bc4  .lM.K...9E?.`.+.
-000010e0: 449c 0caf 66db 7032 c832 f76a 0b6f c02b  D...f.p2.2.j.o.+
-000010f0: bfa4 a8c9 7316 6d1c b4c1 609b 11d4 85b8  ....s.m...`.....
-00001100: 9f4c 177d 7c1f f06e a00b 7fe4 2c4d b241  .L.}|..n....,M.A
-00001110: dc25 e559 1762 9c1a 020b 15a7 0c2a 7ebe  .%.Y.b.......*~.
-00001120: 6006 d6a6 44b1 8dcf 634e 712e 99c0 bff2  `...D...cNq.....
-00001130: 29fb a29f 3dce b251 0166 683f 8ce6 a610  )...=..Q.fh?....
-00001140: 7722 d350 abbd e557 ec9e e038 cff5 b9c1  w".P...W...8....
-00001150: b962 55e6 845d 4669 ce32 af92 906a c738  .bU..]Fi.2...j.8
-00001160: d3a6 fdbc 3145 bb89 85b8 f4ca 03ad d71a  ....1E..........
-00001170: 4245 c6a7 9e73 c9b1 9de4 95d5 917e 18a0  BE...s.......~..
-00001180: 8dbe 00cd 06a0 ceec 8c8e cd5e 84e7 0330  ...........^...0
-00001190: 1bb6 7081 7b1c e0d4 9e1b a470 815c 0c90  ..p.{......p.\..
-000011a0: 5ed7 2bb2 ff41 19d7 7c7a bac3 ded3 4dbd  ^.+..A..|z....M.
-000011b0: 28da 9a36 6416 ea98 703c babd 1619 1dde  (..6d...p<......
-000011c0: e9a0 30fa fe26 37c8 8cae 179b 78da 4029  ..0..&7.....x.@)
-000011d0: 20fa 6b44 3e29 e94c ce3f 4bf9 0b50 4b03   .kD>).L.?K..PK.
-000011e0: 0414 0000 0008 00cc 4e68 56fa f742 c353  ........NhV..B.S
-000011f0: 0100 005e 0200 0018 0000 0078 6c2f 776f  ...^.......xl/wo
-00001200: 726b 7368 6565 7473 2f73 6865 6574 372e  rksheets/sheet7.
-00001210: 786d 6c8d 52c1 4ec3 300c fd95 281f b074  xml.R.N.0...(..t
-00001220: 4803 34b5 95d8 1082 03d2 b409 384e 59e3  H.4.........8NY.
-00001230: b6d1 92b8 241e 85bf 27e9 d66a dc38 c576  ....$...'..j.8.v
-00001240: 9e9f df73 92f7 e88f a105 20f6 6d8d 0b05  ...s...... .m...
-00001250: 6f89 baa5 10a1 6ac1 ca30 c30e 5cbc a9d1  o.....j..0..\...
-00001260: 5b49 31f5 8d08 9d07 a986 266b c44d 96dd  [I1.......&k.M..
-00001270: 0a2b b5e3 653e d436 becc f144 463b d878  .+..e>.6...DF;.x
-00001280: 164e d64a ffb3 0283 7dc1 e77c 2c6c 75d3  .N.J....}..|,lu.
-00001290: 522a 8832 ef64 033b a0b7 6ee3 6326 2616  R*.2.d.;..n.c&&.
-000012a0: a52d b8a0 d131 0f75 c11f e6cb d580 1f00  .-...1.u........
-000012b0: ef1a fa70 15b3 e4e4 8078 4cc9 8b2a 7896  ...p.....xL..*x.
-000012c0: 0481 818a 1283 8cc7 17ac c198 4414 657c  ............D.e|
-000012d0: 5e38 f934 3235 5ec7 23fb d3e0 3d7a 39c8  ^8.425^.#...=z9.
-000012e0: 006b 341f 5a51 5bf0 7bce 14d4 f264 688b  .k4.ZQ[.{....dh.
-000012f0: fd33 5cfc 2c26 818f 9264 997b ec99 4f3e  .3\.,&...d.{..O>
-00001300: cbbc 4a41 9a1d 71da a5fd ecc8 c7ba 8e83  ..JA..q.........
-00001310: a8ec 3c56 004a bb26 ecf7 bd3e 6a15 fbb5  ..<V.J.&...>j...
-00001320: ca05 454d 0922 aa0b c5ea 5f14 a4c9 c0df  ..EM."...._.....
-00001330: 6e11 c58c 06cf ead2 e65f a56f b40b cc40  n........_.o...@
-00001340: 1d59 b3d9 dd82 337f 7673 4e08 bbe1 e50e  .Y....3.vsN.....
-00001350: 4884 7608 dbf8 01c0 2740 bcaf 1169 4cd2  H.v.....'@...iL.
-00001360: 32a7 2f55 fe02 504b 0304 1400 0000 0800  2./U..PK........
-00001370: cc4e 6856 1722 a865 4f01 0000 5302 0000  .NhV.".eO...S...
-00001380: 1800 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00001390: 732f 7368 6565 7438 2e78 6d6c 8552 c14e  s/sheet8.xml.R.N
-000013a0: c330 0cfd 952a 1fb0 7448 0334 b595 d810  .0...*..tH.4....
-000013b0: 8203 d2b4 0938 4e59 ebb6 d192 b824 1e85  .....8NY.....$..
-000013c0: bfc7 e9d6 6a9c 38c5 7eb1 9fdf 7392 f5e8  ....j.8.~...s...
-000013d0: 8fa1 05a0 e4db 1a17 72d1 1275 4b29 43d9  ........r..uK)C.
-000013e0: 8255 6186 1d38 bea9 d15b 459c fa46 86ce  .Ua..8...[E..F..
-000013f0: 83aa 8626 6be4 4d9a de4a abb4 1345 3660  ...&k.M..J...E6`
-00001400: 1b5f 6478 22a3 1d6c 7c12 4ed6 2aff b302  ._dx"..l|.N.*...
-00001410: 837d 2ee6 6204 b6ba 6929 02b2 c83a d5c0  .}..b...i)...:..
-00001420: 0ee8 addb 78ce e4c4 5269 0b2e 6874 8987  ....x...Ri..ht..
-00001430: 3a17 0ff3 e56a a81f 0ade 35f4 e12a 4ea2  :....j....5..*N.
-00001440: 9303 e231 262f 552e d228 080c 9414 1914  ...1&/U..(......
-00001450: 1f5f b006 6322 11cb f8bc 708a 6964 6cbc  ._..c"....p.idl.
-00001460: 8e47 f6a7 c13b 7b39 a800 6b34 1fba a236  .G...;{9..k4...6
-00001470: 17f7 22a9 a056 2743 5bec 9fe1 e267 3109  .."..V'C[....g1.
-00001480: 7c54 a48a cc63 9ff8 e8b3 c8ca 18c4 d95c  |T...c.........\
-00001490: a75d dccf 8e3c e39a 0751 e1a1 619d fbbd  .]...<...Q..a...
-000014a0: 5316 3249 2c24 e2b2 bcf4 adfe ebeb f551  S.2I,$.........Q
-000014b0: 573c 5257 7fbb 252b 185d 9d25 c575 bf2a  W<RW..%+.].%.u.*
-000014c0: df68 1712 0335 b3a6 b3bb 8548 fcd9 c239  .h...5.....H...9
-000014d0: 21ec 86e7 3a20 11da 216c f9d5 c1c7 02be  !...: ..!l......
-000014e0: af11 694c e206 a77f 54fc 0250 4b03 0414  ..iL....T..PK...
-000014f0: 0000 0008 00cc 4e68 5652 999d 75ba 0100  ......NhVR..u...
-00001500: 00c4 0400 0018 0000 0078 6c2f 776f 726b  .........xl/work
-00001510: 7368 6565 7473 2f73 6865 6574 392e 786d  sheets/sheet9.xm
-00001520: 6c85 94e9 6edb 300c 805f c5d0 0354 e980  l...n.0.._...T..
-00001530: ae43 e118 68d3 2b5b 3b04 09ba fd2c 149b  .C..h.+[;....,..
-00001540: b685 48a2 4731 f3f6 f693 9c03 c520 40bf  ..H.G1....... @.
-00001550: cc43 1f2f 8b2a 47a4 9def 01b8 f863 8df3  .C./.*G......c..
-00001560: 73d1 330f 3752 faba 07ab fc05 0ee0 82a7  s.3.7R..........
-00001570: 45b2 8a83 4a9d f403 816a 26c8 1af9 6936  E...J....j&...i6
-00001580: fb2c add2 4e54 e564 5b51 55e2 9e8d 76b0  .,..NT.d[QU...v.
-00001590: a2c2 efad 55f4 f70e 0c8e 7371 294e 86b5  ....U.....sq)N..
-000015a0: ee7a 8e06 5995 83ea 6003 fc36 ac28 68f2  .z..Y...`..6.(h.
-000015b0: 1ca5 d116 9cd7 e80a 8276 2e6e 2f6f 5ea6  .........v.n/o^.
-000015c0: f3d3 811f 1a46 ff41 2e62 275b c45d 5496  .....F.A.b'[.]T.
-000015d0: cd5c cc62 4160 a0e6 1841 85cf 6f58 8031  .\.bA`...A..oX.1
-000015e0: 3150 28e3 d731 a638 a78c e047 f914 fd71  1P(..1.8...G...q
-000015f0: ea3d f4b2 551e 1668 7eea 86fb b9f8 228a  .=..U..h~.....".
-00001600: 065a b537 bcc6 f119 8efd 5c9d 0bbc 57ac  .Z.7......\...W.
-00001610: aa92 702c 28f6 5995 7514 62ee 704e bb38  ..p,(.Y.u.b.pN.8
-00001620: 9f0d 53b0 eb90 88ab 3070 348a dedf 47bd  ..S.....0p4...G.
-00001630: d391 5d36 a5e4 504f 74cb fa88 df65 71a7  ..]6..POt....eq.
-00001640: 2c24 c045 166c 3579 fe9e a6ef b374 03be  ,$.E.l5y.....t..
-00001650: 263d c459 27f8 872c dfa3 8578 0f12 f063  &=.Y'..,...x...c
-00001660: 1646 aa75 6a5a 4ff9 b2b7 6648 0efa 398b  .F.ujZO...fH..9.
-00001670: 7688 9d81 cd41 7df3 4089 28cb 6c94 e0d8  v....A}.@.(.l...
-00001680: 41b3 74c9 22be 6671 020f 8aea fe49 716a  A.t.".fq.....Iqj
-00001690: 74df f25d b826 99fa 254b fab0 c6bc 58bf  t..].&..%K....X.
-000016a0: fe8f cb70 e54f 6b74 d881 f85f 5f15 75da  ...p.Okt...__.u.
-000016b0: f9c2 401b c2ce 2eae af44 4187 9d39 288c  ..@......DA..9(.
-000016c0: c3f4 3e6c 9119 ed24 f6e1 9901 8a07 82bf  ..>l...$........
-000016d0: 45e4 9312 57f6 fc70 55ff 0050 4b03 0414  E...W..pU..PK...
-000016e0: 0000 0008 00cc 4e68 567c f3a3 dc51 0200  ......NhV|...Q..
-000016f0: 00f6 0900 000d 0000 0078 6c2f 7374 796c  .........xl/styl
-00001700: 6573 2e78 6d6c dd56 db8a db30 10fd 15e1  es.xml.V...0....
-00001710: 0fa8 9398 3571 49f2 5043 60a1 2d0b bb0f  ....5qI.PC`.-...
-00001720: 7d55 6239 11e8 e2ca f292 f4eb 3b23 3976  }Ub9........;#9v
-00001730: b3ab 5928 7dab 4df0 cc1c 9db9 1b67 d3fb  ..Y(}.M......g..
-00001740: ab12 cf67 213c bb68 65fa 6d76 f6be fb9c  ...g!<.he.mv....
-00001750: e7fd f12c 34ef 3fd9 4e18 405a eb34 f7a0  ...,4.?.N.@Z.4..
-00001760: ba53 de77 4ef0 a647 9256 f96a b128 73cd  .S.wN..G.V.j.(s.
-00001770: a5c9 761b 33e8 bdf6 3d3b dac1 f86d b6c8  ..v.3...=;...m..
-00001780: f2dd a6b5 66b6 2cb3 6880 a35c 0bf6 cad5  ....f.,.h..\....
-00001790: 36ab b992 0727 c359 aea5 ba46 f30a 0d47  6....'.Y...F...G
-000017a0: abac 631e 5211 4806 4bff 2bc2 cba8 6196  ..c.R.H.K.+...a.
-000017b0: a31f 2d8d 7568 cc63 84f0 e8c1 a954 6a4a  ..-.uh.c.....TjJ
-000017c0: 6095 45c3 6ed3 71ef 8533 7b50 0227 18df  `.E.n.q..3{P.'..
-000017d0: 416c 945f ae1d 6470 72fc ba5c 3d64 3321  Al._..dpr..\=d3!
-000017e0: 3c20 c8c1 ba46 b8bb 3aa3 69b7 51a2 f540  < ...F..:.i.Q..@
-000017f0: 70f2 74c6 a7b7 5d8e a0f7 5683 d048 7eb2  p.t...]...V..H~.
-00001800: 8687 1c6e 8c51 00b7 47a1 d433 8ee8 477b  ...n.Q..G..3..G{
-00001810: e7fb d2b2 d8eb c706 dbcc b0d4 9b08 098d  ................
-00001820: 6274 1315 f4ff a7b7 e8fb 9fdd b24e be5a  bt...........N.Z
-00001830: ff65 806a 4cd0 7f0e d68b 2727 5a79 09fa  .e.jL.....''Zy..
-00001840: a5bd 8f3f 850e 89dc 459f ac0c 9763 9b7d  ...?....E....c.}
-00001850: c79d 53b3 0b76 18a4 f2d2 8cda 5936 8d30  ..S..v......Y6.0
-00001860: ef6a 03f7 9e1f 60a9 effc c3f9 46b4 7c50  .j....`.....F.|P
-00001870: fe65 02b7 d92c 7f13 8d1c 7435 9d7a c2b2  .e...,....t5.z..
-00001880: c653 b3fc 1567 b82c a7cd 8458 d234 e222  .S...g.,...X.4."
-00001890: 9a7a 54dd e910 4406 0244 1d2f 24bc 45f6  .zT...D..D./$.E.
-000018a0: e14a 2314 2762 6904 312a 0e95 01c5 892c  .J#.'bi.1*.....,
-000018b0: 2ace ff54 cf9a ac27 6254 6eeb 24b2 2639  *..T...'bTn.$.&9
-000018c0: 6b92 1359 29a4 0e37 1527 cda9 e04a 575a  k..Y)..7.'...JWZ
-000018d0: 5545 5196 5447 eb3a 9941 4df5 ad2c f197  UEQ.TG.:.AM..,..
-000018e0: f646 e586 0c2a 0e46 fabb 5ed3 d3a6 37e4  .F...*.F..^...7.
-000018f0: e33d a066 fad1 8650 95d2 9b48 554a f71a  .=.f...P...HUJ..
-00001900: 9174 df90 5155 e969 5371 9041 4d81 da1d  .t..QU.iSq.AM...
-00001910: 8c9f 8e83 3b95 e614 054e 95ca 8d7a 8369  ....;....N...z.i
-00001920: a4aa 2804 7731 bda3 6549 74a7 c43b 3d1f  ..(.w1..eIt..;=.
-00001930: ea2d 298a aa4a 2388 a533 280a 0ac1 b791  .-)..J#..3(.....
-00001940: 46a8 0c30 070a 298a f01d 7cf3 3dca 6fdf  F..0..)...|.=.o.
-00001950: a97c fea7 b7fb 0d50 4b03 0414 0000 0008  .|.....PK.......
-00001960: 00cc 4e68 5697 8abb 1cc0 0000 0013 0200  ..NhV...........
-00001970: 000b 0000 005f 7265 6c73 2f2e 7265 6c73  ....._rels/.rels
-00001980: 9d92 b96e c330 0c40 7fc5 d09e 3007 d021  ...n.0.@....0..!
-00001990: 8833 65f1 1604 f901 56a2 0fd8 1205 8a45  .3e.....V......E
-000019a0: 9dbf afda a571 900b 1979 3d3c 12dc 1e69  .....q...y=<...i
-000019b0: 40ed 38a4 b68b a918 fd10 5269 5ad5 b801  @.8.......RiZ...
-000019c0: 48b6 258f 69ce 9142 aed4 2c1e 3587 d240  H.%.i..B..,.5..@
-000019d0: 44db 6343 b05a 2c3e 402e 1966 b7bd 6416  D.cC.Z,>@..f..d.
-000019e0: a773 a457 885c d79d a53d db2f 4f41 6f80  .s.W.\...=./OAo.
-000019f0: af3a 4c71 4269 484b 330e f0cd d27f 32f7  .:LqBiHK3.....2.
-00001a00: f30c 3545 e54a 2395 5b1a 78d3 e5fe 76e0  ..5E.J#.[.x...v.
-00001a10: 49d1 a122 5816 9a45 c9d3 a21d a57f 1dc7  I.."X..E........
-00001a20: f690 d3e9 af63 22b4 7a5b e8f9 7168 540a  .....c".z[..qhT.
-00001a30: 8edc 6325 8c71 62b4 fe35 82c9 0fec 7e00  ..c%.qb..5....~.
-00001a40: 504b 0304 1400 0000 0800 cc4e 6856 cda6  PK.........NhV..
-00001a50: beb4 a501 0000 9006 0000 0f00 0000 786c  ..............xl
-00001a60: 2f77 6f72 6b62 6f6f 6b2e 786d 6cbd 95c1  /workbook.xml...
-00001a70: 6edb 300c 865f c5d0 03cc 699a a469 50f7  n.0.._....i..iP.
-00001a80: d276 5b80 610b 9aa1 77c5 a663 a2b2 6850  .v[.a...w..c..hP
-00001a90: 74b2 f5e9 473b 30aa 6180 b18b 7b92 f853  t...G;0.a...{..S
-00001aa0: f8f1 9184 e9bb 33f1 eb81 e835 f955 3b1f  ......3....5.U;.
-00001ab0: 3253 8934 9b34 0d79 05b5 0d9f a801 af99  2S.4.4.y........
-00001ac0: 92b8 b6a2 211f d3d0 30d8 2254 0052 bb74  ....!...0."T.R.t
-00001ad0: 3e9b add2 daa2 37f7 7783 d78e d338 2081  >.....7.w....8 .
-00001ae0: 5c90 bc8a 9df0 8270 0eef f92e 4c4e 18f0  \......p....LN..
-00001af0: 800e e577 66fa bb03 93d4 e8b1 c637 2832  ...wf........7(2
-00001b00: 3333 49a8 e8fc 9518 dfc8 8b75 fb9c c9b9  33I........u....
-00001b10: cc5c 5d12 2fc0 82f9 3ff2 be83 fc69 0fa1  .\]./...?....i..
-00001b20: 57c4 1e9e ad82 6466 3553 c312 3948 ffa2  W.....df5S..9H..
-00001b30: f7b7 ca78 027d 9c99 b546 add0 6774 02fc  ...x.}...F..gt..
-00001b40: 6805 be30 b50d fa63 67a3 55a4 5119 7d1f  h..0...cg.U.Q.}.
-00001b50: 86f3 d2c4 0dff 4f1b a92c 3187 47ca db1a  ......O..,1.G...
-00001b60: bc5c fac8 e03a 401f 2a6c 8249 bcad 2133  .\...:@.*l.I..!3
-00001b70: 0fda 95ae 1cf5 df16 97d2 4499 a246 f106  ..........D..F..
-00001b80: 35c1 dba2 a79b 9084 5a2f 1cc3 cc47 60e6  5.......Z/...G`.
-00001b90: d3c2 3c9d 341f a15c 8fa0 5c7f 00ca 1e18  ..<.4..\..\.....
-00001ba0: 2144 408b 11a0 c5b4 405b 1f04 a5ed f408  !D@.....@[......
-00001bb0: 6839 02b4 9c16 6867 1be0 0865 3582 b29a  h9....hg...e5...
-00001bc0: 1885 2907 28f4 6b8e 8775 3302 7433 2dd0  ..).(.k..u3.t3-.
-00001bd0: 331c ff9e d37a 8465 3d2d cb3e afc8 d978  3....z.e=-.>...x
-00001be0: 52b7 2330 b7fd 321c 3660 0125 7a28 beab  R.#0..2.6`.%z(..
-00001bf0: 5150 5db7 71be e3a4 3bfa b535 5f2c afd4  QP].q...;..5_,..
-00001c00: ac6c 9d7b 50ed 87ff 46b6 1816 eaf0 33b8  .l.{P...F.....3.
-00001c10: ff03 504b 0304 1400 0000 0800 cc4e 6856  ..PK.........NhV
-00001c20: 7b0c faf9 dd00 0000 8206 0000 1a00 0000  {...............
-00001c30: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
-00001c40: 6b2e 786d 6c2e 7265 6c73 c5d5 cd0e 8230  k.xml.rels.....0
-00001c50: 0c07 f057 217b 008b 80f8 11e0 e4c5 abf1  ...W!{..........
-00001c60: 0516 2c1f 11d8 b2d6 a86f 2fc1 03d6 78f0  ..,......o/...x.
-00001c70: 6276 5ada 65ff fe4e 5d76 c44e 736b 066a  bvZ.e..N]v.Nsk.j
-00001c80: 5a4b c1bd ef06 ca55 c36c 7700 5436 d86b  ZK.....U.lw.T6.k
-00001c90: 5a18 8bc3 7853 19d7 6b1e 4b57 83d5 e545  Z...xS..k.KW...E
-00001ca0: d708 5118 a6e0 de33 5491 bd67 06a7 87c5  ..Q....3T..g....
-00001cb0: 5f12 4d55 b525 ee4d 79ed 71e0 2fc1 7033  _.MU.%.My.q./.p3
-00001cc0: ee42 0d22 abe0 a45d 8d9c 2bb8 7773 9b60  .B."...]..+.ws.`
-00001cd0: 3a96 8b31 5905 8773 aedc e1bc 54e0 1b14  :..1Y..s....T...
-00001ce0: 0950 e41f 140b 50ec 1f94 0850 e21f b412  .P....P....P....
-00001cf0: a095 7f50 2a40 a97f d05a 80d6 fe41 1b01  ...P*@...Z...A..
-00001d00: daf8 076d 0568 fb47 10f1 a343 9a35 af5a  ...m.h.G...C.5.Z
-00001d10: aec1 f08f f379 7c8b f3f8 a97c 353f 76f1  .....y|....|5?v.
-00001d20: b48c 417c 39c5 1350 4b03 0414 0000 0008  ..A|9..PK.......
-00001d30: 00cc 4e68 5647 aed8 393a 0100 000f 0800  ..NhVG..9:......
-00001d40: 0013 0000 005b 436f 6e74 656e 745f 5479  .....[Content_Ty
-00001d50: 7065 735d 2e78 6d6c cd96 cb4e c330 1045  pes].xml...N.0.E
-00001d60: 7f25 cab6 6a5c 0a94 87da 6e80 2d74 c10f  .%..j\....n.-t..
-00001d70: 9864 d258 f54b 9e69 49ff 9e49 fa90 4025  .d.X.K.iI..I..@%
-00001d80: 6a15 24bc 8915 cfcc 3dd7 330b 7bfa bef5  j.$.....=.3.{...
-00001d90: 8049 6db4 c559 5a11 f947 2130 afc0 48cc  .Im..YZ..G!0..H.
-00001da0: 9c07 cb91 d205 2389 7fc3 5278 99af e412  ......#...Rx....
-00001db0: c478 349a 88dc 5902 4b43 6a34 d2f9 f419  .x4...Y.KCj4....
-00001dc0: 4ab9 d694 bcd4 bc8d cad9 591a 4063 9a3c  J.........Y.@c.<
-00001dd0: ed12 1bd6 2c95 de6b 954b e2b8 d8d8 e207  ....,..k.K......
-00001de0: 65b8 2764 5cd9 e660 a53c 0e38 2115 2709  e.'d\..`.<.8!.'.
-00001df0: 4de4 77c0 beee 6d03 21a8 0292 850c f42a  M.w...m.!......*
-00001e00: 0d67 895a 0ba4 ad06 ccba 254e 7874 65a9  .g.Z......%Nxte.
-00001e10: 7228 5cbe 365c 92a1 0f20 0bac 00c8 e86c  r(\.6\... .....l
-00001e20: 273a e826 1377 1876 dfab defc 56a6 0bc8  ':.&.w.v....V...
-00001e30: 998b e03c f2c4 025c 8e3b 8ca4 a91e 7a16  ...<...\.;....z.
-00001e40: 8240 aafb 8847 224b f73e 1f34 d32e a038  .@...G"K.>.4...8
-00001e50: 93cd edfd 7461 d5ce 0345 bbf4 eff1 f719  ....ta...E......
-00001e60: 1ff5 2ff4 318e c4c7 7524 3e6e 22f1 711b  ../.1...u$>n".q.
-00001e70: 898f 4924 3eee 22f1 711f 898f 877f f4f1  ..I$>.".q.......
-00001e80: e1dc eaaf afa8 66cd 8c54 f6c0 17ed 3b60  ......f..T....;`
-00001e90: fe05 504b 0102 1403 1400 0000 0800 cc4e  ..PK...........N
-00001ea0: 6856 0741 4d62 8100 0000 b100 0000 1000  hV.AMb..........
-00001eb0: 0000 0000 0000 0000 0000 8001 0000 0000  ................
-00001ec0: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
-00001ed0: 504b 0102 1403 1400 0000 0800 cc4e 6856  PK...........NhV
-00001ee0: d1f9 d168 ef00 0000 2b02 0000 1100 0000  ...h....+.......
-00001ef0: 0000 0000 0000 0000 8001 af00 0000 646f  ..............do
-00001f00: 6350 726f 7073 2f63 6f72 652e 786d 6c50  cProps/core.xmlP
-00001f10: 4b01 0214 0314 0000 0008 00cc 4e68 5699  K...........NhV.
-00001f20: 5c9c 2310 0600 009c 2700 0013 0000 0000  \.#.....'.......
-00001f30: 0000 0000 0000 0080 01cd 0100 0078 6c2f  .............xl/
-00001f40: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
-00001f50: 504b 0102 1403 1400 0000 0800 cc4e 6856  PK...........NhV
-00001f60: e6d2 6d07 4d01 0000 4f02 0000 1800 0000  ..m.M...O.......
-00001f70: 0000 0000 0000 0000 8081 0e08 0000 786c  ..............xl
-00001f80: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00001f90: 7431 2e78 6d6c 504b 0102 1403 1400 0000  t1.xmlPK........
-00001fa0: 0800 cc4e 6856 243f a25d 5001 0000 5502  ...NhV$?.]P...U.
-00001fb0: 0000 1800 0000 0000 0000 0000 0000 8081  ................
-00001fc0: 9109 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00001fd0: 732f 7368 6565 7432 2e78 6d6c 504b 0102  s/sheet2.xmlPK..
-00001fe0: 1403 1400 0000 0800 cc4e 6856 6e63 3f1e  .........NhVnc?.
-00001ff0: 9201 0000 e803 0000 1800 0000 0000 0000  ................
-00002000: 0000 0000 8081 170b 0000 786c 2f77 6f72  ..........xl/wor
-00002010: 6b73 6865 6574 732f 7368 6565 7433 2e78  ksheets/sheet3.x
-00002020: 6d6c 504b 0102 1403 1400 0000 0800 cc4e  mlPK...........N
-00002030: 6856 f1ce 3baa 7501 0000 2303 0000 1800  hV..;.u...#.....
-00002040: 0000 0000 0000 0000 0000 8081 df0c 0000  ................
-00002050: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00002060: 6565 7434 2e78 6d6c 504b 0102 1403 1400  eet4.xmlPK......
-00002070: 0000 0800 cc4e 6856 7ee8 1a77 7301 0000  .....NhV~..ws...
-00002080: 2203 0000 1800 0000 0000 0000 0000 0000  "...............
-00002090: 8081 8a0e 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-000020a0: 6574 732f 7368 6565 7435 2e78 6d6c 504b  ets/sheet5.xmlPK
-000020b0: 0102 1403 1400 0000 0800 cc4e 6856 e6b4  ...........NhV..
-000020c0: 1ac5 7401 0000 3803 0000 1800 0000 0000  ..t...8.........
-000020d0: 0000 0000 0000 8081 3310 0000 786c 2f77  ........3...xl/w
-000020e0: 6f72 6b73 6865 6574 732f 7368 6565 7436  orksheets/sheet6
-000020f0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00002100: cc4e 6856 faf7 42c3 5301 0000 5e02 0000  .NhV..B.S...^...
-00002110: 1800 0000 0000 0000 0000 0000 8081 dd11  ................
-00002120: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00002130: 7368 6565 7437 2e78 6d6c 504b 0102 1403  sheet7.xmlPK....
-00002140: 1400 0000 0800 cc4e 6856 1722 a865 4f01  .......NhV.".eO.
-00002150: 0000 5302 0000 1800 0000 0000 0000 0000  ..S.............
-00002160: 0000 8081 6613 0000 786c 2f77 6f72 6b73  ....f...xl/works
-00002170: 6865 6574 732f 7368 6565 7438 2e78 6d6c  heets/sheet8.xml
-00002180: 504b 0102 1403 1400 0000 0800 cc4e 6856  PK...........NhV
-00002190: 5299 9d75 ba01 0000 c404 0000 1800 0000  R..u............
-000021a0: 0000 0000 0000 0000 8081 eb14 0000 786c  ..............xl
-000021b0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-000021c0: 7439 2e78 6d6c 504b 0102 1403 1400 0000  t9.xmlPK........
-000021d0: 0800 cc4e 6856 7cf3 a3dc 5102 0000 f609  ...NhV|...Q.....
-000021e0: 0000 0d00 0000 0000 0000 0000 0000 8001  ................
-000021f0: db16 0000 786c 2f73 7479 6c65 732e 786d  ....xl/styles.xm
-00002200: 6c50 4b01 0214 0314 0000 0008 00cc 4e68  lPK...........Nh
-00002210: 5697 8abb 1cc0 0000 0013 0200 000b 0000  V...............
-00002220: 0000 0000 0000 0000 0080 0157 1900 005f  ...........W..._
-00002230: 7265 6c73 2f2e 7265 6c73 504b 0102 1403  rels/.relsPK....
-00002240: 1400 0000 0800 cc4e 6856 cda6 beb4 a501  .......NhV......
-00002250: 0000 9006 0000 0f00 0000 0000 0000 0000  ................
-00002260: 0000 8001 401a 0000 786c 2f77 6f72 6b62  ....@...xl/workb
-00002270: 6f6f 6b2e 786d 6c50 4b01 0214 0314 0000  ook.xmlPK.......
-00002280: 0008 00cc 4e68 567b 0cfa f9dd 0000 0082  ....NhV{........
-00002290: 0600 001a 0000 0000 0000 0000 0000 0080  ................
-000022a0: 0112 1c00 0078 6c2f 5f72 656c 732f 776f  .....xl/_rels/wo
-000022b0: 726b 626f 6f6b 2e78 6d6c 2e72 656c 7350  rkbook.xml.relsP
-000022c0: 4b01 0214 0314 0000 0008 00cc 4e68 5647  K...........NhVG
-000022d0: aed8 393a 0100 000f 0800 0013 0000 0000  ..9:............
-000022e0: 0000 0000 0000 0080 0127 1d00 005b 436f  .........'...[Co
-000022f0: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-00002300: 504b 0506 0000 0000 1100 1100 6e04 0000  PK..........n...
-00002310: 921e 0000 0000                           ......
+000000e0: c14a c430 1086 5f45 726f 274d 6091 d0ed  .J.0.._Ero'M`...
+000000f0: 45f1 a420 b8a0 780b 93d9 dd60 d386 64a4  E.. ..x....`..d.
+00000100: ddb7 b7ad bb5d 441f c063 66fe 7cf3 0d4c  .....]D..cf.|..L
+00000110: 8dd1 609f e839 f591 127b ca37 6368 bb6c  ..`..9...{.7ch.l
+00000120: 306e c591 391a 808c 470a 3697 53a2 9b9a  0n..9...G.6.S...
+00000130: fb3e 05cb d333 1d20 5afc b007 0225 e506  .>...3. Z....%..
+00000140: 02b1 7596 2dcc c022 ae44 d1d4 0e0d 26b2  ..u.-..".D....&.
+00000150: dca7 33de e18a 8f9f a95d 600e 815a 0ad4  ..3......]`..Z..
+00000160: 7186 aaac 4034 f3c4 781a db1a ae80 19c6  q...@4..x.......
+00000170: 9442 fe2e 905b 894b f54f ecd2 0171 4e8e  .B...[.K.O...qN.
+00000180: d9af a961 18ca 412f b969 870a de9e 1e5f  ...a..A/.i....._
+00000190: 9675 0bdf 65b6 1dd2 f42b 7bc3 a748 5b71  .u..e....+{..H[q
+000001a0: 99fc aaef ee77 0fa2 5152 e942 ea42 e99d  .....w..QR.B.B..
+000001b0: dc18 756b a47c 9f5d 7ff8 5d85 43ef fcde  ..uk.|.]..].C...
+000001c0: ff63 e38b 6053 c3af bb68 be00 504b 0304  .c..`S...h..PK..
+000001d0: 1400 0000 0800 803b 7756 995c 9c23 1006  .......;wV.\.#..
+000001e0: 0000 9c27 0000 1300 0000 786c 2f74 6865  ...'......xl/the
+000001f0: 6d65 2f74 6865 6d65 312e 786d 6ced 5a5b  me/theme1.xml.Z[
+00000200: 73da 3814 7eef afd0 7867 f66d 0bc6 3681  s.8.~...xg.m..6.
+00000210: b6b4 1373 6976 dbb4 9984 ed4e 1f85 1158  ...siv.....N...X
+00000220: 8d6c 7964 9184 7fbf 4736 10cb 960d ed92  .lyd....G6......
+00000230: 4dba 9b3c 042c e9fb ce45 47e7 e838 79f3  M..<.,...EG..8y.
+00000240: ee2e 62e8 8688 94f2 7860 d92f dbd6 bbb7  ..b.....x`./....
+00000250: 2fde e057 3224 1141 3019 a7af f0c0 0aa5  /..W2$.A0.......
+00000260: 4c5e b55a 6900 c338 7dc9 1312 c3dc 828b  L^.Zi..8}.......
+00000270: 084b 7814 cbd6 5ce0 5b1a 2f23 d6ea b4db  .Kx...\.[./#....
+00000280: dd56 8469 6ca1 1847 6460 7d5e 2c68 40d0  .V.il..Gd`}^,h@.
+00000290: 5451 5a6f 5f20 b4e5 1f33 f815 cb54 8d65  TQZo_ ...3...T.e
+000002a0: a301 1357 4126 b988 b4f2 f96c c5fc dade  ...WA&.....l....
+000002b0: 3e65 cfe9 3a1d 3281 6e30 1b58 207f ce6f  >e..:.2.n0.X ..o
+000002c0: a7e4 4e5a 88e1 54c2 c4c0 6a67 3f56 6bc7  ..NZ..T...jg?Vk.
+000002d0: d1d2 4880 82c9 7d94 05ba 49f6 a3d3 1508  ..H...}...I.....
+000002e0: 320d 3b3a 9d58 ce76 7cf6 c4ed 9f8c cada  2.;:.X.v|.......
+000002f0: 7434 6d1a e0e3 f178 38b6 cbd2 8b70 1c04  t4m....x8....p..
+00000300: e051 bb9e c29d f46c bfa4 4109 b4a3 69d0  .Q.....l..A...i.
+00000310: 64d8 f6da ae91 a6aa 8d53 4fd3 f77d dfeb  d........SO..}..
+00000320: 9b68 9c0a 8d5b 4fd3 6b77 ddd3 8e89 c6ad  .h...[O.kw......
+00000330: d078 0dbe f14f 87c3 ae89 c6ab d074 eb69  .x...O.......t.i
+00000340: 2627 fdae 6ba4 e916 6842 46e3 eb7a 1215  &'..k...hBF..z..
+00000350: b5e5 40d3 2000 5870 76d6 ccd2 0396 5e29  ..@. .Xpv.....^)
+00000360: fa75 941a d91d bbdd 415c f058 ee39 8911  .u......A\.X.9..
+00000370: fec6 c504 d669 d219 9634 4672 9d90 050e  .....i...4Fr....
+00000380: 0037 c4d1 4c50 7caf 41b6 8ae0 c292 d25c  .7..LP|.A......\
+00000390: 90d6 cf29 b550 1a08 9ac8 81f5 4782 21c5  ...).P......G.!.
+000003a0: dcaf fdf5 97bb c9a4 337a 9d7d 3ace 6b94  ........3z.}:.k.
+000003b0: 7f69 ab01 a7ed bb9b cf93 fc73 e8e4 9fa7  .i.........s....
+000003c0: 93d7 4d42 ce70 bc2c 09f1 fb23 5b61 8727  ..MB.p.,...#[a.'
+000003d0: 6e3b 1372 3a1c 6742 7ccf f6f6 91a5 2532  n;.r:.gB|.....%2
+000003e0: cfef f90a eb4e 3c67 1f56 96b0 5dcf cfe4  .....N<g.V..]...
+000003f0: 9e8c 7223 bbdd f658 7df6 4f47 6e23 d7a9  ..r#...X}.OGn#..
+00000400: c0b3 22d7 9446 2445 9fc8 2dba e411 38b5  .."..F$E..-...8.
+00000410: 490d 3213 3f08 9d86 986a 501c 02a4 0931  I.2.?....jP....1
+00000420: 96a1 86f8 b4c6 ac11 e013 7db7 be08 c8df  ..........}.....
+00000430: 8d88 f7ab 6f9a 3d57 a158 49da 84f8 1046  ....o.=W.XI....F
+00000440: 1ae2 9c73 e673 d16c fb07 a546 d1f6 55bc  ...s.s.l...F..U.
+00000450: dca3 9758 1501 9718 df34 aa35 2cc5 d678  ...X.....4.5,..x
+00000460: 95c0 f1ad 9c3c 1d13 12cd 940b 0641 8697  .....<.......A..
+00000470: 2426 12a9 397e 4d48 13fe 2ba5 dafe 9cd3  $&..9~MH..+.....
+00000480: 40f0 942f 24fa 4a91 8f69 b323 a774 26cd  @../$.J..i.#.t&.
+00000490: e833 1ac1 46af 1b75 8768 d23c 7afe 05f9  .3..F..u.h.<z...
+000004a0: 9c35 0a1c 911b 1d02 671b b346 2184 69bb  .5......g..F!.i.
+000004b0: f01e af24 8e9a adc2 112b 423e 6219 361a  ...$.....+B>b.6.
+000004c0: 72b5 1681 b671 a984 605a 12c6 d178 4ed2  r....q..`Z...xN.
+000004d0: b411 fc59 ac35 933e 60c8 eccd 9175 ced6  ...Y.5.>`....u..
+000004e0: 910e 1192 5e37 423e 62ce 8b90 11bf 1e86  ....^7B>b.......
+000004f0: 384a 9aed a271 5804 fd9e 5ec3 49c1 e882  8J...qX...^.I...
+00000500: cb66 fdb8 7e86 d533 6c2c 8ef7 47d4 174a  .f..~..3l,..G..J
+00000510: e40f 26a7 3fe9 3234 07a3 9a59 09bd 8456  ..&.?.24...Y...V
+00000520: 6a9f aa87 343e a81e 320a 05f1 b91e 3ee5  j...4>..2.....>.
+00000530: 7a78 0a37 96c6 bc50 ae82 7b01 ffd1 da37  zx.7...P..{....7
+00000540: c2ab f882 c039 7f2e 7dcf a5ef b9f4 3da1  .....9..}.....=.
+00000550: d2b7 3723 7d67 c1d3 8b5b de46 6e5b c4fb  ..7#}g...[.Fn[..
+00000560: ae31 dad7 342e 2863 5772 cdc8 c754 af93  .1..4.(cWr...T..
+00000570: 29d8 399f c0ec fd68 3e9e f1ed fad9 2484  ).9....h>.....$.
+00000580: af9a 592d 2316 904b 81b3 4124 b8fc 8bca  ..Y-#..K..A$....
+00000590: f02a c409 e864 5b25 09cb 54d3 6537 8a12  .*...d[%..T.e7..
+000005a0: 9e42 1b6e e953 f54a 95d7 e5af b928 b83c  .B.n.S.J.....(.<
+000005b0: 5be4 e9af a174 3e2c cff9 3c5f e7b4 cd0b  [....t>,..<_....
+000005c0: 3343 b772 4bea b694 beb5 2638 4af4 b1cc  3C.rK.....&8J...
+000005d0: 704e 1ecb 0c3b 673c 921d b677 a01d 35fb  pN...;g<...w..5.
+000005e0: f65d 76e4 23a5 3053 9743 b81a 42be 036d  .]v.#.0S.C..B..m
+000005f0: ba9d dc3a 389e 9891 b90a d352 906f c3f9  ...:8......R.o..
+00000600: e9c5 781a e239 d904 b97d 9857 6de7 d8d1  ..x..9...}.Wm...
+00000610: d1fb e7c1 51b0 a3ef 3c96 1dc7 88f2 a221  ....Q...<......!
+00000620: eea1 8698 cfc3 4387 797b 5f98 6795 c650  ......C.y{_.g..P
+00000630: 3414 6d6c ac24 2c46 b760 b8d7 f12c 14e0  4.ml.$,F.`...,..
+00000640: 6460 2da0 0783 af51 02f2 5255 6031 5bc6  d`-....Q..RU`1[.
+00000650: 032b 90a2 7c4c 8c45 e870 e797 5c5f e3d1  .+..|L.E.p..\_..
+00000660: 92e3 dba6 65b5 6eaf 2977 196d 2252 39c2  ....e.n.)w.m"R9.
+00000670: 6998 1367 abca de65 b1c1 551d cf55 5bf2  i..g...e..U..U[.
+00000680: b0be 6a3d b415 4ecf fe59 adc8 9f0c 114e  ..j=..N..Y.....N
+00000690: 160b 1248 6394 17a6 4aa2 f319 53be e72b  ...Hc...J...S..+
+000006a0: 49c4 5538 bf45 33b6 1297 18bc e3e6 c771  I.U8.E3........q
+000006b0: 4e53 b812 76b6 0f02 32b9 bb39 a97a 6531  NS..v...2..9.ze1
+000006c0: 67a6 f2df 2d0c 092c 5b88 5912 e24d 5ded  g...-..,[.Y..M].
+000006d0: d5e7 9b9c ae7a 2276 fa97 77c1 60f2 fd70  .....z"v..w.`..p
+000006e0: c947 0fe5 3be7 5ff4 5d43 ae7e f6dd e3fa  .G..;._.]C.~....
+000006f0: 6e93 3b48 4c9c 79c5 1101 7445 0223 951c  n.;HL.y...tE.#..
+00000700: 0616 1732 e450 ee92 9006 1301 cd94 c944  ...2.P.........D
+00000710: f002 8264 a61c 8098 fa0b bdf2 0cb9 2915  ...d..........).
+00000720: cead 3e39 7f45 2c83 864e 5ed2 2512 148a  ..>9.E,..N^.%...
+00000730: b00c 0521 1772 e3ef ef93 6a77 8cd7 fa2c  ...!.r....jw...,
+00000740: 816d 8454 3264 d517 ca43 89c1 3d33 7243  .m.T2d...C..=3rC
+00000750: d854 25f3 aeda 260b 85db e254 cdbb 1abe  .T%...&....T....
+00000760: 2660 4bc3 7a6e 9d2d 27ff db5e d43d b417  &`K.zn.-'..^.=..
+00000770: 3d46 f3a3 99e0 1eb3 8773 9b7a b8c2 45ac  =F.......s.z..E.
+00000780: ff58 d61e f932 df39 70db 3ade 035e e613  .X...2.9p.:..^..
+00000790: 2c43 a47e c17d 8a8a 8011 ab62 beba af4f  ,C.~.}.....b...O
+000007a0: f925 9c3b b47b f181 209b fcd6 dba4 f6dd  .%.;.{.. .......
+000007b0: e00c 7cd4 ab5a a564 2b11 3f4b 077c 1f92  ..|..Z.d+.?K.|..
+000007c0: 0663 8c5b f434 5f8f 1462 ada6 b1ad c6da  .c.[.4_..b......
+000007d0: 310c 7980 58f3 0ca1 6638 df87 459a 1a33  1.y.X...f8..E..3
+000007e0: d58b ac39 8d0a 6f41 d540 e53f dbd4 0d68  ...9..oA.@.?...h
+000007f0: f60d 341c 9105 5e31 99b6 36a3 e44e 0a3c  ..4...^1..6..N.<
+00000800: dcfe ef0d b0c2 c48e e1ed 8bbf 0150 4b03  .............PK.
+00000810: 0414 0000 0008 0080 3b77 5685 36ce 1a64  ........;wV.6..d
+00000820: 0100 00f9 0200 0018 0000 0078 6c2f 776f  ...........xl/wo
+00000830: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
+00000840: 786d 6c75 92c1 6ec2 300c 865f 25ca 0310  xmlu..n.0.._%...
+00000850: 98c4 36a1 b6d2 80a1 ed30 0981 b61d a7d0  ..6......0......
+00000860: ba34 2289 bbc4 ace3 ed97 14a8 98d4 9e62  .4"............b
+00000870: 3b9f 7fc7 8e93 06dd c157 00c4 7e8d b63e  ;........W..~..>
+00000880: e515 513d 13c2 e715 18e9 4758 830d 3725  ..Q=......GX..7%
+00000890: 3a23 29b8 6e2f 7ced 4016 6d92 d1e2 6e3c  :#).n/|.@.m...n<
+000008a0: be17 462a cbb3 a48d ad5d 96e0 91b4 b2b0  ..F*.....]......
+000008b0: 76cc 1f8d 91ee 3407 8d4d ca27 fc1a d8a8  v.....4..M.'....
+000008c0: 7d45 3120 b2a4 967b d802 bdd7 6b17 3cd1  }E1 ...{....k.<.
+000008d0: a914 ca80 f50a 2d73 50a6 fc69 325b b57c  ......-sP..i2[.|
+000008e0: 0b7c 2868 fc8d cd62 273b c443 745e 8b94  .|(h...b';.Ct^..
+000008f0: 8fe3 8340 434e 5141 86e3 0716 a075 140a  ...@CNQA.....u..
+00000900: cff8 be68 f2ae 644c bcb5 afea abb6 f7d0  ...h..dL........
+00000910: cb4e 7a58 a0fe 5405 5529 7fe4 ac80 521e  .NzX..T.U)....R.
+00000920: 356d b079 814b 3fd3 ee81 4b49 324b 1c36  5m.y.K?...KI2K.6
+00000930: ccc5 3eb3 248f 46ac 1d38 65e3 7cb6 e442  ..>.$.F..8e.|..B
+00000940: 5c85 4294 1de0 9408 0af5 a32b f20b 3e1f  \.B........+..>.
+00000950: c22d f6d0 8b21 3afc 98ff 5245 4fca 7228  .-...!:...REO.r(
+00000960: a501 38f4 f0cf 437c 013d f46a 8806 fb9f  ..8...C|.=.j....
+00000970: 1661 4ed7 d99f 0717 97e2 4dba bdb2 9e69  .aN.......M....i
+00000980: 2883 ca78 f430 e5cc 9d07 7d76 08eb 76a9  (..x.0....}v..v.
+00000990: 7648 84a6 35ab b09b e022 10ee 4b44 ba3a  vH..5...."..KD.:
+000009a0: f19f bb6d cffe 0050 4b03 0414 0000 0008  ...m...PK.......
+000009b0: 0080 3b77 56dc 634f f272 0100 0035 0300  ..;wV.cO.r...5..
+000009c0: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+000009d0: 7473 2f73 6865 6574 322e 786d 6c75 53db  ts/sheet2.xmluS.
+000009e0: 6ec2 300c fd95 2a1f 4060 12db 84da 4a03  n.0...*.@`....J.
+000009f0: 06db c324 04da f638 a5ad db46 2471 9798  ...$...8...F$q..
+00000a00: 75fc fd92 7211 9ada a7fa 38e7 1cdb 891b  u...r.....8.....
+00000a10: b768 f7ae 06a0 e857 2be3 1256 1335 33ce  .h.....W+..V.53.
+00000a20: 5d5e 8316 6e84 0d18 7f52 a2d5 823c b415  ]^..n....R...<..
+00000a30: 778d 0551 7422 adf8 dd78 7ccf b590 86a5  w..Qt"...x|.....
+00000a40: 7197 dbd8 34c6 0329 6960 6323 77d0 5ad8  q...4..)i`c#w.Z.
+00000a50: e31c 14b6 099b b04b 622b ab9a 4282 a771  .......Kb+..B..q
+00000a60: 232a d801 bd37 1beb 11bf ba14 5283 7112  #*...7......R.q.
+00000a70: 4d64 a14c d8d3 64b6 eef8 1de1 4342 eb6e  Md.L..d.....CB.n
+00000a80: e228 4c92 21ee 0378 2d12 360e 0d81 829c  .(L.!..x-.6.....
+00000a90: 8283 f09f 1f58 8052 c1c8 b7f1 7df6 64d7  .....X.R....}.d.
+00000aa0: 9241 781b 5fdc 57dd ec7e 964c 3858 a0fa  .Ax._.W..~.L8X..
+00000ab0: 9405 d509 7b64 5101 a538 28da 62fb 02e7  ....{dQ..8(.b...
+00000ac0: 79a6 d706 9782 441a 5b6c 231b e64c e33c  y.....D.[l#..L.<
+00000ad0: 04a1 b6e7 4913 ee67 47d6 e7a5 2f44 e91e  ....I..gG.../D..
+00000ae0: 8e31 275f 3f40 9e9f e9f3 21ba 39e8 1efa  .1'_?@....!.9...
+00000af0: 6290 2e34 f4f0 9743 fca6 a1af 52aa 3ecd  b..4...C....R.>.
+00000b00: f390 c6e5 1232 ec51 ac86 1495 2425 b21e  .....2.Q....$%..
+00000b10: c57a 48a1 118b ff5d 717f c797 773b 5d7a  .zH....]q...w;]z
+00000b20: 58a8 3761 2b69 5ca4 a0f4 4ee3 d1c3 9445  X.7a+i\...N....E
+00000b30: f6f4 4827 40d8 740b 9921 11ea 2eac fd5e  ..H'@.t..!.....^
+00000b40: 830d 047f 5e22 d205 841d b9fe 29e9 1f50  ....^"......)..P
+00000b50: 4b03 0414 0000 0008 0080 3b77 56db d46f  K.........;wV..o
+00000b60: e18e 0100 000d 0400 0018 0000 0078 6c2f  .............xl/
+00000b70: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00000b80: 332e 786d 6c85 54db 4ec3 300c fd95 2a1f  3.xml.T.N.0...*.
+00000b90: b00c 242e 426d 2536 1883 0969 da04 3c67  ..$.Bm%6...i..<g
+00000ba0: adbb 46cb a538 2e85 bf27 e9b6 6a48 2d7b  ..F..8...'..jH-{
+00000bb0: aaed 9ce3 63b7 278d 1b8b 3b57 0250 f4ad  ....c.'...;W.P..
+00000bc0: 9571 092b 89aa 3bce 5d56 8216 6e64 2b30  .q.+..;.]V..nd+0
+00000bd0: fea4 b0a8 05f9 14b7 dc55 0822 6f49 5af1  .........U."oIZ.
+00000be0: cbf1 f89a 6b21 0d4b e3b6 b6c4 34b6 3529  ....k!.K....4.5)
+00000bf0: 6960 8991 abb5 16f8 3301 659b 845d b063  i`......3.e..].c
+00000c00: 6125 b725 8502 4fe3 4a6c 610d f456 2dd1  a%.%..O.Jla..V-.
+00000c10: 67bc eb92 4b0d c649 6b22 8422 61f7 1777  g...K..Ik"."a..w
+00000c20: 8b16 df02 de25 34ee 248e c226 1b6b 7721  .....%4.$..&.kw!
+00000c30: 79ce 1336 0e03 8182 8c42 07e1 1f5f 3005  y..6.....B..._0.
+00000c40: a542 233f c6e7 a127 eb24 03f1 343e 769f  .B#?...'.$..4>v.
+00000c50: b5bb fb5d 36c2 c1d4 aa0f 9953 99b0 5b16  ...]6......S..[.
+00000c60: e550 885a d1ca 3673 38ec 73d5 0df8 2048  .P.Z..6s8.s... H
+00000c70: a431 da26 c2b0 671a 6721 08da 1e27 4d78  .1.&..g.g!...'Mx
+00000c80: 3f6b 425f 975e 88d2 1dfc c49c bc7e 4879  ?kB_.^.......~Hy
+00000c90: 7680 4f86 e09f 8b5e fc74 082f f31e f4c3  v.O....^.t./....
+00000ca0: 103a 2b45 4580 3d94 c733 94fe b166 432c  .:+EE.=..3...fC,
+00000cb0: 576f a683 5a4f e759 fd72 f321 227a 3f7c  Wo..ZO.Y.r.!"z?|
+00000cc0: 0993 410f e9f9 9f2f e3bd 95bb 1ece cbe0  ..A..../........
+00000cd0: 84b2 5f64 3144 a80d 49f5 97c0 bd77 8e7e  .._d1D..I....w.~
+00000ce0: dc9b 295c 9457 815b 695c a4a0 f08d c6a3  ..)\.W.[i\......
+00000cf0: 9b2b 16e1 de7c fb84 6cd5 5eb4 8d25 b2ba  .+...|..l.^..%..
+00000d00: 0d4b 7f5f 0103 c09f 17d6 d231 09de effe  .K._.......1....
+00000d10: 00e9 2f50 4b03 0414 0000 0008 0080 3b77  ../PK.........;w
+00000d20: 5623 2837 0d8c 0100 00a5 0300 0018 0000  V#(7............
+00000d30: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00000d40: 6865 6574 342e 786d 6c75 535d 6f9d 300c  heet4.xmluS]o.0.
+00000d50: fd2b 283f a0b9 9dd4 75aa 0069 bd6d d7fb  .+(?....u..i.m..
+00000d60: 30e9 aad5 b6c7 2917 0c44 2431 734c 59ff  0.....)..D$1sLY.
+00000d70: fd1c ee87 3a09 9ef0 71ce b17d 8893 4f48  ....:...q..}..OH
+00000d80: 7dec 0038 fbeb 5d88 85ea 9887 3bad 63d5  }..8..].....;.c.
+00000d90: 8137 f10a 0708 72d2 2079 c302 a9d5 7120  .7....r. y....q 
+00000da0: 30f5 2cf2 4e7f da6c 3e6b 6f6c 5065 3ee7  0.,.N..l>kolPe>.
+00000db0: f654 e638 b2b3 01f6 94c5 d17b 43ef f7e0  .T.8.......{C...
+00000dc0: 702a d4b5 3a27 5e6c db71 4ae8 321f 4c0b  p*..:'^l.qJ.2.L.
+00000dd0: afc0 3f86 3d09 d297 2ab5 f510 a2c5 9011  ..?.=...*.......
+00000de0: 3485 fa7a 7db7 9bf9 33e1 a785 297e 88b3  4..z}...3...)~..
+00000df0: e4e4 80d8 27b0 ab0b b549 0381 838a 5305  ....'....I....S.
+00000e00: 239f 37d8 8273 a990 8cf1 e754 535d 5a26  #.7..s.....TS]Z&
+00000e10: e1c7 f85c fd69 f62e 5e0e 26c2 16dd 2f5b  ...\.i..^.&.../[
+00000e20: 7357 a82f 2aab a131 a3e3 179c 9ee1 e4e7  sW./*..1........
+00000e30: e632 e083 6153 e684 5346 c967 9957 2948  .2..aS..SF.g.W)H
+00000e40: bd85 6743 fa3f af4c 92b7 d288 cb1e de73  ..gC.?.L.......s
+00000e50: cdd2 3f41 5d9d e8f7 6b74 e3ac 4c13 1724  ..?A]...kt..L..$
+00000e60: db35 490d 0bec 8735 3684 05f6 e31a 7bb2  .5I....56.....{.
+00000e70: bdad c5b0 ad17 544f 6b2a c1fd 9285 6feb  ......TOk*....o.
+00000e80: 0206 323c d292 95e7 35d5 486e a9cb 6e8d  ..2<....5.Hn..n.
+00000e90: 1fd9 543d be01 35b2 b4bf d9b4 ff8b b5dc  ..T=..5.........
+00000ea0: e979 4f8e 979c 16f8 bba1 d686 9839 68a4  .yO..........9h.
+00000eb0: e8e6 eaf6 4665 745c 8a23 601c e607 7040  ....Fet\.#`...p@
+00000ec0: 66f4 73d8 c93b 024a 0439 6f10 f90c d24e  f.s..;.J.9o....N
+00000ed0: 5e5e 66f9 0f50 4b03 0414 0000 0008 0080  ^^f..PK.........
+00000ee0: 3b77 5613 346b 2f8b 0100 00d5 0300 0018  ;wV.4k/.........
+00000ef0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00000f00: 2f73 6865 6574 352e 786d 6c75 53db 6ae4  /sheet5.xmluS.j.
+00000f10: 300c fd95 e00f a8a7 0bbd 5092 403b bdc3  0.........P.@;..
+00000f20: c2d0 b2bb cf9e 8992 98b1 ad54 d634 dbbf  ...........T.4..
+00000f30: 5f39 73a1 0bf1 5374 e473 8e24 472e 47a4  _9s...St.s.$G.G.
+00000f40: 6dec 01b8 f8eb 5d88 95ea 9987 1bad e3a6  m.....].........
+00000f50: 076f e219 0e10 e4a4 45f2 8605 52a7 e340  .o......E...R..@
+00000f60: 609a 49e4 9dfe b158 5c6a 6f6c 5075 39e5  `.I....X\jolPu9.
+00000f70: 5654 97b8 6367 03ac a888 3bef 0d7d dd81  VT..cg....;..}..
+00000f80: c3b1 52e7 ea98 78b3 5dcf 29a1 eb72 301d  ..R...x.].)..r0.
+00000f90: bc03 ff1a 5624 489f 5c1a eb21 448b a120  ....V$H.\..!D.. 
+00000fa0: 682b 757b 7ef3 3af1 27c2 6f0b 63fc 1617  h+u{~.:.'.o.c...
+00000fb0: 6992 35e2 3681 97a6 528b d410 38d8 7072  i.5.6...R...8.pr
+00000fc0: 30f2 f984 2538 978c a48d 8f83 a73a 954c  0...%8.......:.L
+00000fd0: c2ef f1d1 fd71 9a5d 6659 9b08 4b74 7f6c  .....q.]fY..Kt.l
+00000fe0: c37d a5ae 55d1 406b 768e df70 7c86 c33c  .}..U.@kv..p|..<
+00000ff0: 17a7 06ef 0d9b ba24 1c0b 4a73 d6e5 2605  .......$..Js..&.
+00001000: a9b6 f06c 48f7 f3ce 2479 2b85 b8fe d8c2  ...lH...$y+.....
+00001010: 57a9 591a 4858 6f0e fcbb 1c7f 98e7 2f73  W.Y.HXo......./s
+00001020: fcd4 7c30 1e66 34f7 d91a f263 66f8 0f39  ..|0.f4....cf..9
+00001030: 7ec6 ff31 c767 cb6e 4ef0 9413 c8cc f29b  ~..1.g.nN.......
+00001040: 9b38 a379 ce69 046f e704 2f79 0103 19de  .8.y.i.o../y....
+00001050: d15c 6baf 5915 180a 3674 4f68 dcff 3a2d  .\k.Y...6tOh..:-
+00001060: 3b70 dcab fd52 a47b fd69 a8b3 2116 0e5a  ;p...R.{.i..!..Z
+00001070: f15b 9c5d 5da8 82f6 4bb4 078c c3f4 60d6  .[.]]...K.....`.
+00001080: c88c 7e0a 7b79 7740 8920 e72d 221f 41da  ..~.{yw@. .-".A.
+00001090: e1d3 4bae ff01 504b 0304 1400 0000 0800  ..K...PK........
+000010a0: 803b 7756 e637 718b 7e01 0000 9303 0000  .;wV.7q.~.......
+000010b0: 1800 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+000010c0: 732f 7368 6565 7436 2e78 6d6c 7553 d16e  s/sheet6.xmluS.n
+000010d0: c230 0cfc 952a 1f40 6012 db84 da4a 03c6  .0...*.@`....J..
+000010e0: 40d3 2404 daf6 1c5a 9746 2471 49cc 3afe  @.$....Z.F$qI.:.
+000010f0: 7e49 a188 49ed 537d cedd d96e 9cb8 467b  ~I..I.S}...n..F{
+00001100: 7025 0045 bf5a 1997 b092 a89a 70ee b212  p%.E.Z......p...
+00001110: b470 03ac c0f8 9302 ad16 e4a1 dd73 5759  .p...........sWY
+00001120: 1079 23d2 8a3f 0c87 8f5c 0b69 581a 37b9  .y#..?...\.iX.7.
+00001130: b54d 633c 9192 06d6 3672 27ad 853d 4f41  .Mc<....6r'..=OA
+00001140: 619d b011 6b13 1bb9 2f29 2478 1a57 620f  a...k.../)$x.Wb.
+00001150: 5ba0 cf6a 6d3d e237 975c 6a30 4ea2 892c  [..jm=.7.\j0N..,
+00001160: 1409 7b19 4d56 0dbf 217c 49a8 dd5d 1c85  ..{.MV..!|I..]..
+00001170: 4976 8887 0056 79c2 86a1 2150 9051 7010  Iv...Vy...!P.Qp.
+00001180: fef3 0333 502a 18f9 368e 574f 762b 1984  ...3P*..6.WOv+..
+00001190: f771 ebbe 6866 f7b3 ec84 8319 aa6f 9953  .q..hf.......o.S
+000011a0: 99b0 6716 e550 8893 a20d d64b b8ce 33be  ..g..P.....K..3.
+000011b0: 3538 1724 d2d8 621d d930 671a 6721 08b5  58.$..b..0g.g!..
+000011c0: 3d4f 9af0 7fb6 647d 5efa 4294 1edf e11c  =O....d}^.B.....
+000011d0: 73f2 0d04 ccb3 2b7f dac7 3f74 d267 7df4  s.....+...?t.g}.
+000011e0: 0c4d 0615 7548 e67d 1227 bda4 43f0 da5b  .M..uH.}.'..C..[
+000011f0: a384 ecd0 2158 f409 2a8b 3b05 ba43 f2d6  ....!X..*.;..C..
+00001200: 27c1 ae02 cb3e 3621 09d5 2158 f576 e417  '....>6!..!X.v..
+00001210: f93f 9ffb 1b6c b7e2 72a5 615d 3f84 dd4b  .?...l..r.a]?..K
+00001220: e322 0585 f719 0e9e c62c b297 15b8 00c2  .".......,......
+00001230: aa59 f71d 12a1 6ec2 d2bf 1ab0 81e0 cf0b  .Y....n.........
+00001240: 446a 41d8 c0db 3b4c ff00 504b 0304 1400  DjA...;L..PK....
+00001250: 0000 0800 803b 7756 aca9 9829 4d01 0000  .....;wV...)M...
+00001260: 6d02 0000 1800 0000 786c 2f77 6f72 6b73  m.......xl/works
+00001270: 6865 6574 732f 7368 6565 7437 2e78 6d6c  heets/sheet7.xml
+00001280: 7552 d14e c330 0cfc 9528 1fb0 7448 0334  uR.N.0...(..tH.4
+00001290: b595 5811 8207 a469 13f0 9cb5 6e1b 2d89  ..X....i....n.-.
+000012a0: 4be2 d1f1 f724 dd5a 0d69 7b8a cf39 9f7d  K....$.Z.i{..9.}
+000012b0: 71d2 1edd deb7 00c4 8e46 5b9f f196 a85b  q........F[....[
+000012c0: 0ae1 cb16 8cf4 33ec c086 9b1a 9d91 14a0  ......3.........
+000012d0: 6b84 ef1c c86a 2832 5adc 25c9 bd30 5259  k....j(2Z.%..0RY
+000012e0: 9ea7 436e edf2 140f a495 85b5 63fe 608c  ..Cn........c.`.
+000012f0: 74bf 2bd0 d867 7cce c7c4 4635 2dc5 84c8  t.+..g|...F5-...
+00001300: d34e 36b0 05fa e8d6 2e20 31a9 54ca 80f5  .N6...... 1.T...
+00001310: 0a2d 7350 67fc 69be 2c06 fe40 f854 d0fb  .-sPg.i.,..@.T..
+00001320: 8b98 4527 3bc4 7d04 6f55 c693 3810 6828  ..E';.}.oU..8.h(
+00001330: 292a c870 fc40 015a 47a1 30c6 f759 934f  )*.p.@.ZG.0..Y.O
+00001340: 2d63 e165 3caa bf0c de83 979d f450 a0fe  -c.e<........P..
+00001350: 5215 b519 7fe4 ac82 5a1e 346d b07f 85b3  R.......Z.4m....
+00001360: 9fc5 34e0 b324 99a7 0e7b e6a2 cf3c 2d63  ..4..$...{...<-c
+00001370: 107b 079e b2f1 7db6 e442 5e85 4694 2b02  .{....}..B^.F.+.
+00001380: 930a 0a03 442c ca33 7f75 8b1f f653 eeaf  ....D,.3.u...S..
+00001390: 1414 b70a 6a75 fc4f 1761 b6d1 ef69 d8b8  ....ju.O.a...i..
+000013a0: 8877 e91a 653d d350 0799 64f6 b0e0 cc9d  .w..e=.P..d.....
+000013b0: cc9d 0061 372c 7287 4468 86b0 0dff 015c  ...a7,r.Dh.....\
+000013c0: 2484 fb1a 9146 10df 76fa 61f9 1f50 4b03  $....F..v.a..PK.
+000013d0: 0414 0000 0008 0080 3b77 56aa 5da3 295a  ........;wV.].)Z
+000013e0: 0100 00b0 0200 0018 0000 0078 6c2f 776f  ...........xl/wo
+000013f0: 726b 7368 6565 7473 2f73 6865 6574 382e  rksheets/sheet8.
+00001400: 786d 6c75 52db 4ec3 300c fd95 281f b074  xmluR.N.0...(..t
+00001410: 4803 34b5 95d8 2604 0f48 d326 e039 6bdd  H.4...&..H.&.9k.
+00001420: 365a 2e25 f1e8 f87b e26e ad26 419f e2e3  6Z.%...{.n.&A...
+00001430: f81c fb38 493b e78f a101 4076 36da 868c  ...8I;....@v6...
+00001440: 3788 ed52 8850 3460 6498 b916 6cbc a99c  7..R.P4`d...l...
+00001450: 3712 23f4 b508 ad07 59f6 24a3 c55d 92dc  7.#.....Y.$..]..
+00001460: 0b23 95e5 79da e7b6 3e4f dd09 b5b2 b0f5  .#..y...>O......
+00001470: 2c9c 8c91 fe67 05da 7519 9ff3 21b1 5375  ,....g..u...!.Su
+00001480: 8394 1079 daca 1af6 80ef edd6 4724 4695  ...y........G$F.
+00001490: 5219 b041 39cb 3c54 197f 9a2f 377d 7d5f  R..A9.<T.../7}}_
+000014a0: f0a1 a00b 3731 2327 07e7 8e04 5ecb 8c27  ....71#'....^..'
+000014b0: 3410 6828 9014 643c be61 0d5a 9350 1ce3  4.h(..d<.a.Z.P..
+000014c0: ebaa c9c7 9644 bc8d 07f5 e7de 7bf4 7290  .....D......{.r.
+000014d0: 01d6 4e7f aa12 9b8c 3f72 5642 254f 1a77  ..N.....?rVB%O.w
+000014e0: ae7b 81ab 9fc5 38e0 46a2 cc53 ef3a e6c9  .{....8.F..S.:..
+000014f0: 679e 1614 50ef 58a7 2ced 678f 3ee6 556c  g...P.X.,.g.>.Ul
+00001500: 84b9 2a53 81b1 3d21 515c ab57 53d5 706e  ..*S..=!Q\.WS.pn
+00001510: a331 49d6 fea1 ada7 69d2 283b 45db 4cd1  .1I.....i.(;E.L.
+00001520: 4a08 8557 ed5f 9a88 f686 955d fcd2 5bbe  J..W._.....]..[.
+00001530: 495f 2b1b 9886 2aca 25b3 8705 67fe b29f  I_+...*.%...g...
+00001540: 0b40 d7f6 7fe1 e010 9de9 c326 7e29 f054  .@.........&~).T
+00001550: 10ef 2be7 7000 f43c e327 cd7f 0150 4b03  ..+.p..<.'...PK.
+00001560: 0414 0000 0008 0080 3b77 56ca 3cde 0882  ........;wV.<...
+00001570: 0100 009b 0300 0018 0000 0078 6c2f 776f  ...........xl/wo
+00001580: 726b 7368 6565 7473 2f73 6865 6574 392e  rksheets/sheet9.
+00001590: 786d 6c75 53db 4ec3 300c fd95 2a1f 4006  xmluS.N.0...*.@.
+000015a0: 1217 a1b6 128c cbf6 8034 8180 e774 71d7  .........4...tq.
+000015b0: 6849 5c1c 97c2 df93 7417 0da9 7daa ed9c  hI\.....t...}...
+000015c0: 8b9d b879 8fb4 0d0d 0067 3fce fa50 8886  ...y.....g?..P..
+000015d0: b9bd 9532 ac1b 702a 9c61 0b3e 9ed4 484e  ...2..p*.a.>..HN
+000015e0: 714c 6923 434b a0f4 4072 565e cc66 57d2  qLi#CK..@rV^.fW.
+000015f0: 29e3 4599 0fb5 1595 3976 6c8d 8715 65a1  ).E.....9vl...e.
+00001600: 734e d1ef 3d58 ec0b 712e 0e85 57b3 6938  sN..=X..q...W.i8
+00001610: 1564 99b7 6a03 6fc0 efed 8a62 268f 2ada  .d..j.o....b&.*.
+00001620: 38f0 c1a0 cf08 ea42 dc9d df2e 07fc 00f8  8......B........
+00001630: 30d0 8793 384b 9354 88db 942c 7521 66a9  0...8K.T...,u!f.
+00001640: 21b0 b0e6 a4a0 e2e7 1be6 606d 128a 6d7c  !.........`m..m|
+00001650: ed35 c5d1 3211 4fe3 83fa d330 7b9c a552  .5..2.O....0{..R
+00001660: 01e6 683f 8de6 a610 3722 d350 abce f22b  ..h?....7".P...+
+00001670: f60b d8cf 7379 6cf0 41b1 2a73 c23e a334  ....syl.A.*s.>.4
+00001680: 6799 af53 90bc 23ce f874 3f6f 4cb1 6ea2  g..S..#..t?oL.n.
+00001690: 1197 46e7 92a3 7dca e47a 8fbe 9f42 6b34  ..F...}..z...Bk4
+000016a0: 23f0 f914 bc37 5ba3 633f a326 0f93 2d85  #....7[.c?.&..-.
+000016b0: ca8f e01f a7f0 6cd8 c208 e169 8aa0 3a6e  ......l....i..:n
+000016c0: 90c2 08e5 798a d276 9535 f17e 6984 b498  ....y..v.5.~i...
+000016d0: 22fd 821a c32f 274d 74fd 4ef6 3f43 c697  "..../'Mt.N.?C..
+000016e0: 3c6c c7ee 69d3 dabe 28da 181f 320b 7554  <l..i...(...2.uT
+000016f0: 9a9d 5d5f 8a8c 76ab b04b 18db 61ed 2b64  ..]_..v..K..a.+d
+00001700: 4637 844d fc7b 8012 209e d788 7c48 d226  F7.M.{.. ...|H.&
+00001710: 1eff c7f2 0f50 4b03 0414 0000 0008 0080  .....PK.........
+00001720: 3b77 5688 c588 ed4d 0100 006e 0200 0019  ;wV....M...n....
+00001730: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00001740: 2f73 6865 6574 3130 2e78 6d6c 7552 d14e  /sheet10.xmluR.N
+00001750: c330 0cfc 9528 1fb0 7448 0334 b595 5811  .0...(..tH.4..X.
+00001760: 8207 a469 13f0 9cb5 6e1b 2d89 4be2 52f8  ...i....n.-.K.R.
+00001770: 7b92 6ead 86c4 9ee2 b3cf 675f 9274 4077  {.n.......g_.t@w
+00001780: f42d 00b1 6fa3 adcf 784b d4ad 85f0 650b  .-..o...xK....e.
+00001790: 46fa 0576 6043 a546 6724 05e8 1ae1 3b07  F..v`C.Fg$....;.
+000017a0: b21a 9b8c 1637 4972 2b8c 5496 e7e9 98db  .....7Ir+.T.....
+000017b0: ba3c c59e b4b2 b075 ccf7 c648 f7b3 018d  .<.....u...H....
+000017c0: 43c6 977c 4aec 54d3 524c 883c ed64 037b  C..|J.T.RL.<.d.{
+000017d0: a0b7 6eeb 0212 b34a a50c 58af d032 0775  ..n....J..X..2.u
+000017e0: c61f 96eb 62e4 8f84 7705 83bf 8859 7472  ....b...w....Ytr
+000017f0: 403c 46f0 5265 3c89 0b81 8692 a282 0cc7  @<F.Re<.........
+00001800: 1714 a075 140a 6b7c 9e35 f93c 3236 5ec6  ...u..k|.5.<26^.
+00001810: 93fa d3e8 3d78 3948 0f05 ea0f 5551 9bf1  ....=x9H....UQ..
+00001820: 7bce 2aa8 65af 6987 c333 9cfd ace6 051f  {.*.e.i..3......
+00001830: 25c9 3c75 3830 177d e669 1983 383b f094  %.<u80.}.i..8;..
+00001840: 8df7 b327 17f2 2a0c a2bc 5155 2a28 cc8f  ...'..*...QU*(..
+00001850: 5094 67fa e61a bd44 5b42 47ff b414 d75a  P.g....D[BG....Z
+00001860: 7aa7 ffd2 4558 6e32 7cda 36be c4ab 748d  z...EXn2|.6...t.
+00001870: b29e 69a8 834c b2b8 5b71 e64e ee4e 80b0  ..i..L..[q.N.N..
+00001880: 1b5f f280 4468 c6b0 0d1f 025c 2484 7a8d  ._..Dh.....\$.z.
+00001890: 4813 8897 3b7f b1fc 1750 4b03 0414 0000  H...;....PK.....
+000018a0: 0008 0080 3b77 567c f3a3 dc51 0200 00f6  ....;wV|...Q....
+000018b0: 0900 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
+000018c0: 2e78 6d6c dd56 db8a db30 10fd 15e1 0fa8  .xml.V...0......
+000018d0: 9398 3571 49f2 5043 60a1 2d0b bb0f 7d55  ..5qI.PC`.-...}U
+000018e0: 6239 11e8 e2ca f292 f4eb 3b23 3976 b3ab  b9........;#9v..
+000018f0: 5928 7dab 4df0 cc1c 9db9 1b67 d3fb ab12  Y(}.M......g....
+00001900: cf67 213c bb68 65fa 6d76 f6be fb9c e7fd  .g!<.he.mv......
+00001910: f12c 34ef 3fd9 4e18 405a eb34 f7a0 ba53  .,4.?.N.@Z.4...S
+00001920: de77 4ef0 a647 9256 f96a b128 73cd a5c9  .wN..G.V.j.(s...
+00001930: 761b 33e8 bdf6 3d3b dac1 f86d b6c8 f2dd  v.3...=;...m....
+00001940: a6b5 66b6 2cb3 6880 a35c 0bf6 cad5 36ab  ..f.,.h..\....6.
+00001950: b992 0727 c359 aea5 ba46 f30a 0d47 abac  ...'.Y...F...G..
+00001960: 631e 5211 4806 4bff 2bc2 cba8 6196 a31f  c.R.H.K.+...a...
+00001970: 2d8d 7568 cc63 84f0 e8c1 a954 6a4a 6095  -.uh.c.....TjJ`.
+00001980: 45c3 6ed3 71ef 8533 7b50 0227 18df 416c  E.n.q..3{P.'..Al
+00001990: 945f ae1d 6470 72fc ba5c 3d64 3321 3c20  ._..dpr..\=d3!< 
+000019a0: c8c1 ba46 b8bb 3aa3 69b7 51a2 f540 70f2  ...F..:.i.Q..@p.
+000019b0: 74c6 a7b7 5d8e a0f7 5683 d048 7eb2 8687  t...]...V..H~...
+000019c0: 1c6e 8c51 00b7 47a1 d433 8ee8 477b e7fb  .n.Q..G..3..G{..
+000019d0: d2b2 d8eb c706 dbcc b0d4 9b08 098d 6274  ..............bt
+000019e0: 1315 f4ff a7b7 e8fb 9fdd b24e be5a ff65  ...........N.Z.e
+000019f0: 806a 4cd0 7f0e d68b 2727 5a79 09fa a5bd  .jL.....''Zy....
+00001a00: 8f3f 850e 89dc 459f ac0c 9763 9b7d c79d  .?....E....c.}..
+00001a10: 53b3 0b76 18a4 f2d2 8cda 5936 8d30 ef6a  S..v......Y6.0.j
+00001a20: 03f7 9e1f 60a9 effc c3f9 46b4 7c50 fe65  ....`.....F.|P.e
+00001a30: 02b7 d92c 7f13 8d1c 7435 9d7a c2b2 c653  ...,....t5.z...S
+00001a40: b3fc 1567 b82c a7cd 8458 d234 e222 9a7a  ...g.,...X.4.".z
+00001a50: 54dd e910 4406 0244 1d2f 24bc 45f6 e14a  T...D..D./$.E..J
+00001a60: 2314 2762 6904 312a 0e95 01c5 892c 2ace  #.'bi.1*.....,*.
+00001a70: ff54 cf9a ac27 6254 6eeb 24b2 2639 6b92  .T...'bTn.$.&9k.
+00001a80: 1359 29a4 0e37 1527 cda9 e04a 575a 5545  .Y)..7.'...JWZUE
+00001a90: 5196 5447 eb3a 9941 4df5 ad2c f197 f646  Q.TG.:.AM..,...F
+00001aa0: e586 0c2a 0e46 fabb 5ed3 d3a6 37e4 e33d  ...*.F..^...7..=
+00001ab0: a066 fad1 8650 95d2 9b48 554a f71a 9174  .f...P...HUJ...t
+00001ac0: df90 5155 e969 5371 9041 4d81 da1d 8c9f  ..QU.iSq.AM.....
+00001ad0: 8e83 3b95 e614 054e 95ca 8d7a 8369 a4aa  ..;....N...z.i..
+00001ae0: 2804 7731 bda3 6549 74a7 c43b 3d1f ea2d  (.w1..eIt..;=..-
+00001af0: 298a aa4a 2388 a533 280a 0ac1 b791 46a8  )..J#..3(.....F.
+00001b00: 0c30 070a 298a f01d 7cf3 3dca 6fdf a97c  .0..)...|.=.o..|
+00001b10: fea7 b7fb 0d50 4b03 0414 0000 0008 0080  .....PK.........
+00001b20: 3b77 5697 8abb 1cc0 0000 0013 0200 000b  ;wV.............
+00001b30: 0000 005f 7265 6c73 2f2e 7265 6c73 9d92  ..._rels/.rels..
+00001b40: b96e c330 0c40 7fc5 d09e 3007 d021 8833  .n.0.@....0..!.3
+00001b50: 65f1 1604 f901 56a2 0fd8 1205 8a45 9dbf  e.....V......E..
+00001b60: afda a571 900b 1979 3d3c 12dc 1e69 40ed  ...q...y=<...i@.
+00001b70: 38a4 b68b a918 fd10 5269 5ad5 b801 48b6  8.......RiZ...H.
+00001b80: 258f 69ce 9142 aed4 2c1e 3587 d240 44db  %.i..B..,.5..@D.
+00001b90: 6343 b05a 2c3e 402e 1966 b7bd 6416 a773  cC.Z,>@..f..d..s
+00001ba0: a457 885c d79d a53d db2f 4f41 6f80 af3a  .W.\...=./OAo..:
+00001bb0: 4c71 4269 484b 330e f0cd d27f 32f7 f30c  LqBiHK3.....2...
+00001bc0: 3545 e54a 2395 5b1a 78d3 e5fe 76e0 49d1  5E.J#.[.x...v.I.
+00001bd0: a122 5816 9a45 c9d3 a21d a57f 1dc7 f690  ."X..E..........
+00001be0: d3e9 af63 22b4 7a5b e8f9 7168 540a 8edc  ...c".z[..qhT...
+00001bf0: 6325 8c71 62b4 fe35 82c9 0fec 7e00 504b  c%.qb..5....~.PK
+00001c00: 0304 1400 0000 0800 803b 7756 e10c 7d10  .........;wV..}.
+00001c10: bb01 0000 2807 0000 0f00 0000 786c 2f77  ....(.......xl/w
+00001c20: 6f72 6b62 6f6f 6b2e 786d 6cb5 954b 6edb  orkbook.xml..Kn.
+00001c30: 3010 86af 22f0 0095 e2d8 4e62 44d9 3848  0...".....NbD.8H
+00001c40: 62d4 688d b8c8 9ea2 46d1 c07c 0824 6537  b.h.....F..|.$e7
+00001c50: 397d 4714 8410 2d40 74a3 1535 0ffc fc66  9}G...-@t..5...f
+00001c60: 440e ef2f c69e 2a63 4ed9 6f25 b52b 59eb  D../..*cN.o%.+Y.
+00001c70: 7db7 c973 275a 50dc 7d33 1d68 8a34 c62a  }..s'ZP.}3.h.4.*
+00001c80: eec9 b4ef b9eb 2cf0 dab5 005e c97c 5114  ......,....^.|Q.
+00001c90: eb5c 71d4 ece1 7ed2 3ad8 3c36 8c07 e1d1  .\q...~.:.<6....
+00001ca0: 6872 0e8e 3784 8bfb 8a0f 6676 4687 154a  hr..7.....fvF..J
+00001cb0: f41f 250b df12 58a6 50a3 c24f a84b 56b0  ..%...X.P..O.KV.
+00001cc0: ccb5 e6f2 622c 7e1a edb9 3c0a 6ba4 2cd9  ....b,~...<.k.,.
+00001cd0: d518 7803 eb51 fce3 3e0e 90bf 78e5 82c7  ..x..Q..>...x...
+00001ce0: f3ea 9513 48c9 d605 0936 689d 0f19 419f  ....H....6h...A.
+00001cf0: 13e3 1928 79b4 7a6f 9e50 7ab0 8fdc c3b3  ...(y.zo.Pz.....
+00001d00: 357d 87fa 7d90 a12a f2a8 8cd0 8769 1d9b  5}..}..*.....i..
+00001d10: b8b1 ffd3 46d3 3428 e0d1 885e 81f6 631f  ....F.4(...^..c.
+00001d20: 2dc8 0150 bb16 3bc7 32cd 1594 6cdb f28e  -..P..;.2...l...
+00001d30: 3886 8a68 8b5d 3d56 e709 2bea 95dd 2005  8..h.]=V..+... .
+00001d40: ecae 0e80 f3c1 1c2c 38ca 0881 8868 9120  .......,8....h. 
+00001d50: 5acc 4bb4 076e 35fd 9b67 c365 4474 9d20  Z.K..n5..g.eDt. 
+00001d60: ba9e 97e8 3b7c d0e1 ae23 9865 0266 392f  ....;|...#.e.f9/
+00001d70: cc51 620d 11ca 2a81 b29a 1765 db82 3845  .Qb...*....e..8E
+00001d80: 28eb 04ca 7a5e 949d 737d dc95 9b04 cacd  (...z^..s}......
+00001d90: bc28 af20 e1cc b580 3d9c 213e c1b7 09a6  .(. ....=.!>....
+00001da0: db99 6f79 5f49 1aa7 7f5d f2bb 04d0 ddcc  ..oy_I...]......
+00001db0: a778 508e 2760 911a 8145 18d2 d364 aea1  .xP.'`...E...d..
+00001dc0: 410d f50f 1272 e4a7 5742 1c6c 362c 4169  A....r..WB.l6,Ai
+00001dd0: b15c 5d51 654d 2fe5 967c 3ff5 def0 7a1a  .\]QeM/..|?...z.
+00001de0: f4d3 23f5 f007 504b 0304 1400 0000 0800  ..#...PK........
+00001df0: 803b 7756 0bde eded e500 0000 1507 0000  .;wV............
+00001e00: 1a00 0000 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
+00001e10: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 c5d5  kbook.xml.rels..
+00001e20: 4b8e c230 0c06 e0ab 5439 006e 0b94 875a  K..0....T9.n...Z
+00001e30: 566c d88e b840 54dc 8768 9b28 f668 e0f6  Vl...@T..h.(.h..
+00001e40: 5395 4531 62c1 0679 1539 517e 7f2b 3bff  S.E1b..y.9Q~.+;.
+00001e50: c1ce 72eb 066a 5a4f d1ad ef06 2a4c c3ec  ..r..jZO....*L..
+00001e60: f700 5436 d85b 5a38 8fc3 f852 b9d0 5b1e  ..T6.[Z8...R..[.
+00001e70: cb50 83b7 e5d5 d608 691c 6710 9e33 cc21  .P......i.g..3.!
+00001e80: 7fce 8cce 778f 9f24 baaa 6a4b 3cba f2b7  ....w..$..jK<...
+00001e90: c781 df04 c39f 0b57 6a10 d944 671b 6ae4  .......Wj..Dg.j.
+00001ea0: c2c0 ad9b af09 a623 598c c926 3a5d 0a13  .......#Y..&:]..
+00001eb0: 4e97 c480 3628 15a0 541f b414 a0a5 3e68  N...6(..T.....>h
+00001ec0: 2540 2b7d d05a 80d6 faa0 4c80 327d d046  %@+}.Z....L.2}.F
+00001ed0: 8036 faa0 ad00 6df5 413b 01da e983 9258  .6....m.A;.....X
+00001ee0: 4ec6 f88b 24e2 7b87 347b 1eb5 ecff cdd1  N...$.{.4{......
+00001ef0: cce3 5f9c db4f e5e3 f265 3d4c e318 c416  .._..O...e=L....
+00001f00: 3cfc 0350 4b03 0414 0000 0008 0080 3b77  <..PK.........;w
+00001f10: 56e1 ba79 943e 0100 0098 0800 0013 0000  V..y.>..........
+00001f20: 005b 436f 6e74 656e 745f 5479 7065 735d  .[Content_Types]
+00001f30: 2e78 6d6c cd96 cb4e c330 1045 7f25 cab6  .xml...N.0.E.%..
+00001f40: 4adc 1628 0fb5 dd00 5be8 821f 30c9 a4b1  J..(....[...0...
+00001f50: ea97 3cd3 92fe 3d93 f421 814a 4455 24bc  ..<...=..!.JDU$.
+00001f60: 8915 cfcc 3dd7 330b 7bfa b6f5 8049 63b4  ....=.3.{....Ic.
+00001f70: c559 5a13 f907 21b0 a8c1 48cc 9d07 cb91  .YZ...!...H.....
+00001f80: ca05 2389 7fc3 5278 59ac e412 c478 389c  ..#...RxY....x8.
+00001f90: 88c2 5902 4b19 b51a e97c fa04 955c 6b4a  ..Y.K....|...\kJ
+00001fa0: 9e1b de46 e5ec 2c0d a031 4d1e 7789 2d6b  ...F..,..1M.w.-k
+00001fb0: 964a efb5 2a24 715c 6c6c f98d 92ed 0939  .J..*$q\ll.....9
+00001fc0: 5776 3958 2b8f 034e 48c5 4942 1bf9 19b0  Wv9X+..NH.IB....
+00001fd0: af7b dd40 08aa 8464 2103 bd48 c359 a2d1  .{.@...d!..H.Y..
+00001fe0: 0269 ab01 f37e 8913 1e5d 55a9 024a 57ac  .i...~...]U..JW.
+00001ff0: 0d97 e4e8 03c8 126b 0032 3adf 890e fac9  .......k.2:.....
+00002000: c41d 86dd 7774 31bf 93e9 0372 e622 388f  ....wt1....r."8.
+00002010: 3cb1 00e7 e30e 2369 ab33 cf42 1048 f51f  <.....#i.3.B.H..
+00002020: f148 64e9 8bcf 07ed b44b 287f c9e6 f67e  .Hd......K(....~
+00002030: b8b0 eae6 81a2 5b2e eff1 d719 1ff5 cff4  ......[.........
+00002040: 318e c4c7 5524 3eae 23f1 7113 898f 4924  1...U$>.#.q...I$
+00002050: 3e6e 23f1 7117 898f fb48 7c8c 86ff 68e4  >n#.q....H|...h.
+00002060: ddb9 d55f df95 ed9a 1ba9 ec81 2fba 07c9  ..._......../...
+00002070: fc13 504b 0102 1403 1400 0000 0800 803b  ..PK...........;
+00002080: 7756 0741 4d62 8100 0000 b100 0000 1000  wV.AMb..........
+00002090: 0000 0000 0000 0000 0000 8001 0000 0000  ................
+000020a0: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
+000020b0: 504b 0102 1403 1400 0000 0800 803b 7756  PK...........;wV
+000020c0: 5d95 7193 ee00 0000 2b02 0000 1100 0000  ].q.....+.......
+000020d0: 0000 0000 0000 0000 8001 af00 0000 646f  ..............do
+000020e0: 6350 726f 7073 2f63 6f72 652e 786d 6c50  cProps/core.xmlP
+000020f0: 4b01 0214 0314 0000 0008 0080 3b77 5699  K...........;wV.
+00002100: 5c9c 2310 0600 009c 2700 0013 0000 0000  \.#.....'.......
+00002110: 0000 0000 0000 0080 01cc 0100 0078 6c2f  .............xl/
+00002120: 7468 656d 652f 7468 656d 6531 2e78 6d6c  theme/theme1.xml
+00002130: 504b 0102 1403 1400 0000 0800 803b 7756  PK...........;wV
+00002140: 8536 ce1a 6401 0000 f902 0000 1800 0000  .6..d...........
+00002150: 0000 0000 0000 0000 8081 0d08 0000 786c  ..............xl
+00002160: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00002170: 7431 2e78 6d6c 504b 0102 1403 1400 0000  t1.xmlPK........
+00002180: 0800 803b 7756 dc63 4ff2 7201 0000 3503  ...;wV.cO.r...5.
+00002190: 0000 1800 0000 0000 0000 0000 0000 8081  ................
+000021a0: a709 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+000021b0: 732f 7368 6565 7432 2e78 6d6c 504b 0102  s/sheet2.xmlPK..
+000021c0: 1403 1400 0000 0800 803b 7756 dbd4 6fe1  .........;wV..o.
+000021d0: 8e01 0000 0d04 0000 1800 0000 0000 0000  ................
+000021e0: 0000 0000 8081 4f0b 0000 786c 2f77 6f72  ......O...xl/wor
+000021f0: 6b73 6865 6574 732f 7368 6565 7433 2e78  ksheets/sheet3.x
+00002200: 6d6c 504b 0102 1403 1400 0000 0800 803b  mlPK...........;
+00002210: 7756 2328 370d 8c01 0000 a503 0000 1800  wV#(7...........
+00002220: 0000 0000 0000 0000 0000 8081 130d 0000  ................
+00002230: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00002240: 6565 7434 2e78 6d6c 504b 0102 1403 1400  eet4.xmlPK......
+00002250: 0000 0800 803b 7756 1334 6b2f 8b01 0000  .....;wV.4k/....
+00002260: d503 0000 1800 0000 0000 0000 0000 0000  ................
+00002270: 8081 d50e 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00002280: 6574 732f 7368 6565 7435 2e78 6d6c 504b  ets/sheet5.xmlPK
+00002290: 0102 1403 1400 0000 0800 803b 7756 e637  ...........;wV.7
+000022a0: 718b 7e01 0000 9303 0000 1800 0000 0000  q.~.............
+000022b0: 0000 0000 0000 8081 9610 0000 786c 2f77  ............xl/w
+000022c0: 6f72 6b73 6865 6574 732f 7368 6565 7436  orksheets/sheet6
+000022d0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+000022e0: 803b 7756 aca9 9829 4d01 0000 6d02 0000  .;wV...)M...m...
+000022f0: 1800 0000 0000 0000 0000 0000 8081 4a12  ..............J.
+00002300: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00002310: 7368 6565 7437 2e78 6d6c 504b 0102 1403  sheet7.xmlPK....
+00002320: 1400 0000 0800 803b 7756 aa5d a329 5a01  .......;wV.].)Z.
+00002330: 0000 b002 0000 1800 0000 0000 0000 0000  ................
+00002340: 0000 8081 cd13 0000 786c 2f77 6f72 6b73  ........xl/works
+00002350: 6865 6574 732f 7368 6565 7438 2e78 6d6c  heets/sheet8.xml
+00002360: 504b 0102 1403 1400 0000 0800 803b 7756  PK...........;wV
+00002370: ca3c de08 8201 0000 9b03 0000 1800 0000  .<..............
+00002380: 0000 0000 0000 0000 8081 5d15 0000 786c  ..........]...xl
+00002390: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+000023a0: 7439 2e78 6d6c 504b 0102 1403 1400 0000  t9.xmlPK........
+000023b0: 0800 803b 7756 88c5 88ed 4d01 0000 6e02  ...;wV....M...n.
+000023c0: 0000 1900 0000 0000 0000 0000 0000 8081  ................
+000023d0: 1517 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+000023e0: 732f 7368 6565 7431 302e 786d 6c50 4b01  s/sheet10.xmlPK.
+000023f0: 0214 0314 0000 0008 0080 3b77 567c f3a3  ..........;wV|..
+00002400: dc51 0200 00f6 0900 000d 0000 0000 0000  .Q..............
+00002410: 0000 0000 0080 0199 1800 0078 6c2f 7374  ...........xl/st
+00002420: 796c 6573 2e78 6d6c 504b 0102 1403 1400  yles.xmlPK......
+00002430: 0000 0800 803b 7756 978a bb1c c000 0000  .....;wV........
+00002440: 1302 0000 0b00 0000 0000 0000 0000 0000  ................
+00002450: 8001 151b 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
+00002460: 7350 4b01 0214 0314 0000 0008 0080 3b77  sPK...........;w
+00002470: 56e1 0c7d 10bb 0100 0028 0700 000f 0000  V..}.....(......
+00002480: 0000 0000 0000 0000 0080 01fe 1b00 0078  ...............x
+00002490: 6c2f 776f 726b 626f 6f6b 2e78 6d6c 504b  l/workbook.xmlPK
+000024a0: 0102 1403 1400 0000 0800 803b 7756 0bde  ...........;wV..
+000024b0: eded e500 0000 1507 0000 1a00 0000 0000  ................
+000024c0: 0000 0000 0000 8001 e61d 0000 786c 2f5f  ............xl/_
+000024d0: 7265 6c73 2f77 6f72 6b62 6f6f 6b2e 786d  rels/workbook.xm
+000024e0: 6c2e 7265 6c73 504b 0102 1403 1400 0000  l.relsPK........
+000024f0: 0800 803b 7756 e1ba 7994 3e01 0000 9808  ...;wV..y.>.....
+00002500: 0000 1300 0000 0000 0000 0000 0000 8001  ................
+00002510: 031f 0000 5b43 6f6e 7465 6e74 5f54 7970  ....[Content_Typ
+00002520: 6573 5d2e 786d 6c50 4b05 0600 0000 0012  es].xmlPK.......
+00002530: 0012 00b5 0400 0072 2000 0000 00         .......r ....
```

### Comparing `pymetamodel-0.2.7/examples/scientific-events/scientific-events.yaml` & `pymetamodel-0.3.0/examples/scientific-events/scientific-events.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,99 +9,78 @@
     prefix_reference: CrSchema/
   xsd:
     prefix_prefix: xsd
     prefix_reference: http://www.w3.org/2001/XMLSchema#
   shex:
     prefix_prefix: shex
     prefix_reference: http://www.w3.org/ns/shex#
-  schema:
-    prefix_prefix: schema
-    prefix_reference: http://schema.org/
 default_prefix: CrSchema
 default_range: string
 types:
   string:
     name: string
     description: A character string
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Text
     base: str
     uri: xsd:string
   integer:
     name: integer
     description: An integer
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Integer
     base: int
     uri: xsd:integer
   boolean:
     name: boolean
     description: A binary (true or false) value
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Boolean
     base: Bool
     uri: xsd:boolean
     repr: bool
   float:
     name: float
     description: A real number that conforms to the xsd:float specification
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Float
     base: float
     uri: xsd:float
   double:
     name: double
     description: A real number that conforms to the xsd:double specification
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:Float
     base: float
     uri: xsd:double
   decimal:
     name: decimal
     description: A real number with arbitrary precision that conforms to the xsd:decimal
       specification
     from_schema: https://w3id.org/linkml/types
-    broad_mappings:
-    - schema:Number
     base: Decimal
     uri: xsd:decimal
   time:
     name: time
     description: A time object represents a (local) time of day, independent of any
       particular day
     notes:
-    - URI is dateTime because OWL reasoners do not work with straight date or time
+    - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Time
     base: XSDTime
     uri: xsd:dateTime
     repr: str
   date:
     name: date
     description: a date (year, month and day) in an idealized calendar
     notes:
     - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Date
     base: XSDDate
     uri: xsd:date
     repr: str
   datetime:
     name: datetime
     description: The combination of a date and time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:DateTime
     base: XSDDateTime
     uri: xsd:dateTime
     repr: str
   date_or_datetime:
     name: date_or_datetime
     description: Either a date or a datetime
     from_schema: https://w3id.org/linkml/types
@@ -111,36 +90,18 @@
   uriorcurie:
     name: uriorcurie
     description: a URI or a CURIE
     from_schema: https://w3id.org/linkml/types
     base: URIorCURIE
     uri: xsd:anyURI
     repr: str
-  curie:
-    name: curie
-    conforms_to: https://www.w3.org/TR/curie/
-    description: a compact URI
-    comments:
-    - in RDF serializations this MUST be expanded to a URI
-    - in non-RDF serializations MAY be serialized as the compact representation
-    from_schema: https://w3id.org/linkml/types
-    base: Curie
-    uri: xsd:string
-    repr: str
   uri:
     name: uri
-    conforms_to: https://www.ietf.org/rfc/rfc3987.txt
     description: a complete URI
-    comments:
-    - in RDF serializations a slot with range of uri is treated as a literal or type
-      xsd:anyURI unless it is an identifier or a reference to an identifier, in which
-      case it is translated directly to a node
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:URL
     base: URI
     uri: xsd:anyURI
     repr: str
   ncname:
     name: ncname
     description: Prefix part of CURIE
     from_schema: https://w3id.org/linkml/types
```

### Comparing `pymetamodel-0.2.7/examples/scientific-events/scientific-events_puml.txt` & `pymetamodel-0.3.0/examples/scientific-events/scientific-events_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/teaching/TeachingSchema.mermaid` & `pymetamodel-0.3.0/examples/teaching/TeachingSchema.mermaid`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/teaching/TeachingSchema.puml` & `pymetamodel-0.3.0/examples/teaching/TeachingSchema.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/teaching/TeachingSchema.py` & `pymetamodel-0.3.0/examples/teaching/TeachingSchema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from TeachingSchema.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-08T09:54:50
+# Generation date: 2023-03-23T07:27:59
 # Schema: TeachingSchema
 #
 # id: TeachingSchema
 # description:
 # license:
 
 import dataclasses
@@ -18,26 +18,25 @@
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
 from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
 from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
 from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.metamodelcore import Bool, Curie, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
+from linkml_runtime.utils.metamodelcore import Bool, Decimal, ElementIdentifier, NCName, NodeIdentifier, URI, URIorCURIE, XSDDate, XSDDateTime, XSDTime
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
 TEACHINGSCHEMA = CurieNamespace('TeachingSchema', 'TeachingSchema/')
 LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
-SCHEMA = CurieNamespace('schema', 'http://schema.org/')
 SHEX = CurieNamespace('shex', 'http://www.w3.org/ns/shex#')
 XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = TEACHINGSCHEMA
 
 
 # Types
 class String(str):
@@ -124,22 +123,14 @@
     """ a URI or a CURIE """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uriorcurie"
     type_model_uri = TEACHINGSCHEMA.Uriorcurie
 
 
-class Curie(Curie):
-    """ a compact URI """
-    type_class_uri = XSD.string
-    type_class_curie = "xsd:string"
-    type_name = "curie"
-    type_model_uri = TEACHINGSCHEMA.Curie
-
-
 class Uri(URI):
     """ a complete URI """
     type_class_uri = XSD.anyURI
     type_class_curie = "xsd:anyURI"
     type_name = "uri"
     type_model_uri = TEACHINGSCHEMA.Uri
```

### Comparing `pymetamodel-0.2.7/examples/teaching/TeachingSchema.sidif` & `pymetamodel-0.3.0/examples/teaching/TeachingSchema.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/examples/teaching/TeachingSchema.yaml` & `pymetamodel-0.3.0/examples/teaching/TeachingSchema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,99 +9,78 @@
     prefix_reference: TeachingSchema/
   xsd:
     prefix_prefix: xsd
     prefix_reference: http://www.w3.org/2001/XMLSchema#
   shex:
     prefix_prefix: shex
     prefix_reference: http://www.w3.org/ns/shex#
-  schema:
-    prefix_prefix: schema
-    prefix_reference: http://schema.org/
 default_prefix: TeachingSchema
 default_range: string
 types:
   string:
     name: string
     description: A character string
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Text
     base: str
     uri: xsd:string
   integer:
     name: integer
     description: An integer
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Integer
     base: int
     uri: xsd:integer
   boolean:
     name: boolean
     description: A binary (true or false) value
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Boolean
     base: Bool
     uri: xsd:boolean
     repr: bool
   float:
     name: float
     description: A real number that conforms to the xsd:float specification
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Float
     base: float
     uri: xsd:float
   double:
     name: double
     description: A real number that conforms to the xsd:double specification
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:Float
     base: float
     uri: xsd:double
   decimal:
     name: decimal
     description: A real number with arbitrary precision that conforms to the xsd:decimal
       specification
     from_schema: https://w3id.org/linkml/types
-    broad_mappings:
-    - schema:Number
     base: Decimal
     uri: xsd:decimal
   time:
     name: time
     description: A time object represents a (local) time of day, independent of any
       particular day
     notes:
-    - URI is dateTime because OWL reasoners do not work with straight date or time
+    - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Time
     base: XSDTime
     uri: xsd:dateTime
     repr: str
   date:
     name: date
     description: a date (year, month and day) in an idealized calendar
     notes:
     - URI is dateTime because OWL reasoners don't work with straight date or time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:Date
     base: XSDDate
     uri: xsd:date
     repr: str
   datetime:
     name: datetime
     description: The combination of a date and time
     from_schema: https://w3id.org/linkml/types
-    exact_mappings:
-    - schema:DateTime
     base: XSDDateTime
     uri: xsd:dateTime
     repr: str
   date_or_datetime:
     name: date_or_datetime
     description: Either a date or a datetime
     from_schema: https://w3id.org/linkml/types
@@ -111,36 +90,18 @@
   uriorcurie:
     name: uriorcurie
     description: a URI or a CURIE
     from_schema: https://w3id.org/linkml/types
     base: URIorCURIE
     uri: xsd:anyURI
     repr: str
-  curie:
-    name: curie
-    conforms_to: https://www.w3.org/TR/curie/
-    description: a compact URI
-    comments:
-    - in RDF serializations this MUST be expanded to a URI
-    - in non-RDF serializations MAY be serialized as the compact representation
-    from_schema: https://w3id.org/linkml/types
-    base: Curie
-    uri: xsd:string
-    repr: str
   uri:
     name: uri
-    conforms_to: https://www.ietf.org/rfc/rfc3987.txt
     description: a complete URI
-    comments:
-    - in RDF serializations a slot with range of uri is treated as a literal or type
-      xsd:anyURI unless it is an identifier or a reference to an identifier, in which
-      case it is translated directly to a node
     from_schema: https://w3id.org/linkml/types
-    close_mappings:
-    - schema:URL
     base: URI
     uri: xsd:anyURI
     repr: str
   ncname:
     name: ncname
     description: Prefix part of CURIE
     from_schema: https://w3id.org/linkml/types
```

### Comparing `pymetamodel-0.2.7/examples/teaching/TeachingSchema_puml.txt` & `pymetamodel-0.3.0/examples/teaching/TeachingSchema_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/meta/metamodel.py` & `pymetamodel-0.3.0/meta/metamodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,16 @@
         if not hasattr(prop, "topic"):
             self.error(f"prop  {prop} has no topic")
             return False
         topic_name = prop.topic
         if not hasattr(prop, "name"):
             self.error(f"prop {prop} has no name")
             return False
+        if not hasattr(prop, "type"):
+            prop.type="Text"
         topic=self.lookupTopic(topic_name,f"property {prop.name}")
         if topic:
             topic.properties[prop.name] = prop  
             return True 
         
     def createProperty4TopicLink(self,tl:'TopicLink')->'Propertx':
         """
```

### Comparing `pymetamodel-0.2.7/meta/metamodel_cmd.py` & `pymetamodel-0.3.0/meta/metamodel_cmd.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/meta/mw.py` & `pymetamodel-0.3.0/meta/mw.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/meta/profiler.py` & `pymetamodel-0.3.0/meta/profiler.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/meta/sidif2linkml.py` & `pymetamodel-0.3.0/meta/sidif2linkml.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/meta/smw_type.py` & `pymetamodel-0.3.0/meta/smw_type.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/meta/uml.py` & `pymetamodel-0.3.0/meta/uml.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/meta/version.py` & `pymetamodel-0.3.0/meta/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     '''
     Version handling for pyMetaModel
     '''
     name="pyMetaModel"
     description='pyMetaModel: MetaModel for Knowledge Graphs'
     version=meta.__version__
     date = '2022-11-30'
-    updated = '2023-02-19'
+    updated = '2023-04-09'
     authors='Wolfgang Fahl'
     doc_url="https://wiki.bitplan.com/index.php/pyMetaModel"
     chat_url="https://github.com/WolfgangFahl/pyMetaModel/discussions"
     cm_url="https://github.com/WolfgangFahl/pyMetaModel"
     license=f'''Copyright 2022 contributors. All rights reserved.
   Licensed under the Apache License 2.0
   http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pymetamodel-0.2.7/scripts/genexamples` & `pymetamodel-0.3.0/scripts/genexamples`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/scripts/test` & `pymetamodel-0.3.0/scripts/test`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/tests/basemwtest.py` & `pymetamodel-0.3.0/tests/basemwtest.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/tests/basetest.py` & `pymetamodel-0.3.0/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/tests/test_linkml.py` & `pymetamodel-0.3.0/tests/test_linkml.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/tests/test_metamodel.py` & `pymetamodel-0.3.0/tests/test_metamodel.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/tests/test_mw.py` & `pymetamodel-0.3.0/tests/test_mw.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/tests/test_plantuml.py` & `pymetamodel-0.3.0/tests/test_plantuml.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/tests/test_sidif.py` & `pymetamodel-0.3.0/tests/test_sidif.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/.gitignore` & `pymetamodel-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/LICENSE` & `pymetamodel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/README.md` & `pymetamodel-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.2.7/pyproject.toml` & `pymetamodel-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         # https://pypi.org/project/py-3rdparty-mediawiki/
 		'py-3rdparty-mediawiki>=0.8.0',
 		# https://pypi.org/project/pylodstorage/
         'pyLodStorage>=0.4.7',
 		# https://pypi.org/project/mwparserfromhell/
 		'mwparserfromhell>=0.6.4',
 		# https://pypi.org/project/linkml/
-		'linkml>=1.4.4',
+		'linkml>=1.4.11',
 		# https://pypi.org/project/linkml-runtime/
-		'linkml-runtime>=1.4.5',
+		'linkml-runtime>=1.4.10',
 		# https://github.com/konradhalas/dacite
 		'dacite>=1.7.0',
      ]
 
 requires-python = ">=3.8"
 classifiers=[
     "Development Status :: 4 - Beta",
```

### Comparing `pymetamodel-0.2.7/PKG-INFO` & `pymetamodel-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMetaModel
-Version: 0.2.7
+Version: 0.3.0
 Project-URL: Home, https://github.com/WolfgangFahl/pyMetaModel
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/PyMetaModel
 Project-URL: Source, https://github.com/WolfgangFahl/pyMetaModel
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -218,16 +218,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Requires-Dist: dacite>=1.7.0
-Requires-Dist: linkml-runtime>=1.4.5
-Requires-Dist: linkml>=1.4.4
+Requires-Dist: linkml-runtime>=1.4.10
+Requires-Dist: linkml>=1.4.11
 Requires-Dist: mwparserfromhell>=0.6.4
 Requires-Dist: py-3rdparty-mediawiki>=0.8.0
 Requires-Dist: py-sidif>=0.1.0
 Requires-Dist: pylodstorage>=0.4.7
 Requires-Dist: urllib3
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
```

