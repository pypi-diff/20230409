# Comparing `tmp/dash_component_editor-0.0.1.tar.gz` & `tmp/dash_component_editor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_component_editor-0.0.1.tar", last modified: Sat Apr  8 00:35:32 2023, max compression
+gzip compressed data, was "dash_component_editor-0.0.2.tar", last modified: Sun Apr  9 00:11:19 2023, max compression
```

## Comparing `dash_component_editor-0.0.1.tar` & `dash_component_editor-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-08 00:35:32.923714 dash_component_editor-0.0.1/
--rw-r--r--   0 zhuowen    (501) staff       (20)     2401 2023-03-27 16:49:46.000000 dash_component_editor-0.0.1/LICENSE.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)     1898 2023-04-08 00:35:32.923572 dash_component_editor-0.0.1/PKG-INFO
--rw-r--r--   0 zhuowen    (501) staff       (20)     1274 2023-04-07 23:27:26.000000 dash_component_editor-0.0.1/README.md
--rw-r--r--   0 zhuowen    (501) staff       (20)       38 2023-04-08 00:35:32.923764 dash_component_editor-0.0.1/setup.cfg
--rw-r--r--   0 zhuowen    (501) staff       (20)     1652 2023-04-08 00:35:09.000000 dash_component_editor-0.0.1/setup.py
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-08 00:35:32.922689 dash_component_editor-0.0.1/src/
-drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-08 00:35:32.923378 dash_component_editor-0.0.1/src/dash_component_editor.egg-info/
--rw-r--r--   0 zhuowen    (501) staff       (20)     1898 2023-04-08 00:35:32.000000 dash_component_editor-0.0.1/src/dash_component_editor.egg-info/PKG-INFO
--rw-r--r--   0 zhuowen    (501) staff       (20)      303 2023-04-08 00:35:32.000000 dash_component_editor-0.0.1/src/dash_component_editor.egg-info/SOURCES.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)        1 2023-04-08 00:35:32.000000 dash_component_editor-0.0.1/src/dash_component_editor.egg-info/dependency_links.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)       75 2023-04-08 00:35:32.000000 dash_component_editor-0.0.1/src/dash_component_editor.egg-info/requires.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)       22 2023-04-08 00:35:32.000000 dash_component_editor-0.0.1/src/dash_component_editor.egg-info/top_level.txt
--rw-r--r--   0 zhuowen    (501) staff       (20)    15043 2023-04-08 00:04:50.000000 dash_component_editor-0.0.1/src/dash_component_editor.py
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-09 00:11:19.335972 dash_component_editor-0.0.2/
+-rw-r--r--   0 zhuowen    (501) staff       (20)     2401 2023-03-27 16:49:46.000000 dash_component_editor-0.0.2/LICENSE.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)     2816 2023-04-09 00:11:19.335799 dash_component_editor-0.0.2/PKG-INFO
+-rw-r--r--   0 zhuowen    (501) staff       (20)     2192 2023-04-08 23:59:48.000000 dash_component_editor-0.0.2/README.md
+-rw-r--r--   0 zhuowen    (501) staff       (20)       38 2023-04-09 00:11:19.336075 dash_component_editor-0.0.2/setup.cfg
+-rw-r--r--   0 zhuowen    (501) staff       (20)     1644 2023-04-09 00:10:35.000000 dash_component_editor-0.0.2/setup.py
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-09 00:11:19.334738 dash_component_editor-0.0.2/src/
+drwxr-xr-x   0 zhuowen    (501) staff       (20)        0 2023-04-09 00:11:19.335569 dash_component_editor-0.0.2/src/dash_component_editor.egg-info/
+-rw-r--r--   0 zhuowen    (501) staff       (20)     2816 2023-04-09 00:11:19.000000 dash_component_editor-0.0.2/src/dash_component_editor.egg-info/PKG-INFO
+-rw-r--r--   0 zhuowen    (501) staff       (20)      303 2023-04-09 00:11:19.000000 dash_component_editor-0.0.2/src/dash_component_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)        1 2023-04-09 00:11:19.000000 dash_component_editor-0.0.2/src/dash_component_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)       75 2023-04-09 00:11:19.000000 dash_component_editor-0.0.2/src/dash_component_editor.egg-info/requires.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)       22 2023-04-09 00:11:19.000000 dash_component_editor-0.0.2/src/dash_component_editor.egg-info/top_level.txt
+-rw-r--r--   0 zhuowen    (501) staff       (20)    15043 2023-04-08 00:04:50.000000 dash_component_editor-0.0.2/src/dash_component_editor.py
```

### Comparing `dash_component_editor-0.0.1/LICENSE.txt` & `dash_component_editor-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash_component_editor-0.0.1/PKG-INFO` & `dash_component_editor-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-Metadata-Version: 2.1
-Name: dash_component_editor
-Version: 0.0.1
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: Zhuowen Zhao, Ronald Pandolfi
-Author-email: zwenzhao11@gmail.com
-License: UNKNOWN
-Project-URL: Source, https://github.com/mlexchange/mlex_dash_component_editor.git
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Dash
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # MLExchange Dash component editor
-This script creates adaptive Dash GUI component from keywords (JSON format data).
+This script creates adaptive Dash GUI components from keyword pairs (JSON format).
+
+It currently supports 8 types of Dash GUI components: 3 types of [input forms](https://dash-bootstrap-components.opensource.faculty.ai/docs/components/input/) (int, float, str), [slider](https://dash.plotly.com/dash-core-components/slider), [dropdown](https://dash.plotly.com/dash-core-components/dropdown), [radio items](https://dash.plotly.com/dash-core-components/radioitems), [boolean toggle switch](https://dash.plotly.com/dash-daq/toggleswitch), and [image](https://dash.plotly.com/dash-html-components/img). The corresponding keyword values are 'int', 'float', 'str', 'slider', 'dropdown', 'radio', 'bool', and 'img'.
+
+Legal keyword pairs: {'type': xxx, 'name': xxx, 'title': xxx, 'param_key': xxx, 'value': xxx} and all the other legal keyword pairs in the corresponding Dash components. **Note**: 'name' is the unique string identifier.
+
+
 
-Dependency: dash==2.9.0
+## Dependencies:
+
+```
+dash>=2.9.0,
+dash_daq==0.5.0,
+dash_bootstrap_components>=1.0.0,
+werkzeug==2.0
+```
 
 
 ## Code example
 
 ```python
 from dash import Dash, html
 from dash_component_editor import JSONParameterEditor
-import json
 
 # data
 component_kwargs = {"gui_parameters": [{"type": "int", "name": "num-tree", "title": "Number of Trees", "param_key": "n_estimators", "value": "30"}, 
                                        {"type": "int", "name": "tree-depth", "title": "Tree Depth", "param_key": "max_depth", "value": "8"}]}
 
 
 # Set up Dash server and web layouts
@@ -54,9 +47,7 @@
                                 )
     item_list.init_callbacks(app)
     
     return [html.H5("GUI Layout", className="card-title"), item_list]
 ```
 
 
-
-
```

### Comparing `dash_component_editor-0.0.1/setup.py` & `dash_component_editor-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dash_component_editor",                     # This is the name of the package
-    version="0.0.1",                        # The initial release version
+    version="0.0.2",                        # The release version
     author="Zhuowen Zhao, Ronald Pandolfi",                     # Full name of the author
     author_email='zwenzhao11@gmail.com',
     description="",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     license_files = ('LICENSE.txt',),                                     # Information to filter the project on PyPi website
```

### Comparing `dash_component_editor-0.0.1/src/dash_component_editor.py` & `dash_component_editor-0.0.2/src/dash_component_editor.py`

 * *Files identical despite different names*

