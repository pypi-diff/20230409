# Comparing `tmp/py_yprinciple_gen-0.2.6.tar.gz` & `tmp/py_yprinciple_gen-0.2.7.tar.gz`

## Comparing `py_yprinciple_gen-0.2.6.tar` & `py_yprinciple_gen-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/.pydevproject
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/scripts/install
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/tests/basemwtest.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/tests/basesmwtest.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/tests/basetest.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/tests/test_editor.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/tests/test_python.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/tests/test_smw.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/tests/test_smw_generate.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/__init__.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/editor.py
--rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/genapi.py
--rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/gengrid.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/profiler.py
--rw-r--r--   0        0        0    22327 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/smw_targets.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/target.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/version.py
--rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/ypcell.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/ypgen.py
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/ypgenapp.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/yprinciple/resources/static/css/md_style_indigo.css
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/LICENSE
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/README.md
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.pydevproject
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.github/workflows/upload-to-pypi.yml
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/scripts/install
+-rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/basemwtest.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/basesmwtest.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/basetest.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/test_editor.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/test_python.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/test_smw.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/tests/test_smw_generate.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/__init__.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/editor.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/genapi.py
+-rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/gengrid.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/profiler.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/push.py
+-rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/smw_targets.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/target.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/version.py
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/ypcell.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/ypgen.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/ypgenapp.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/yprinciple/resources/static/css/md_style_indigo.css
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/README.md
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.7/PKG-INFO
```

### Comparing `py_yprinciple_gen-0.2.6/.github/workflows/build.yml` & `py_yprinciple_gen-0.2.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/.github/workflows/upload-to-pypi.yml` & `py_yprinciple_gen-0.2.7/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/scripts/test` & `py_yprinciple_gen-0.2.7/scripts/test`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/tests/basemwtest.py` & `py_yprinciple_gen-0.2.7/tests/basemwtest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/tests/basesmwtest.py` & `py_yprinciple_gen-0.2.7/tests/basesmwtest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/tests/basetest.py` & `py_yprinciple_gen-0.2.7/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/tests/test_editor.py` & `py_yprinciple_gen-0.2.7/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/tests/test_smw.py` & `py_yprinciple_gen-0.2.7/tests/test_smw.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/tests/test_smw_generate.py` & `py_yprinciple_gen-0.2.7/tests/test_smw_generate.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/editor.py` & `py_yprinciple_gen-0.2.7/yprinciple/editor.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/genapi.py` & `py_yprinciple_gen-0.2.7/yprinciple/genapi.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/gengrid.py` & `py_yprinciple_gen-0.2.7/yprinciple/gengrid.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/profiler.py` & `py_yprinciple_gen-0.2.7/yprinciple/profiler.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/smw_targets.py` & `py_yprinciple_gen-0.2.7/yprinciple/smw_targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,16 @@
 end note
 note as {topic.name}Note
 {topic.documentation}
 end note
 class {topic.name} {{
 """
         for prop in topic.properties.values():
-            markup+=f"  {prop.type} {prop.name}\n"
+            prop_type=getattr(prop,"type","Text")
+            markup+=f"  {prop_type} {prop.name}\n"
         markup+=f"""}}
 {topic.name}Note .. {topic.name}
 """
         # Relations/Topic Links        
         for topicLink in topic.sourceTopicLinks.values(): 
             markup+=f"{self.plantUmlRelation(topicLink)}"
         for topicLink in topic.targetTopicLinks.values(): 
@@ -363,16 +364,17 @@
         for prop in topic.propertiesByIndex():
             values_from_key="values from="
             if prop.isLink:
                 prop.values_from=f"{prop.topicLink.source}"
                 prop.inputType="dropdown"
                 values_from_key="values from concept="
                 pass
+            prop_type=getattr(prop,"type","Text")
             markup+=f"""! {prop.label}:
-<!-- {prop.type} {prop.name} -->\n"""
+<!-- {prop_type} {prop.name} -->\n"""
             inputType    =f"|input type={prop.inputType}"     if getattr(prop,"inputType",None) else ""
             if "textarea"==getattr(prop,"inputType",None):
                 inputType+="|editor=wikieditor"
             size         =f"|size={prop.size}"                if getattr(prop,"size",None) else ""
             mandatory    =f"|mandatory"                       if getattr(prop,"mandatory",None) else ""
             uploadable   =f"|uploadable"                      if getattr(prop,"uploadable",None) else ""
             size         =f"|size={prop.size}"                if getattr(prop,"size",None) else ""
@@ -532,18 +534,19 @@
 ! colspan='2' style='text-align:left' {{{{!}}}} {{{{Icon|name=edit|size=24}}}}{{{{Link|target=Special:FormEdit/{topic.name}/{{{{FULLPAGENAME}}}}|title=edit}}}}
 {{{{!}}}}-
 }}}}
 """
         for prop in topic.properties.values():
             # https://github.com/WolfgangFahl/py-yprinciple-gen/issues/13
             # show Links for external Identifiers in templates
-            if prop.type=="External identifier" or prop.isLink:
+            prop_type=getattr(prop,"type","Text")
+            if prop_type=="External identifier" or prop.isLink:
                 link_markup="→{{#show: {{FULLPAGENAME}}|"+f"?{topic.name} {prop.name}"+"}}"
                 pass
-            elif prop.type=="Page":           
+            elif prop_type=="Page":           
                 link_markup=f"→[[{{{{{{{prop.name}|}}}}}}]]"
             else:
                 link_markup=""
             markup+=f"""![[Property:{topic.name} {prop.name}|{prop.name}]]
 {{{{!}}}}&nbsp;{{{{#if:{{{{{{{prop.name}|}}}}}}|{{{{{{{prop.name}}}}}}}|}}}}{link_markup}
 {{{{!}}}}-\n"""
         markup+=f"{{{{!}}}}}}\n" # end of table
@@ -604,15 +607,16 @@
         topicWithConcept=f"Concept:{topic_name}"
         markup=f"""{{{{Property
 |name={prop.name}
 |label={prop.label} 
         """
         if hasattr(prop, "documentation"):
             markup+=f"""|documentation={prop.documentation}\n"""
-        markup+=f"""|type=Special:Types/{prop.type}
+        prop_type=getattr(prop,"type","Text")
+        markup+=f"""|type=Special:Types/{prop_type}
 """
         # @TODO read from metamodel
         for prop_name in ["index","sortPos","primaryKey","mandatory",
            "namespace","size","uploadable","defaultValue","inputType",
            "allowedValues","values_from","formatterURI","showInGrid","isLink"]:
             if hasattr(prop, prop_name):
                 value=getattr(prop,prop_name,None)
```

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/target.py` & `py_yprinciple_gen-0.2.7/yprinciple/target.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/version.py` & `py_yprinciple_gen-0.2.7/yprinciple/version.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/ypcell.py` & `py_yprinciple_gen-0.2.7/yprinciple/ypcell.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/ypgen.py` & `py_yprinciple_gen-0.2.7/yprinciple/ypgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 '''
 
 from argparse import ArgumentParser
 from argparse import RawDescriptionHelpFormatter
 from yprinciple.version import Version
 from yprinciple.ypgenapp import YPGenApp
 from yprinciple.genapi import GeneratorAPI
+from yprinciple.push import Push
 import os
 import sys
 import traceback
 import webbrowser
 # import after app!
 from jpcore.justpy_app import JustpyServer
 
@@ -43,16 +44,18 @@
         parser.add_argument("--targetPath", dest="targetPath", help="path for the files to be generated - uses wikibackup default path for wikiId if not specified", required=False)
         parser.add_argument("--sidif", help="path to SiDIF input file")
         parser.add_argument("-d", "--debug", dest="debug", action="store_true", help="show debug info [default: %(default)s]")
         parser.add_argument("-nd","--noDry", action="store_true", help="switch off dry run [default: %(default)s]")   
         parser.add_argument("--editor", action="store_true", help="open editor for results [default: %(default)s]")       
         parser.add_argument('--host',default=JustpyServer.getDefaultHost(),help="the host to serve / listen from [default: %(default)s]")
         parser.add_argument('--port',type=int,default=8778,help="the port to serve from [default: %(default)s]")
+        parser.add_argument("--push", action="store_true", help="push from source to target [default: %(default)s]")       
         parser.add_argument("--serve",help="start webserver",action="store_true")
-        parser.add_argument('--wikiId', default="wiki",help='id of the wiki to generate for [default: %(default)s]')
+        parser.add_argument('--wikiId',"-t","--target", default="wiki",help='id of the wiki to generate for [default: %(default)s]')
+        parser.add_argument('--source',"-s", default="profiwiki",help='id of the wiki to get concept and contexts (schemas) from [default: %(default)s]')
         parser.add_argument('-q', '--quiet', help="not verbose [default: %(default)s]" )
         parser.add_argument('-V', '--version', action='version', version=version_msg)
         return parser
     
 __version__ = Version.version
 __date__ = Version.date
 __updated__ = Version.updated
@@ -107,14 +110,17 @@
                 print(f"{gen.errmsg}", file=sys.stderr)
                 return 3
             dryRun=not args.noDry
             if args.genViaMwApi:
                 gen.generateViaMwApi(target_names=args.targets,topic_names=args.topics, dryRun=dryRun, withEditor=args.editor)
             if args.genToFile:
                 gen.generateToFile(target_dir=args.targetPath,target_names=args.targets,topic_names=args.topics, dryRun=dryRun, withEditor=args.editor) 
+        elif args.push:
+            push=Push(args)
+            push.push()       
         pass
     except KeyboardInterrupt:
         ### handle keyboard interrupt ###
         return 1
     except Exception as e:
         if DEBUG:
             raise(e)
```

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/ypgenapp.py` & `py_yprinciple_gen-0.2.7/yprinciple/ypgenapp.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/yprinciple/resources/static/css/md_style_indigo.css` & `py_yprinciple_gen-0.2.7/yprinciple/resources/static/css/md_style_indigo.css`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/.gitignore` & `py_yprinciple_gen-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/LICENSE` & `py_yprinciple_gen-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/README.md` & `py_yprinciple_gen-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.6/pyproject.toml` & `py_yprinciple_gen-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         # https://pypi.org/project/pyJustpyWidgets/
         'pyJustpyWidgets>=0.1.13',
         # https://pypi.org/project/search-engine-parser/
         'search-engine-parser>=0.6.8',
         # https://pypi.org/project/py-3rdparty-mediawiki/
         'py-3rdparty-mediawiki>=0.8.0',
         # https://pypi.org/project/pyMetaModel/
-        'pyMetaModel>=0.2.7',
+        'pyMetaModel>=0.3.0',
         # https://pypi.org/project/beautifulsoup4/
         'beautifulsoup4',
         # https://github.com/borisbabic/browser_cookie3
         # 'browser_cookie>=0.16.2'
      ]
 
 requires-python = ">=3.8"
```

### Comparing `py_yprinciple_gen-0.2.6/PKG-INFO` & `py_yprinciple_gen-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-yprinciple-gen
-Version: 0.2.6
+Version: 0.2.7
 Project-URL: Home, https://github.com/WolfgangFahl/py-yprinciple-gen
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/Py-yprinciple-gen
 Project-URL: Source, https://github.com/WolfgangFahl/py-yprinciple-gen
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4
 Requires-Dist: justpy>=0.12.1
 Requires-Dist: py-3rdparty-mediawiki>=0.8.0
 Requires-Dist: pyjustpywidgets>=0.1.13
-Requires-Dist: pymetamodel>=0.2.7
+Requires-Dist: pymetamodel>=0.3.0
 Requires-Dist: search-engine-parser>=0.6.8
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
 
 # py-yprinciple-gen
 python Library for code generation according to the Y-Principle
```

