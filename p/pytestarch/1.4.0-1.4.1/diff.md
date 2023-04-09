# Comparing `tmp/pytestarch-1.4.0.tar.gz` & `tmp/pytestarch-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestarch-1.4.0.tar", max compression
+gzip compressed data, was "pytestarch-1.4.1.tar", max compression
```

## Comparing `pytestarch-1.4.0.tar` & `pytestarch-1.4.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11311 2023-04-09 18:30:26.608422 pytestarch-1.4.0/LICENSE
--rwxr-xr-x   0        0        0     1658 2023-04-09 18:30:26.608422 pytestarch-1.4.0/README.md
--rw-r--r--   0        0        0     1541 2023-04-09 18:30:26.612422 pytestarch-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      555 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/dependency_to_rule_converter.py
--rw-r--r--   0        0        0     8085 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/diagram_parser.py
--rw-r--r--   0        0        0     4024 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/diagram_rule.py
--rw-r--r--   0        0        0      126 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/exceptions.py
--rw-r--r--   0        0        0      215 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/parsed_dependencies.py
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/__init__.py
--rw-r--r--   0        0        0     8432 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/breadth_first_searches.py
--rw-r--r--   0        0        0     7786 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_architecture.py
--rw-r--r--   0        0        0     2939 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_graph.py
--rw-r--r--   0        0        0      696 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_structures.py
--rw-r--r--   0        0        0      123 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/exceptions.py
--rw-r--r--   0        0        0     3531 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/module_name_converter.py
--rw-r--r--   0        0        0    11036 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/networkxgraph.py
--rw-r--r--   0        0        0     1893 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/types.py
--rw-r--r--   0        0        0      612 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/utils.py
--rw-r--r--   0        0        0      171 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/__init__.py
--rw-r--r--   0        0        0      378 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/config.py
--rw-r--r--   0        0        0     2214 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/converter.py
--rw-r--r--   0        0        0       80 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/exceptions.py
--rw-r--r--   0        0        0     1088 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/file_filter.py
--rw-r--r--   0        0        0     1450 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/import_filter.py
--rw-r--r--   0        0        0     1895 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/import_types.py
--rw-r--r--   0        0        0     1323 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py
--rw-r--r--   0        0        0     2842 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/parser.py
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/graph_generation/__init__.py
--rw-r--r--   0        0        0     4553 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py
--rwxr-xr-x   0        0        0     3770 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/pytestarch.py
--rw-r--r--   0        0        0    25816 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/LANGUAGE_DEFINTION.md
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/__init__.py
--rw-r--r--   0        0        0     8156 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/base_language.py
--rw-r--r--   0        0        0       85 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/exceptions.py
--rw-r--r--   0        0        0     7699 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/layered_architecture_rule.py
--rw-r--r--   0        0        0      914 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/multiple_rule_applier.py
--rw-r--r--   0        0        0    12304 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/rule.py
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/error_message/__init__.py
--rw-r--r--   0        0        0    20878 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/error_message/message_generator.py
--rw-r--r--   0        0        0       82 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/__init__.py
--rw-r--r--   0        0        0     2517 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py
--rw-r--r--   0        0        0    11661 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py
--rw-r--r--   0        0        0     1691 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/module_requirement.py
--rw-r--r--   0        0        0     9989 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_matcher.py
--rw-r--r--   0        0        0    17861 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py
--rw-r--r--   0        0        0      802 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_violations.py
--rw-r--r--   0        0        0        0 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/utils/__init__.py
--rw-r--r--   0        0        0      576 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/utils/decorators.py
--rw-r--r--   0        0        0     1489 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/utils/partial_match_to_regex_converter.py
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 pytestarch-1.4.0/setup.py
--rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 pytestarch-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11311 2023-04-09 18:39:45.177121 pytestarch-1.4.1/LICENSE
+-rwxr-xr-x   0        0        0     1646 2023-04-09 18:39:45.177121 pytestarch-1.4.1/README.md
+-rw-r--r--   0        0        0     1541 2023-04-09 18:39:45.177121 pytestarch-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/dependency_to_rule_converter.py
+-rw-r--r--   0        0        0     8085 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/diagram_parser.py
+-rw-r--r--   0        0        0     4024 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/diagram_rule.py
+-rw-r--r--   0        0        0      126 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/exceptions.py
+-rw-r--r--   0        0        0      215 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/parsed_dependencies.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/__init__.py
+-rw-r--r--   0        0        0     8432 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/breadth_first_searches.py
+-rw-r--r--   0        0        0     7786 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_architecture.py
+-rw-r--r--   0        0        0     2939 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_graph.py
+-rw-r--r--   0        0        0      696 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_structures.py
+-rw-r--r--   0        0        0      123 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/exceptions.py
+-rw-r--r--   0        0        0     3531 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/module_name_converter.py
+-rw-r--r--   0        0        0    11036 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/networkxgraph.py
+-rw-r--r--   0        0        0     1893 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/types.py
+-rw-r--r--   0        0        0      612 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/utils.py
+-rw-r--r--   0        0        0      171 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/config.py
+-rw-r--r--   0        0        0     2214 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/converter.py
+-rw-r--r--   0        0        0       80 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/exceptions.py
+-rw-r--r--   0        0        0     1088 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/file_filter.py
+-rw-r--r--   0        0        0     1450 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/import_filter.py
+-rw-r--r--   0        0        0     1895 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/import_types.py
+-rw-r--r--   0        0        0     1323 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py
+-rw-r--r--   0        0        0     2842 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/parser.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/graph_generation/__init__.py
+-rw-r--r--   0        0        0     4553 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py
+-rwxr-xr-x   0        0        0     3770 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/pytestarch.py
+-rw-r--r--   0        0        0    25816 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/LANGUAGE_DEFINTION.md
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/__init__.py
+-rw-r--r--   0        0        0     8156 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/base_language.py
+-rw-r--r--   0        0        0       85 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/exceptions.py
+-rw-r--r--   0        0        0     7699 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/layered_architecture_rule.py
+-rw-r--r--   0        0        0      914 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/multiple_rule_applier.py
+-rw-r--r--   0        0        0    12304 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/rule.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/error_message/__init__.py
+-rw-r--r--   0        0        0    20878 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/error_message/message_generator.py
+-rw-r--r--   0        0        0       82 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/__init__.py
+-rw-r--r--   0        0        0     2517 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py
+-rw-r--r--   0        0        0    11661 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py
+-rw-r--r--   0        0        0     1691 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/module_requirement.py
+-rw-r--r--   0        0        0     9989 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_matcher.py
+-rw-r--r--   0        0        0    17861 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py
+-rw-r--r--   0        0        0      802 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_violations.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/utils/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/utils/decorators.py
+-rw-r--r--   0        0        0     1489 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/utils/partial_match_to_regex_converter.py
+-rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 pytestarch-1.4.1/setup.py
+-rw-r--r--   0        0        0     3097 1970-01-01 00:00:00.000000 pytestarch-1.4.1/PKG-INFO
```

### Comparing `pytestarch-1.4.0/LICENSE` & `pytestarch-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/README.md` & `pytestarch-1.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 ## Usage Guide
 Three steps are required to test an architectural rule:
 
 1) Create an evaluable representation of the source code you want to test
 
 ```
-from pytestarch.pytestarch import get_evaluable_architecture
+from pytestarch import get_evaluable_architecture
 
 evaluable = get_evaluable_architecture("/home/dummy/project", "/home/dummy/project/src")
 ```
 This will scan all python files under /home/dummy/project/src for imports and build an internal representation that can
 later be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external 
 dependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),
 you could use a fixture for this evaluable object.
 
 2) Define an architectural rule
 ```
-from pytestarch. import Rule
+from pytestarch import Rule
 
 rule = Rule() \
         .modules_that() \
         .are_named("src.moduleB") \
         .should_not() \
         .be_imported_by_modules_that() \
         .are_sub_modules_of("src.moduleA") \
```

