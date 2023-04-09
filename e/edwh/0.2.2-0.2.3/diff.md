# Comparing `tmp/edwh-0.2.2.tar.gz` & `tmp/edwh-0.2.3.tar.gz`

## Comparing `edwh-0.2.2.tar` & `edwh-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 edwh-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.2.2/.idea/.gitignore
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.2.2/.idea/edwh.iml
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.2.2/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 edwh-0.2.2/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.2.2/.idea/modules.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.2.2/.idea/vcs.xml
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 edwh-0.2.2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.2.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.2.2/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.2/src/edwh/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 edwh-0.2.2/src/edwh/cli.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 edwh-0.2.2/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 edwh-0.2.2/README.md
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 edwh-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 edwh-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 edwh-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/.gitignore
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/edwh.iml
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh-0.2.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.2.3/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.3/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.2.3/src/edwh/cli.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 edwh-0.2.3/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.2.3/README.md
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 edwh-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 edwh-0.2.3/PKG-INFO
```

### Comparing `edwh-0.2.2/CHANGELOG.md` & `edwh-0.2.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `edwh-0.2.2/.idea/jupyter-settings.xml` & `edwh-0.2.3/.idea/jupyter-settings.xml`

 * *Files identical despite different names*

### Comparing `edwh-0.2.2/.idea/workspace.xml` & `edwh-0.2.3/.idea/workspace.xml`

 * *Files 16% similar despite different names*

#### Comparing `edwh-0.2.2/.idea/workspace.xml` & `edwh-0.2.3/.idea/workspace.xml`

```diff
@@ -1,24 +1,27 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="a8ee968c-c8d6-4911-ae81-e260b5e9d9f0" name="Changes" comment="build: version bump">
+    <list default="true" id="a8ee968c-c8d6-4911-ae81-e260b5e9d9f0" name="Changes" comment="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list.">
       <change beforePath="$PROJECT_DIR$/.idea/vcs.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/vcs.xml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/edwh/cli.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/edwh/cli.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
+    <option name="RECENT_BRANCH_BY_REPOSITORY">
+      <map>
+        <entry key="$PROJECT_DIR$" value="master"/>
+      </map>
+    </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2O1KNWZ6CP36BVEqAMkUxvDRxX7"/>
   <component name="ProjectViewState">
@@ -28,15 +31,15 @@
   </component>
   <component name="PropertiesComponent">{
   &quot;keyToString&quot;: {
     &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
     &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
     &quot;SHARE_PROJECT_CONFIGURATION_FILES&quot;: &quot;true&quot;,
     &quot;WebServerToolWindowFactoryState&quot;: &quot;false&quot;,
-    &quot;git-widget-placeholder&quot;: &quot;master&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
     &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
     &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
     &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
     &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
   }
 }</component>
   <component name="RecentsManager">
@@ -51,15 +54,17 @@
       <created>1680722607644</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1680722607644</updated>
       <workItem from="1680722608717" duration="182000"/>
       <workItem from="1680724415156" duration="2074000"/>
       <workItem from="1680965546116" duration="403000"/>
-      <workItem from="1680967358935" duration="1178000"/>
+      <workItem from="1680967358935" duration="3652000"/>
+      <workItem from="1681073068492" duration="64000"/>
+      <workItem from="1681073149934" duration="817000"/>
     </task>
     <task id="LOCAL-00001" summary="feat: added `plugins` as an optional dependencies">
       <created>1680724520623</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1680724520623</updated>
@@ -74,20 +79,39 @@
     <task id="LOCAL-00003" summary="build: version bump">
       <created>1680726710476</created>
       <option name="number" value="00003"/>
       <option name="presentableId" value="LOCAL-00003"/>
       <option name="project" value="LOCAL"/>
       <updated>1680726710476</updated>
     </task>
-    <option name="localTasksCounter" value="4"/>
+    <task id="LOCAL-00004" summary="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list.">
+      <created>1680968678579</created>
+      <option name="number" value="00004"/>
+      <option name="presentableId" value="LOCAL-00004"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1680968678579</updated>
+    </task>
+    <option name="localTasksCounter" value="5"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
+  <component name="Vcs.Log.Tabs.Properties">
+    <option name="TAB_STATES">
+      <map>
+        <entry key="MAIN">
+          <value>
+            <State/>
+          </value>
+        </entry>
+      </map>
+    </option>
+  </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="feat: added `plugins` as an optional dependencies"/>
     <MESSAGE value="fix: added `edwh-demo-tasks-plugin` as a `plugins` optional dependency"/>
     <MESSAGE value="build: version bump"/>
-    <option name="LAST_COMMIT_MESSAGE" value="build: version bump"/>
+    <MESSAGE value="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list."/>
+    <option name="LAST_COMMIT_MESSAGE" value="fix: added `tomlkit` dependency voor `omgeving`, changed the output of the discovered plugins list."/>
   </component>
 </project>
```

### Comparing `edwh-0.2.2/src/edwh/cli.py` & `edwh-0.2.3/src/edwh/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 discovered_plugins = entry_points(group='edwh.tasks')
 for plugin in discovered_plugins:
     plugin_module = plugin.load()
     plugin_collection = Collection.from_module(plugin_module)
     collection.add_collection(plugin_collection, plugin.name)
 
 import os
-print('plugins:',discovered_plugins)
+print('Discovered plugins:',[_.value.split('.')[0] for _ in discovered_plugins])
 
 old_path = sys.path[:]
 
 for path in ['.', '..', '../..']:
     path = pathlib.Path(path)
     sys.path = [str(path)] + old_path
     try:
```

### Comparing `edwh-0.2.2/LICENSE.txt` & `edwh-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.2.2/pyproject.toml` & `edwh-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
   'importlib_metadata >=3.6 ; python_version < "3.10"',
 ]
 [project.optional-dependencies]
 omgeving = [
   'humanize',
   'tabulate',
   'pyyaml',
+  'tomlkit'
 ]
 plugins = [
   'edwh-multipass-plugin',
   'edwh-demo-tasks-plugin',
   'edwh-restic-plugin',
 ]
```

### Comparing `edwh-0.2.2/PKG-INFO` & `edwh-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.2.2
+Version: 0.2.3
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -20,14 +20,15 @@
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: invoke
 Provides-Extra: omgeving
 Requires-Dist: humanize; extra == 'omgeving'
 Requires-Dist: pyyaml; extra == 'omgeving'
 Requires-Dist: tabulate; extra == 'omgeving'
+Requires-Dist: tomlkit; extra == 'omgeving'
 Provides-Extra: plugins
 Requires-Dist: edwh-demo-tasks-plugin; extra == 'plugins'
 Requires-Dist: edwh-multipass-plugin; extra == 'plugins'
 Requires-Dist: edwh-restic-plugin; extra == 'plugins'
 Description-Content-Type: text/markdown
 
 # edwh
@@ -37,17 +38,22 @@
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
+- [Changelog](#changelog)
 
 ## Installation
 
 ```console
 pipx install edwh
 ```
 
 ## License
 
 `edwh` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+
+## Changelog 
+
+[See CHANGELOG.md](CHANGELOG.md)
```

