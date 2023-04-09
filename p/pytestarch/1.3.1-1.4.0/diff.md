# Comparing `tmp/pytestarch-1.3.1.tar.gz` & `tmp/pytestarch-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestarch-1.3.1.tar", max compression
+gzip compressed data, was "pytestarch-1.4.0.tar", max compression
```

## Comparing `pytestarch-1.3.1.tar` & `pytestarch-1.4.0.tar`

### file list

```diff
@@ -1,49 +1,56 @@
--rw-r--r--   0        0        0    11311 2023-01-27 14:29:07.767978 pytestarch-1.3.1/LICENSE
--rwxr-xr-x   0        0        0     1675 2023-01-27 14:29:07.767978 pytestarch-1.3.1/README.md
--rw-r--r--   0        0        0     1572 2023-01-27 14:29:07.771978 pytestarch-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      433 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/diagram_extension/__init__.py
--rw-r--r--   0        0        0     2726 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/diagram_extension/dependency_to_rule_converter.py
--rw-r--r--   0        0        0     8085 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/diagram_extension/diagram_parser.py
--rw-r--r--   0        0        0     4024 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/diagram_extension/diagram_rule.py
--rw-r--r--   0        0        0      126 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/diagram_extension/exceptions.py
--rw-r--r--   0        0        0      215 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/diagram_extension/parsed_dependencies.py
--rw-r--r--   0        0        0        0 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/__init__.py
--rw-r--r--   0        0        0     8442 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/breadth_first_searches.py
--rw-r--r--   0        0        0     5099 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/evaluable_architecture.py
--rw-r--r--   0        0        0     7631 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/evaluable_graph.py
--rw-r--r--   0        0        0      696 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/evaluable_structures.py
--rw-r--r--   0        0        0       80 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/exceptions.py
--rw-r--r--   0        0        0    10551 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/networkxgraph.py
--rw-r--r--   0        0        0     1973 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/types.py
--rw-r--r--   0        0        0      612 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure/utils.py
--rw-r--r--   0        0        0      171 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/__init__.py
--rw-r--r--   0        0        0      350 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/config.py
--rw-r--r--   0        0        0     2214 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/converter.py
--rw-r--r--   0        0        0       80 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/exceptions.py
--rw-r--r--   0        0        0     1985 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/file_filter.py
--rw-r--r--   0        0        0     1450 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/import_filter.py
--rw-r--r--   0        0        0     1887 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/import_types.py
--rw-r--r--   0        0        0     1323 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py
--rw-r--r--   0        0        0     2842 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/parser.py
--rw-r--r--   0        0        0        0 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/graph_generation/__init__.py
--rw-r--r--   0        0        0     4548 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py
--rwxr-xr-x   0        0        0     2914 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/pytestarch.py
--rw-r--r--   0        0        0    13341 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/query_language/LANGUAGE_DEFINTION.md
--rw-r--r--   0        0        0        0 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/query_language/__init__.py
--rw-r--r--   0        0        0     4003 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/query_language/base_language.py
--rw-r--r--   0        0        0       85 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/query_language/exceptions.py
--rw-r--r--   0        0        0      914 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/query_language/multiple_rule_applier.py
--rw-r--r--   0        0        0     9443 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/query_language/rule.py
--rw-r--r--   0        0        0        0 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/__init__.py
--rw-r--r--   0        0        0        0 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/error_message/__init__.py
--rw-r--r--   0        0        0    13416 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/error_message/message_generator.py
--rw-r--r--   0        0        0       82 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/rule_check/__init__.py
--rw-r--r--   0        0        0     5231 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py
--rw-r--r--   0        0        0     1700 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/rule_check/module_requirement.py
--rw-r--r--   0        0        0     3965 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/rule_check/rule_matcher.py
--rw-r--r--   0        0        0     1051 2023-01-27 14:29:07.771978 pytestarch-1.3.1/src/pytestarch/rule_assessment/rule_check/rule_violations.py
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 pytestarch-1.3.1/setup.py
--rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 pytestarch-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11311 2023-04-09 18:30:26.608422 pytestarch-1.4.0/LICENSE
+-rwxr-xr-x   0        0        0     1658 2023-04-09 18:30:26.608422 pytestarch-1.4.0/README.md
+-rw-r--r--   0        0        0     1541 2023-04-09 18:30:26.612422 pytestarch-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/dependency_to_rule_converter.py
+-rw-r--r--   0        0        0     8085 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/diagram_parser.py
+-rw-r--r--   0        0        0     4024 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/diagram_rule.py
+-rw-r--r--   0        0        0      126 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/exceptions.py
+-rw-r--r--   0        0        0      215 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/diagram_extension/parsed_dependencies.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/__init__.py
+-rw-r--r--   0        0        0     8432 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/breadth_first_searches.py
+-rw-r--r--   0        0        0     7786 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_architecture.py
+-rw-r--r--   0        0        0     2939 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_graph.py
+-rw-r--r--   0        0        0      696 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_structures.py
+-rw-r--r--   0        0        0      123 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/exceptions.py
+-rw-r--r--   0        0        0     3531 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/module_name_converter.py
+-rw-r--r--   0        0        0    11036 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/networkxgraph.py
+-rw-r--r--   0        0        0     1893 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/types.py
+-rw-r--r--   0        0        0      612 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure/utils.py
+-rw-r--r--   0        0        0      171 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/config.py
+-rw-r--r--   0        0        0     2214 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/converter.py
+-rw-r--r--   0        0        0       80 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/exceptions.py
+-rw-r--r--   0        0        0     1088 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/file_filter.py
+-rw-r--r--   0        0        0     1450 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/import_filter.py
+-rw-r--r--   0        0        0     1895 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/import_types.py
+-rw-r--r--   0        0        0     1323 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py
+-rw-r--r--   0        0        0     2842 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/parser.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/graph_generation/__init__.py
+-rw-r--r--   0        0        0     4553 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py
+-rwxr-xr-x   0        0        0     3770 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/pytestarch.py
+-rw-r--r--   0        0        0    25816 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/LANGUAGE_DEFINTION.md
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/__init__.py
+-rw-r--r--   0        0        0     8156 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/base_language.py
+-rw-r--r--   0        0        0       85 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/exceptions.py
+-rw-r--r--   0        0        0     7699 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/layered_architecture_rule.py
+-rw-r--r--   0        0        0      914 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/multiple_rule_applier.py
+-rw-r--r--   0        0        0    12304 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/query_language/rule.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/error_message/__init__.py
+-rw-r--r--   0        0        0    20878 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/error_message/message_generator.py
+-rw-r--r--   0        0        0       82 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.612422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/__init__.py
+-rw-r--r--   0        0        0     2517 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py
+-rw-r--r--   0        0        0    11661 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py
+-rw-r--r--   0        0        0     1691 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/module_requirement.py
+-rw-r--r--   0        0        0     9989 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_matcher.py
+-rw-r--r--   0        0        0    17861 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py
+-rw-r--r--   0        0        0      802 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/rule_violations.py
+-rw-r--r--   0        0        0        0 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/utils/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/utils/decorators.py
+-rw-r--r--   0        0        0     1489 2023-04-09 18:30:26.616422 pytestarch-1.4.0/src/pytestarch/utils/partial_match_to_regex_converter.py
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 pytestarch-1.4.0/setup.py
+-rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 pytestarch-1.4.0/PKG-INFO
```

### Comparing `pytestarch-1.3.1/LICENSE` & `pytestarch-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/README.md` & `pytestarch-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 This will scan all python files under /home/dummy/project/src for imports and build an internal representation that can
 later be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external 
 dependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),
 you could use a fixture for this evaluable object.
 
 2) Define an architectural rule
 ```
-from pytestarch.query_language.base_language import Rule
+from pytestarch. import Rule
 
-rule = Rule()
-        .modules_that()
-        .are_named("src.moduleB")
-        .should_not()
-        .be_imported_by_modules_that()
-        .are_sub_modules_of("src.moduleA"),
+rule = Rule() \
+        .modules_that() \
+        .are_named("src.moduleB") \
+        .should_not() \
+        .be_imported_by_modules_that() \
+        .are_sub_modules_of("src.moduleA") \
 ```
 
 This rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module
 that is a submodule of "src.moduleA", excluding "src.moduleA" itself.
 
 3) Evaluate your code against this rule