### Comparing `pytestarch-1.4.0/pyproject.toml` & `pytestarch-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyTestArch"
-version = "1.4.0"
+version = "1.4.1"
 description = "Test framework for software architecture based on imports between modules"
 authors = ["zyskarch <zyskarch@gmail.com>"]
 maintainers = ["zyskarch <zyskarch@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 documentation = "https://zyskarch.github.io/pytestarch/"
 repository = "https://github.com/zyskarch/pytestarch"
```

### Comparing `pytestarch-1.4.0/src/pytestarch/__init__.py` & `pytestarch-1.4.1/src/pytestarch/__init__.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/diagram_extension/dependency_to_rule_converter.py` & `pytestarch-1.4.1/src/pytestarch/diagram_extension/dependency_to_rule_converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/diagram_extension/diagram_parser.py` & `pytestarch-1.4.1/src/pytestarch/diagram_extension/diagram_parser.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/diagram_extension/diagram_rule.py` & `pytestarch-1.4.1/src/pytestarch/diagram_extension/diagram_rule.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure/breadth_first_searches.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure/breadth_first_searches.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_architecture.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_architecture.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_graph.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_graph.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_structures.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_structures.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure/module_name_converter.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure/module_name_converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure/networkxgraph.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure/networkxgraph.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure/types.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure/types.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure/utils.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure/utils.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/converter.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/file_filter.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/file_filter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/import_filter.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/import_filter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/import_types.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/import_types.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/parser.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/parser.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py` & `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/pytestarch.py` & `pytestarch-1.4.1/src/pytestarch/pytestarch.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/query_language/LANGUAGE_DEFINTION.md` & `pytestarch-1.4.1/src/pytestarch/query_language/LANGUAGE_DEFINTION.md`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/query_language/base_language.py` & `pytestarch-1.4.1/src/pytestarch/query_language/base_language.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/query_language/layered_architecture_rule.py` & `pytestarch-1.4.1/src/pytestarch/query_language/layered_architecture_rule.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/query_language/multiple_rule_applier.py` & `pytestarch-1.4.1/src/pytestarch/query_language/multiple_rule_applier.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/query_language/rule.py` & `pytestarch-1.4.1/src/pytestarch/query_language/rule.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/rule_assessment/error_message/message_generator.py` & `pytestarch-1.4.1/src/pytestarch/rule_assessment/error_message/message_generator.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py` & `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py` & `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/module_requirement.py` & `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/module_requirement.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_matcher.py` & `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_matcher.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py` & `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_violations.py` & `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_violations.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/utils/decorators.py` & `pytestarch-1.4.1/src/pytestarch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/src/pytestarch/utils/partial_match_to_regex_converter.py` & `pytestarch-1.4.1/src/pytestarch/utils/partial_match_to_regex_converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.0/setup.py` & `pytestarch-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 {'': ['*']}
 
 install_requires = \
 ['b2>=3.7.1,<4.0.0', 'matplotlib>=3.5.3,<4.0.0', 'networkx>=3.0,<4.0']
 
 setup_kwargs = {
     'name': 'pytestarch',
-    'version': '1.4.0',
+    'version': '1.4.1',
     'description': 'Test framework for software architecture based on imports between modules',
-    'long_description': '# Welcome to PyTestArch\n\nPyTestArch is an open source library that allows users to define architectural rules and test their code against them. It is \ngenerally inspired by [ArchUnit](https://www.archunit.org/).\n\n## Installation Guide\nPyTestArch is available via [PyPI](https://pypi.org/project/pytestarch/) and can be installed e.g. via pip: `pip install pytestarch`.\n\n## Usage Guide\nThree steps are required to test an architectural rule:\n\n1) Create an evaluable representation of the source code you want to test\n\n```\nfrom pytestarch.pytestarch import get_evaluable_architecture\n\nevaluable = get_evaluable_architecture("/home/dummy/project", "/home/dummy/project/src")\n```\nThis will scan all python files under /home/dummy/project/src for imports and build an internal representation that can\nlater be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external \ndependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),\nyou could use a fixture for this evaluable object.\n\n2) Define an architectural rule\n```\nfrom pytestarch. import Rule\n\nrule = Rule() \\\n        .modules_that() \\\n        .are_named("src.moduleB") \\\n        .should_not() \\\n        .be_imported_by_modules_that() \\\n        .are_sub_modules_of("src.moduleA") \\\n```\n\nThis rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module\nthat is a submodule of "src.moduleA", excluding "src.moduleA" itself.\n\n3) Evaluate your code against this rule\n\n```\nrule.assert_applies(evaluable)\n```\nThat\'s it!\n',
+    'long_description': '# Welcome to PyTestArch\n\nPyTestArch is an open source library that allows users to define architectural rules and test their code against them. It is \ngenerally inspired by [ArchUnit](https://www.archunit.org/).\n\n## Installation Guide\nPyTestArch is available via [PyPI](https://pypi.org/project/pytestarch/) and can be installed e.g. via pip: `pip install pytestarch`.\n\n## Usage Guide\nThree steps are required to test an architectural rule:\n\n1) Create an evaluable representation of the source code you want to test\n\n```\nfrom pytestarch import get_evaluable_architecture\n\nevaluable = get_evaluable_architecture("/home/dummy/project", "/home/dummy/project/src")\n```\nThis will scan all python files under /home/dummy/project/src for imports and build an internal representation that can\nlater be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external \ndependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),\nyou could use a fixture for this evaluable object.\n\n2) Define an architectural rule\n```\nfrom pytestarch import Rule\n\nrule = Rule() \\\n        .modules_that() \\\n        .are_named("src.moduleB") \\\n        .should_not() \\\n        .be_imported_by_modules_that() \\\n        .are_sub_modules_of("src.moduleA") \\\n```\n\nThis rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module\nthat is a submodule of "src.moduleA", excluding "src.moduleA" itself.\n\n3) Evaluate your code against this rule\n\n```\nrule.assert_applies(evaluable)\n```\nThat\'s it!\n',
     'author': 'zyskarch',
     'author_email': 'zyskarch@gmail.com',
     'maintainer': 'zyskarch',
     'maintainer_email': 'zyskarch@gmail.com',
     'url': 'https://github.com/zyskarch/pytestarch',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pytestarch-1.4.0/PKG-INFO` & `pytestarch-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestarch
-Version: 1.4.0
+Version: 1.4.1
 Summary: Test framework for software architecture based on imports between modules
 Home-page: https://github.com/zyskarch/pytestarch
 License: Apache-2.0
 Keywords: architecture,test
 Author: zyskarch
 Author-email: zyskarch@gmail.com
 Maintainer: zyskarch
@@ -42,26 +42,26 @@
 
 ## Usage Guide
 Three steps are required to test an architectural rule:
 
 1) Create an evaluable representation of the source code you want to test
 
 ```
-from pytestarch.pytestarch import get_evaluable_architecture
+from pytestarch import get_evaluable_architecture
 
 evaluable = get_evaluable_architecture("/home/dummy/project", "/home/dummy/project/src")
 ```
 This will scan all python files under /home/dummy/project/src for imports and build an internal representation that can
 later be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external 
 dependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),
 you could use a fixture for this evaluable object.
 
 2) Define an architectural rule
 ```
-from pytestarch. import Rule
+from pytestarch import Rule
 
 rule = Rule() \
         .modules_that() \
         .are_named("src.moduleB") \
         .should_not() \
         .be_imported_by_modules_that() \
         .are_sub_modules_of("src.moduleA") \
```