```

### Comparing `pytestarch-1.3.1/pyproject.toml` & `pytestarch-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyTestArch"
-version = "1.3.1"
+version = "1.4.0"
 description = "Test framework for software architecture based on imports between modules"
 authors = ["zyskarch <zyskarch@gmail.com>"]
 maintainers = ["zyskarch <zyskarch@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 documentation = "https://zyskarch.github.io/pytestarch/"
 repository = "https://github.com/zyskarch/pytestarch"
@@ -25,18 +25,19 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/zyskarch/pytestarch/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 networkx = "^3.0"
 matplotlib = "^3.5.3"
+b2 = "^3.7.1"
 
 [tool.poetry.dev-dependencies]
 mkdocs = "^1.3.1"
-mkdocstrings-python = "^0.8.2"
+mkdocstrings-python = "^0.9.0"
 mkdocs-material = "^9.0.4"
 nox = "^2022.8.7"
 pre-commit = "^2.20.0"
 pytest = "^7.1.2"
 coverage = "^7.0.5"
 mike = "^1.1.2"
 
@@ -45,13 +46,12 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 sourcepath = "src"
 
 [tool.isort]
 profile = "black"
-extend_skip = ["src/pytestarch/__init__.py"]
 add_imports = ["from __future__ import annotations"]
 
 [tool.bandit]
 [tool.bandit.assert_used]
 skips = ["*/test_*.py"]
```

### Comparing `pytestarch-1.3.1/src/pytestarch/diagram_extension/dependency_to_rule_converter.py` & `pytestarch-1.4.0/src/pytestarch/diagram_extension/dependency_to_rule_converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/diagram_extension/diagram_parser.py` & `pytestarch-1.4.0/src/pytestarch/diagram_extension/diagram_parser.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/diagram_extension/diagram_rule.py` & `pytestarch-1.4.0/src/pytestarch/diagram_extension/diagram_rule.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure/breadth_first_searches.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure/breadth_first_searches.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pytestarch.eval_structure.utils import get_excluded_nodes, get_node, to_modules
 
 
 def get_dependency_between_modules(
     graph: AbstractGraph, dependent: Module, dependent_upon: Module
 ) -> List[StrictDependency]:
     dependent_node = get_node(dependent)
-    dependent_upon_nodes = _get_all_submodules_of(graph, dependent_upon)
+    dependent_upon_nodes = get_all_submodules_of(graph, dependent_upon)
 
     nodes_to_exclude = get_excluded_nodes([dependent, dependent_upon])
 
     nodes_to_check = [dependent_node]
     checked_nodes = set()
 
     dependencies = []
@@ -40,33 +40,33 @@
                 and child not in nodes_to_exclude
             ):
                 dependencies.append(tuple(to_modules([node, child])))
     return dependencies  # type: ignore
 
 
 def any_dependency_to_module_other_than(  # noqa: C901
-    graph: AbstractGraph, dependent: Module, dependent_upons: List[Module]
+    graph: AbstractGraph, dependent: Module, dependent_upons: Set[Module]
 ) -> List[StrictDependency]:
     # nodes to exclude are nodes that once reached will not have their submodules analysed next
     nodes_to_exclude = set()
     for dependent_upon in dependent_upons:
         if dependent_upon == dependent:
             continue
-        nodes_to_exclude.update(_get_all_submodules_of(graph, dependent_upon))
+        nodes_to_exclude.update(get_all_submodules_of(graph, dependent_upon))
 
     nodes_fulfilling_criteria = []
 
     # nodes that count as not fulfilling the criterion are nodes that would technically fulfill the criterion,
     # but have to be excluded for consistency reasons. For example, if the dependent is called A and has two
     # submodules A.X and A.Y. If A.X and A.Y import each other, this would be registered as fulfilling the
     # requirement of a module other than the dependent upons (assuming that A.X and A.Y are not in this list).
     # however, this is not really an import of a module outside A, which is what we are actually looking for
 
     # should submodules of the dependent module import each other, this does not count as a dependency
-    nodes_that_do_not_fulfill_criterion = _get_all_submodules_of(graph, dependent)
+    nodes_that_do_not_fulfill_criterion = get_all_submodules_of(graph, dependent)
 
     if dependent.parent_module is not None:
         # if the parent module is set and has a dependency other than dependent upon, it should not count as only
         # the dependent and its submodules should be considered
         # Example: if we are looking for imports by A.X, we do not care if A itself imports something
         # (but we do care if A.X.M (submodule of A.X) imports something, as this is part of A.X)
         nodes_to_exclude.add(dependent.parent_module)
@@ -92,50 +92,49 @@
             continue
 
         checked_nodes.add(node)
 
         children = graph.direct_successor_nodes(node)
 
         for child in children:
-
             if not graph.parent_child_relationship(node, child):
                 if (
                     child not in nodes_to_exclude
                     and child not in nodes_that_do_not_fulfill_criterion
                 ):
                     nodes_fulfilling_criteria.append(tuple(to_modules([node, child])))
                 else:
                     nodes_to_check.append(child)
 
     return nodes_fulfilling_criteria  # type: ignore
 
 
 def any_other_dependency_to_module_than(  # noqa: C901
-    graph: AbstractGraph, dependents: List[Module], dependent_upon: Module
+    graph: AbstractGraph, dependents: Set[Module], dependent_upon: Module
 ) -> List[StrictDependency]:
     # submodules of the dependent upon module do not count as an import that is not the dependent upon module
     # submodules of and including the dependent do not count as allowed imports
 
     # nodes to exclude are nodes that once reached will not have their submodules analysed next
     nodes_to_exclude = set()
     for dependent in dependents:
         if dependent == dependent_upon:
             continue
-        nodes_to_exclude.update(_get_all_submodules_of(graph, dependent))
+        nodes_to_exclude.update(get_all_submodules_of(graph, dependent))
 
     nodes_fulfilling_criteria = []
 
     # nodes that count as not fulfilling the criterion are nodes that would technically fulfill the criterion,
     # but have to be excluded for consistency reasons. For example, if the dependent upon is called A and has two
     # submodules A.X and A.Y. If A.X and A.Y import each other, this would be registered as fulfilling the
     # requirement of a module other than the dependents (assuming that A.X and A.Y are not in this list).
     # however, this is not really an import by a module outside A, which is what we are actually looking for
 
     # submodules of the dependent upon do not count as allowed imports e.g. if they import each other
-    nodes_that_count_as_not_fulfilling_criterion = _get_all_submodules_of(
+    nodes_that_count_as_not_fulfilling_criterion = get_all_submodules_of(
         graph, dependent_upon
     )
 
     if dependent_upon.parent_module is not None:
         # if the dependent upon module is defined via a parent module, this parent module is not included in the
         # list of modules that do not fulfill the criteria - only its true submodules are
         # reason: there is a dependency from the parent module to the child module, but this is not an import
@@ -161,29 +160,28 @@
             continue
 
         checked_nodes.add(node)
 
         parents = graph.direct_predecessor_nodes(node)
 
         for parent in parents:
-
             if not graph.parent_child_relationship(parent, node):
                 if (
                     parent not in nodes_to_exclude
                     and parent not in nodes_that_count_as_not_fulfilling_criterion
                 ):
                     nodes_fulfilling_criteria.append(tuple(to_modules([parent, node])))
 
                 if parent not in nodes_to_exclude:
                     nodes_to_check.append(parent)
 
     return nodes_fulfilling_criteria  # type: ignore
 
 
-def _get_all_submodules_of(graph: AbstractGraph, module: Module) -> Set[AbstractNode]:
+def get_all_submodules_of(graph: AbstractGraph, module: Module) -> Set[AbstractNode]:
     """Returns all submodules of a given module.
 
     Args:
         module: module to retrieve submodules of
 
     Returns:
         all submodules, including the module itself
```

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure/evaluable_structures.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure/evaluable_structures.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure/networkxgraph.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure/networkxgraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from typing import Any, Dict, List, Optional, Tuple
 
 import networkx as nx
 from networkx import draw_networkx, has_path, spring_layout
 
 from pytestarch.eval_structure.evaluable_structures import AbstractGraph, AbstractNode
-from pytestarch.eval_structure.types import Import
+from pytestarch.eval_structure.types import Import, get_parent_modules
 
 EXPECTED_EDGE_AND_NODE_TYPES = "Only str and tuple of two str supported."
 
 
 Node = AbstractNode
 
 
@@ -73,27 +73,33 @@
             ):
                 self._create_edge(parent, child, inherits=True)
 
     def _add_all_modules_as_nodes(self) -> None:
         for module in self._all_modules:
             self._create_node(module)
 
+            self._add_edges_within_module_hierarchy(
+                get_parent_modules(module),
+                module,
+            )
+
     def _add_edges_within_module_hierarchy(
         self,
         parent_modules: List[Node],
         child: Node,
     ) -> None:
         """Create edges between a node and its parent recursively until the parent-less parent is reached.
 
         Args:
             parent_modules: list of all parent modules in order, last element is the direct parent of the child module
             child: lowest element in the module hierarchy
         """
         all_modules = parent_modules + [child]
         for parent, child in zip(all_modules[:-1], all_modules[1:]):
+            self._create_node(parent)
             self._create_edge(parent, child, inherits=True)
 
     def _create_node(self, node: Node) -> None:
         """Create a node in the dependency graph.
         Args:
             node: to add to the graph
         """
@@ -123,15 +129,15 @@
         # in order to not add a function/class to the eval_structure, an ende to
         # foo.bar will only be added if both importer
         # and importee are already part of the eval_structure (which they will
         # be if they correspond to modules in the file system
         if (
             self._graph.has_node(node_start)
             and self._graph.has_node(node_end)
-            and not self._graph.has_edge(node_start, node_end)
+            and not self._edge_already_present(node_start, node_end, inherits)
         ):
             self._graph.add_edge(node_start, node_end, inherits=inherits)
 
     def __contains__(self, item) -> bool:
         if not isinstance(item, (str, tuple)):
             raise TypeError(EXPECTED_EDGE_AND_NODE_TYPES)
 
@@ -294,7 +300,15 @@
         # base module: src
         # children: src.A, src.B
         # not to be included: src.A.a, src.A.aa, src.B.b, ...
         # logic: include at most level "." in the node name
 
         node_parts = node.split(".")
         return ".".join(node_parts[: self._level_limit + 1])
+
+    def _edge_already_present(
+        self, node_start: Node, node_end: Node, inherits: bool
+    ) -> bool:
+        if not self._graph.has_edge(node_start, node_end):
+            return False
+
+        return self.parent_child_relationship(node_start, node_end) == inherits
```

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure/types.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 
 
 class Import(ABC):
     def __init__(self, importer: str) -> None:
         self._importer = importer
 
-        self._importer_module_hierarchy = self._get_parent_modules(self._importer)
+        self._importer_module_hierarchy = get_parent_modules(self._importer)
 
     def importer(self) -> str:
         """Returns name of the module that imports something.
 
         Returns:
             module name
         """
@@ -43,34 +43,35 @@
             list of module names
         """
         raise NotImplementedError()
 
     def __str__(self) -> str:
         return f"{self.importer()} imports {self.importee()}"
 
-    def _get_parent_modules(self, module: str) -> List[str]:
-        """Calculates all parent modules of a given module.
+    def _append_prefix(self, value: str, prefix: str) -> str:
+        return f"{prefix}.{value}"
 
-        Example: source root is a
-        module: a.b.c
-        returned: [a, a.b]
 
-        Args:
-            module: module to calculate parent modules for
+def get_parent_modules(module: str) -> List[str]:
+    """Calculates all parent modules of a given module.
 
-        Returns:
-            List of all parent modules, containing their full names up to the source code root.
-        """
-        parent_modules = []
+    Example: source root is a
+    module: a.b.c
+    returned: [a, a.b]
 
-        parent: List[str] = []
+    Args:
+        module: module to calculate parent modules for
 
-        for char in module:
-            if char == ".":
-                parent_modules.append("".join(parent))
+    Returns:
+        List of all parent modules, containing their full names up to the source code root.
+    """
+    parent_modules = []
 
-            parent.append(char)
+    parent: List[str] = []
 
-        return parent_modules
+    for char in module:
+        if char == ".":
+            parent_modules.append("".join(parent))
 
-    def _append_prefix(self, value: str, prefix: str) -> str:
-        return f"{prefix}.{value}"
+        parent.append(char)
+
+    return parent_modules
```

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure/utils.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure/utils.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/converter.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/import_filter.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/import_filter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/import_types.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/import_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import ast
 from dataclasses import dataclass
 from typing import List, Optional
 
-from pytestarch.eval_structure.types import Import
+from pytestarch.eval_structure.types import Import, get_parent_modules
 from pytestarch.eval_structure_generation.file_import.exceptions import ImportException
 
 
 @dataclass
 class NamedModule:
     """Contains an ast module with its name.
 
@@ -23,15 +23,15 @@
 
 class AbsoluteImport(Import):
     """Represents an absolute import."""
 
     def __init__(self, importer: str, module_name: str) -> None:
         super().__init__(importer)
         self._module_name = module_name
-        self._importee_module_hierarchy = self._get_parent_modules(self._module_name)
+        self._importee_module_hierarchy = get_parent_modules(self._module_name)
 
     def importee(self) -> str:
         return self._module_name
 
     def importee_parent_modules(self) -> List[str]:
         return self._importee_module_hierarchy
 
@@ -53,15 +53,15 @@
         if module_name is None and import_name is None:
             raise ImportException(
                 "Either name of module of of import needs to be specified."
             )
 
         self._importee = self._calculate_importee()
 
-        self._importee_module_hierarchy = self._get_parent_modules(self._module_name)
+        self._importee_module_hierarchy = get_parent_modules(self._module_name)
 
     def importee(self) -> str:
         return self._importee
 
     def importee_parent_modules(self) -> List[str]:
         return self._importee_module_hierarchy
```

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure_generation/file_import/parser.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/file_import/parser.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py` & `pytestarch-1.4.0/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,16 @@
 
 
 def _get_internal_module_prefix(
     path_diff_between_root_and_module: str, root_path: Path
 ) -> str:
     """In general, all internal modules should start with the root module name to be able to differentiate between
     internal and external modules. If the root and base module differ, the modules between them also need to be taken
-    into account, as not root.a.b modules are external, but root.a.b.base are internal."""
+    into account, as not root.a.b modules are external, but root.a.b.base are internal.
+    """
     internal_module_prefix = root_path.name + "."
 
     if path_diff_between_root_and_module != ".":
         internal_module_prefix += path_diff_between_root_and_module
 
     return internal_module_prefix
```

### Comparing `pytestarch-1.3.1/src/pytestarch/pytestarch.py` & `pytestarch-1.4.0/src/pytestarch/pytestarch.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,64 +9,87 @@
 from types import ModuleType
 from typing import Optional, Tuple
 
 from pytestarch import EvaluableArchitecture
 from pytestarch.eval_structure_generation.graph_generation.graph_generator import (
     generate_graph,
 )
+from pytestarch.query_language.exceptions import ImproperlyConfigured
+from pytestarch.utils.partial_match_to_regex_converter import (
+    convert_partial_match_to_regex,
+)
 
-DEFAULT_EXCLUSIONS = ("*__pycache__",)
+DEFAULT_EXCLUSIONS = ("*__pycache__*",)
 
 
 def get_evaluable_architecture(
     root_path: str,
     module_path: str,
     exclusions: Tuple[str, ...] = DEFAULT_EXCLUSIONS,
     exclude_external_libraries: bool = True,
     level_limit: Optional[int] = None,
+    regex_exclusions: Optional[Tuple[str, ...]] = None,
 ) -> EvaluableArchitecture:
     """Constructs an evaluable object based on the given module.
 
     Args:
         root_path: root directory of the source code. Should not be set to a submodule of the top level module.
         module_path: path of module to generate the evaluable for. Must be a submodule of the root_path module.
         exclusions: pseudo-regex to exclude files and directories from being integrated into the evaluable, e.g. *Test.py
         exclude_external_libraries: if True, external dependencies (defined as all dependencies to module outside the
             module_path, including Python built-in modules) will not be taken into account for the dependency analysis.
+            Can only be specified if regex_exclusions is not specified.
         level_limit: if not None, specifies the depth of the graph. For example, a limit of 1 will result in only the
             modules one level below the module path to be added as nodes. Note that this only applies to the final graph;
             all modules will be parsed, the graph will simply be flattened: if a submodule of X imports Y, this import is
             then assigned to X instead, if Y is above the level limit.
+        regex_exclusions: Proper regex version of 'exclusions'. Can only be specified if regex_exclusions is not specified.
     """
+    if regex_exclusions and exclusions:
+        raise ImproperlyConfigured(
+            "Partial match exclusions and regex exclusions cannot both be specified."
+        )
+
+    if exclusions:
+        regex_exclusions = [
+            convert_partial_match_to_regex(pattern) for pattern in exclusions
+        ]
+
     root_path = Path(root_path)
     module_path = Path(module_path)
 
     path_diff_between_root_and_module = str(module_path.relative_to(root_path)).replace(
         os.sep, "."
     )
 
     return generate_graph(
         root_path,
         module_path,
         path_diff_between_root_and_module,
-        exclusions,
+        regex_exclusions,
         exclude_external_libraries,
         level_limit,
     )
 
 
 def get_evaluable_architecture_for_module_objects(
     root_module: ModuleType,
     module: ModuleType,
     exclusions: Tuple[str, ...] = DEFAULT_EXCLUSIONS,
     exclude_external_libraries: bool = True,
     level_limit: Optional[int] = None,
+    regex_exclusions: Optional[Tuple[str, ...]] = None,
 ) -> EvaluableArchitecture:
     """Same functionality as get_evaluable_architecture, but root module and module to evaluate are passed in as module objects
     instead of the absolute paths to them.
     """
     root_path = os.path.dirname(root_module.__file__)
     module_path = os.path.dirname(module.__file__)
 
     return get_evaluable_architecture(
-        root_path, module_path, exclusions, exclude_external_libraries, level_limit
+        root_path,
+        module_path,
+        exclusions,
+        exclude_external_libraries,
+        level_limit,
+        regex_exclusions,
     )
```

### Comparing `pytestarch-1.3.1/src/pytestarch/query_language/multiple_rule_applier.py` & `pytestarch-1.4.0/src/pytestarch/query_language/multiple_rule_applier.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.3.1/src/pytestarch/query_language/rule.py` & `pytestarch-1.4.0/src/pytestarch/query_language/rule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, replace
-from typing import Callable, List, Optional, Type, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 from pytestarch import EvaluableArchitecture
 from pytestarch.eval_structure.evaluable_architecture import Module
 from pytestarch.query_language.base_language import (
     BehaviorSpecification,
     DependencySpecification,
     RuleApplier,
@@ -18,19 +18,23 @@
     BehaviorRequirement,
 )
 from pytestarch.rule_assessment.rule_check.module_requirement import ModuleRequirement
 from pytestarch.rule_assessment.rule_check.rule_matcher import (
     DefaultRuleMatcher,
     RuleMatcher,
 )
+from pytestarch.utils.decorators import deprecated
+from pytestarch.utils.partial_match_to_regex_converter import (
+    convert_partial_match_to_regex,
+)
 
 
 @dataclass
 class RuleConfiguration:
-    module_to_check: Optional[Module] = None
+    modules_to_check: Optional[List[Module]] = None
     modules_to_check_against: Optional[List[Module]] = None
     should: bool = False
     should_only: bool = False
     should_not: bool = False
     except_present: bool = False
     import_: bool = None
     rule_object_anything: bool = False
@@ -45,23 +49,26 @@
     RuleApplier,
 ):
     """Represents an architectural rule of the form
     Module1 [verb, such as 'should'] [import type, such as 'import'] Module2
     """
 
     def __init__(
-        self, rule_matcher_class: Type[RuleMatcher] = DefaultRuleMatcher
+        self,
+        rule_matcher_class: Callable[
+            [ModuleRequirement, BehaviorRequirement], RuleMatcher
+        ] = DefaultRuleMatcher,
     ) -> None:
         self._rule_matcher_class = rule_matcher_class
         self._modules_to_check_to_be_specified_next = None
         self._configuration = RuleConfiguration()
 
     @property
-    def rule_subject(self) -> Optional[Module]:
-        return self._configuration.module_to_check
+    def rule_subjects(self) -> Optional[List[Module]]:
+        return self._configuration.modules_to_check
 
     def modules_that(self) -> RuleSubject:
         self._modules_to_check_to_be_specified_next = True
         return self
 
     def are_sub_modules_of(
         self, modules: Union[str, List[str]]
@@ -69,46 +76,77 @@
         self._set_modules(modules, lambda name: Module(parent_module=name))
         return self
 
     def are_named(self, names: Union[str, List[str]]) -> BehaviorSpecification:
         self._set_modules(names, lambda name: Module(name=name))
         return self
 
+    @deprecated
     def have_name_containing(
         self, partial_names: Union[str, List[str]]
     ) -> BehaviorSpecification:
         self._set_modules(
-            partial_names, lambda name: Module(name=name, partial_match=True)
+            partial_names,
+            lambda name: Module(name=convert_partial_match_to_regex(name), regex=True),
         )
         return self
 
+    def have_name_matching(
+        self,
+        regex: str,
+    ) -> BehaviorSpecification:
+        self._set_modules(regex, lambda name: Module(name=name, regex=True))
+        return self
+
     def _set_modules(
         self,
         module_names: Union[str, List[str]],
         create_module_fn: Callable[[str], Module],
     ) -> None:
         if self._modules_to_check_to_be_specified_next is None:
             raise ImproperlyConfigured("Specify a RuleSubject or RuleObject first.")
 
-        if self._modules_to_check_to_be_specified_next and isinstance(
-            module_names, list
-        ):
-            raise ImproperlyConfigured("Only rule subjects can be specified in batch.")
-
-        if not self._modules_to_check_to_be_specified_next and isinstance(
-            module_names, str
-        ):
+        if isinstance(module_names, str):
             module_names = [module_names]
 
+        modules = [create_module_fn(n) for n in module_names]
         if self._modules_to_check_to_be_specified_next:
-            self._configuration.module_to_check = create_module_fn(module_names)  # type: ignore
+            self._configuration.modules_to_check = modules
         else:
-            self._configuration.modules_to_check_against = [
-                create_module_fn(n) for n in module_names
-            ]
+            self._configuration.modules_to_check_against = modules
+
+    def _add_modules(self, modules: List[Tuple[str, bool]]) -> BehaviorSpecification:
+        module_names = []
+        module_creation_fn = []
+
+        for module, name_is_regex in modules:
+            module_names.append(module)
+            module_creation_fn.append(
+                lambda name: Module(name=name, regex=name_is_regex)
+            )
+
+        self._append_modules(module_names, module_creation_fn)
+        return self
+
+    def _append_modules(
+        self,
+        module_names: List[str],
+        create_module_fns: List[Callable[[str], Module]],
+    ) -> None:
+        modules = [fn(n) for n, fn in zip(module_names, create_module_fns)]
+        if self._modules_to_check_to_be_specified_next:
+            if self._configuration.modules_to_check is None:
+                self._configuration.modules_to_check = []
+
+            self._configuration.modules_to_check.extend(modules)
+        else:
+            if self._configuration.modules_to_check_against is None:
+                self._configuration.modules_to_check_against = []
+
+            self._configuration.modules_to_check_against.extend(modules)
 
     def should(self) -> DependencySpecification:
         self._configuration.should = True
         return self
 
     def should_only(self) -> DependencySpecification:
         self._configuration.should_only = True
@@ -155,15 +193,15 @@
         self._assert_required_configuration_present()
 
         matcher = self._prepare_rule_matcher()
         matcher.match(evaluable)
 
     def _prepare_rule_matcher(self) -> RuleMatcher:
         module_requirement = ModuleRequirement(
-            self._configuration.module_to_check,
+            self._configuration.modules_to_check,
             self._configuration.modules_to_check_against,
             self._configuration.import_,
         )
         behavior_requirement = BehaviorRequirement(
             self._configuration.should,
             self._configuration.should_only,
             self._configuration.should_not,
@@ -175,44 +213,55 @@
     def __str__(self) -> str:
         self._assert_required_configuration_present()
 
         method_name = f'{"should" if self._configuration.should else "should only" if self._configuration.should_only else "should not"}'
 
         subject_prefix = (
             "Sub modules of "
-            if self._configuration.module_to_check.parent_module is not None
+            if self._configuration.modules_to_check[0].parent_module is not None
             else ""
         )
         if self._configuration.rule_object_anything:
             object_message = "anything "
         else:
             object_message = f'modules that are {"named" if self._configuration.modules_to_check_against[0].name is not None else "sub modules of"} '
 
+        combined_rule_subjects = self._combine_names(
+            self._configuration.modules_to_check
+        )
+        combined_rule_objects = self._combine_names(
+            self._configuration.modules_to_check_against
+        )
         return (
-            f'{subject_prefix}"{self._get_module_name(self._configuration.module_to_check)}" '
+            f'{subject_prefix}"{combined_rule_subjects}" '
             f"{method_name} "
             f'{"import" if self._configuration.import_ else "be imported by"} '
             f'{"modules except " if self._configuration.except_present else ""}'
             f"{object_message}"
-            f'"{", ".join(sorted(map(lambda module: self._get_module_name(module), self._configuration.modules_to_check_against)))}".'
+            f'"{combined_rule_objects}".'
+        )
+
+    def _combine_names(self, modules: list[Module]) -> str:
+        return ", ".join(
+            sorted(map(lambda module: self._get_module_name(module), modules))
         )
 
     def _get_module_name(self, module: Module) -> str:
         return module.name if module.name is not None else module.parent_module
 
     def _assert_required_configuration_present(self) -> None:
         behavior_missing = not any(
             [
                 self._configuration.should,
                 self._configuration.should_only,
                 self._configuration.should_not,
             ]
         )
         dependency_missing = self._configuration.import_ is None
-        subject_missing = not self._configuration.module_to_check
+        subject_missing = not self._configuration.modules_to_check
         object_missing = not self._configuration.modules_to_check_against
 
         if any([behavior_missing, dependency_missing, subject_missing, object_missing]):
             subject_message = self._name_or_empty(subject_missing, RuleSubject)
             behavior_message = self._name_or_empty(
                 behavior_missing, BehaviorSpecification
             )
@@ -249,13 +298,46 @@
     @classmethod
     def _convert_aliases(cls, configuration: RuleConfiguration) -> RuleConfiguration:
         if not configuration.rule_object_anything:
             return configuration
 
         # should not import anything is equivalent to should not import except itself
         # should not be imported by anything is equivalent to should not be imported by anything except itself
+
+        modules_to_check_without_parent_and_submodule_combinations = (
+            cls._get_modules_to_check_without_parent_and_submodule_combinations(
+                configuration,
+            )
+        )
+
         return replace(
             configuration,
             rule_object_anything=False,
-            modules_to_check_against=[configuration.module_to_check],
+            modules_to_check=modules_to_check_without_parent_and_submodule_combinations,
+            modules_to_check_against=modules_to_check_without_parent_and_submodule_combinations,
             except_present=True,
         )
+
+    @classmethod
+    def _get_modules_to_check_without_parent_and_submodule_combinations(
+        cls, configuration: RuleConfiguration
+    ) -> Optional[List[Module]]:
+        # if modules_to_check contain a module and its submodule, this can throw off the breadth first search conducted
+        # on the dependency graph - and also, this setup does not really make sense
+        if configuration.modules_to_check is None:
+            return None
+
+        module_names = sorted(
+            map(lambda module: module.name, configuration.modules_to_check)
+        )
+
+        result = []
+        for module in configuration.modules_to_check:
+            parent_module_found = False
+            for module_name in module_names:
+                if module_name in module.name and module.name != module_name:
+                    parent_module_found = True
+
+            if not parent_module_found:
+                result.append(module)
+
+        return result
```

### Comparing `pytestarch-1.3.1/src/pytestarch/rule_assessment/rule_check/module_requirement.py` & `pytestarch-1.4.0/src/pytestarch/rule_assessment/rule_check/module_requirement.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from __future__ import annotations
 
-from typing import List, Union
+from typing import List
 
 from pytestarch.eval_structure.evaluable_architecture import Module
 
 
 class ModuleRequirement:
     """Stores information about which module is supposed to be checked against which module."""
 
     def __init__(
         self,
-        importer: Module,
+        importers: List[Module],
         importees: List[Module],
-        flip_importer_and_importees: bool,
+        importer_specified_as_rule_subject: bool,
     ) -> None:
-        self._importer_as_specified_by_user = importer
+        self._importer_as_specified_by_user = importers
         self._importees_as_specified_by_user = importees
 
-        self._importers = importer
+        self._importers = importers
         self._importees = importees
 
-        self._flip_importer_and_importees = flip_importer_and_importees
+        self._importer_specified_as_rule_subject = importer_specified_as_rule_subject
 
         if self.rule_specified_with_importer_as_rule_object:
             self._importers, self._importees = (
                 self._importees,
                 self._importers,
             )
 
     @property
-    def importers(self) -> Union[Module, List[Module]]:
+    def importers(self) -> List[Module]:
         return self._importers
 
     @property
-    def importees(self) -> Union[Module, List[Module]]:
+    def importees(self) -> List[Module]:
         return self._importees
 
     @property
-    def importers_as_specified_by_user(self) -> Module:
+    def importers_as_specified_by_user(self) -> list[Module]:
         return self._importer_as_specified_by_user
 
     @property
-    def importees_as_specified_by_user(self) -> Union[Module, List[Module]]:
+    def importees_as_specified_by_user(self) -> List[Module]:
         return self._importees_as_specified_by_user
 
     @property
     def rule_specified_with_importer_as_rule_object(self) -> bool:
         # True if rule is of format "is imported by"
-        return not self._flip_importer_and_importees
+        return not self._importer_specified_as_rule_subject
 
     @property
     def rule_specified_with_importer_as_rule_subject(self) -> bool:
-        # True if rule is of format "is imported by"
-        return self._flip_importer_and_importees
+        # True if rule is of format "imports"
+        return self._importer_specified_as_rule_subject
```

### Comparing `pytestarch-1.3.1/setup.py` & `pytestarch-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,28 @@
  'pytestarch.eval_structure',
  'pytestarch.eval_structure_generation',
  'pytestarch.eval_structure_generation.file_import',
  'pytestarch.eval_structure_generation.graph_generation',
  'pytestarch.query_language',
  'pytestarch.rule_assessment',
  'pytestarch.rule_assessment.error_message',
- 'pytestarch.rule_assessment.rule_check']
+ 'pytestarch.rule_assessment.rule_check',
+ 'pytestarch.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['matplotlib>=3.5.3,<4.0.0', 'networkx>=3.0,<4.0']
+['b2>=3.7.1,<4.0.0', 'matplotlib>=3.5.3,<4.0.0', 'networkx>=3.0,<4.0']
 
 setup_kwargs = {
     'name': 'pytestarch',
-    'version': '1.3.1',
+    'version': '1.4.0',
     'description': 'Test framework for software architecture based on imports between modules',
-    'long_description': '# Welcome to PyTestArch\n\nPyTestArch is an open source library that allows users to define architectural rules and test their code against them. It is \ngenerally inspired by [ArchUnit](https://www.archunit.org/).\n\n## Installation Guide\nPyTestArch is available via [PyPI](https://pypi.org/project/pytestarch/) and can be installed e.g. via pip: `pip install pytestarch`.\n\n## Usage Guide\nThree steps are required to test an architectural rule:\n\n1) Create an evaluable representation of the source code you want to test\n\n```\nfrom pytestarch.pytestarch import get_evaluable_architecture\n\nevaluable = get_evaluable_architecture("/home/dummy/project", "/home/dummy/project/src")\n```\nThis will scan all python files under /home/dummy/project/src for imports and build an internal representation that can\nlater be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external \ndependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),\nyou could use a fixture for this evaluable object.\n\n2) Define an architectural rule\n```\nfrom pytestarch.query_language.base_language import Rule\n\nrule = Rule()\n        .modules_that()\n        .are_named("src.moduleB")\n        .should_not()\n        .be_imported_by_modules_that()\n        .are_sub_modules_of("src.moduleA"),\n```\n\nThis rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module\nthat is a submodule of "src.moduleA", excluding "src.moduleA" itself.\n\n3) Evaluate your code against this rule\n\n```\nrule.assert_applies(evaluable)\n```\nThat\'s it!\n',
+    'long_description': '# Welcome to PyTestArch\n\nPyTestArch is an open source library that allows users to define architectural rules and test their code against them. It is \ngenerally inspired by [ArchUnit](https://www.archunit.org/).\n\n## Installation Guide\nPyTestArch is available via [PyPI](https://pypi.org/project/pytestarch/) and can be installed e.g. via pip: `pip install pytestarch`.\n\n## Usage Guide\nThree steps are required to test an architectural rule:\n\n1) Create an evaluable representation of the source code you want to test\n\n```\nfrom pytestarch.pytestarch import get_evaluable_architecture\n\nevaluable = get_evaluable_architecture("/home/dummy/project", "/home/dummy/project/src")\n```\nThis will scan all python files under /home/dummy/project/src for imports and build an internal representation that can\nlater be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external \ndependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),\nyou could use a fixture for this evaluable object.\n\n2) Define an architectural rule\n```\nfrom pytestarch. import Rule\n\nrule = Rule() \\\n        .modules_that() \\\n        .are_named("src.moduleB") \\\n        .should_not() \\\n        .be_imported_by_modules_that() \\\n        .are_sub_modules_of("src.moduleA") \\\n```\n\nThis rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module\nthat is a submodule of "src.moduleA", excluding "src.moduleA" itself.\n\n3) Evaluate your code against this rule\n\n```\nrule.assert_applies(evaluable)\n```\nThat\'s it!\n',
     'author': 'zyskarch',
     'author_email': 'zyskarch@gmail.com',
     'maintainer': 'zyskarch',
     'maintainer_email': 'zyskarch@gmail.com',
     'url': 'https://github.com/zyskarch/pytestarch',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pytestarch-1.3.1/PKG-INFO` & `pytestarch-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestarch
-Version: 1.3.1
+Version: 1.4.0
 Summary: Test framework for software architecture based on imports between modules
 Home-page: https://github.com/zyskarch/pytestarch
 License: Apache-2.0
 Keywords: architecture,test
 Author: zyskarch
 Author-email: zyskarch@gmail.com
 Maintainer: zyskarch
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Unit
+Requires-Dist: b2 (>=3.7.1,<4.0.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Project-URL: Bug Tracker, https://github.com/zyskarch/pytestarch/issues
 Project-URL: Documentation, https://zyskarch.github.io/pytestarch/
 Project-URL: Repository, https://github.com/zyskarch/pytestarch
 Description-Content-Type: text/markdown
 
@@ -52,22 +53,22 @@
 This will scan all python files under /home/dummy/project/src for imports and build an internal representation that can
 later be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external 
 dependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),
 you could use a fixture for this evaluable object.
 
 2) Define an architectural rule
 ```
-from pytestarch.query_language.base_language import Rule
+from pytestarch. import Rule
 
-rule = Rule()
-        .modules_that()
-        .are_named("src.moduleB")
-        .should_not()
-        .be_imported_by_modules_that()
-        .are_sub_modules_of("src.moduleA"),
+rule = Rule() \
+        .modules_that() \
+        .are_named("src.moduleB") \
+        .should_not() \
+        .be_imported_by_modules_that() \
+        .are_sub_modules_of("src.moduleA") \
 ```
 
 This rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module
 that is a submodule of "src.moduleA", excluding "src.moduleA" itself.
 
 3) Evaluate your code against this rule
```

