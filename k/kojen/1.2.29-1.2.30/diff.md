# Comparing `tmp/kojen-1.2.29.tar.gz` & `tmp/kojen-1.2.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kojen-1.2.29.tar", last modified: Sun Mar 26 13:25:19 2023, max compression
+gzip compressed data, was "kojen-1.2.30.tar", last modified: Sun Apr  9 13:23:09 2023, max compression
```

## Comparing `kojen-1.2.29.tar` & `kojen-1.2.30.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 13:25:19.407673 kojen-1.2.29/
--rw-rw-rw-   0        0        0    20890 2023-03-26 13:25:19.407673 kojen-1.2.29/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-26 13:25:19.350678 kojen-1.2.29/kojen/
--rw-rw-rw-   0        0        0     6092 2023-03-26 13:24:52.000000 kojen-1.2.29/kojen/Generate.py
--rw-rw-rw-   0        0        0    14933 2023-03-26 13:24:52.000000 kojen-1.2.29/kojen/Language.py
--rw-rw-rw-   0        0        0    44063 2023-03-26 13:24:52.000000 kojen-1.2.29/kojen/LanguageCPP.py
--rw-rw-rw-   0        0        0    45191 2023-03-26 13:24:52.000000 kojen-1.2.29/kojen/LanguageCsharp.py
--rw-rw-rw-   0        0        0    10159 2023-03-26 13:24:52.000000 kojen-1.2.29/kojen/LanguagePython.py
--rw-rw-rw-   0        0        0      357 2022-07-17 15:56:39.000000 kojen-1.2.29/kojen/__init__.py
--rw-rw-rw-   0        0        0       26 2022-07-17 15:56:39.000000 kojen-1.2.29/kojen/__main__.py
--rw-rw-rw-   0        0        0    26259 2023-03-25 18:25:48.000000 kojen-1.2.29/kojen/cgen.py
--rw-rw-rw-   0        0        0    10071 2023-03-25 18:25:48.000000 kojen-1.2.29/kojen/coggen.py
--rw-rw-rw-   0        0        0    17056 2023-03-25 18:25:48.000000 kojen-1.2.29/kojen/kojentypes.py
--rw-rw-rw-   0        0        0     3169 2023-03-25 18:25:48.000000 kojen-1.2.29/kojen/plant.py
--rw-rw-rw-   0        0        0     9902 2022-08-08 16:04:22.000000 kojen-1.2.29/kojen/preservative.py
--rw-rw-rw-   0        0        0     7048 2023-03-25 18:25:48.000000 kojen-1.2.29/kojen/protogen.py
--rw-rw-rw-   0        0        0    47457 2023-03-25 18:25:48.000000 kojen-1.2.29/kojen/smgen.py
--rw-rw-rw-   0        0        0     4127 2022-07-17 15:56:39.000000 kojen-1.2.29/kojen/smvppxml.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:25:19.406674 kojen-1.2.29/kojen/test/
--rw-rw-rw-   0        0        0        0 2022-07-17 15:56:39.000000 kojen-1.2.29/kojen/test/__init__.py
--rw-rw-rw-   0        0        0    10955 2023-03-25 18:25:48.000000 kojen-1.2.29/kojen/test/cgen_test.py
--rw-rw-rw-   0        0        0    10621 2022-08-08 16:04:22.000000 kojen-1.2.29/kojen/test/preservative_test.py
--rw-rw-rw-   0        0        0    15218 2023-03-25 18:25:48.000000 kojen-1.2.29/kojen/test/smgen_test.py
--rw-rw-rw-   0        0        0    15390 2022-07-17 15:56:39.000000 kojen-1.2.29/kojen/test/vppclassdiagram_test.py
--rw-rw-rw-   0        0        0     3782 2022-07-17 15:56:39.000000 kojen-1.2.29/kojen/test/vppfs_test.py
--rw-rw-rw-   0        0        0    24276 2023-03-26 13:24:52.000000 kojen-1.2.29/kojen/umlgen.py
--rw-rw-rw-   0        0        0    49539 2023-03-26 13:24:52.000000 kojen-1.2.29/kojen/vppclassdiagram.py
--rw-rw-rw-   0        0        0    35625 2022-12-09 07:45:22.000000 kojen-1.2.29/kojen/vppfs.py
-drwxrwxrwx   0        0        0        0 2023-03-26 13:25:19.371674 kojen-1.2.29/kojen.egg-info/
--rw-rw-rw-   0        0        0    20890 2023-03-26 13:25:18.000000 kojen-1.2.29/kojen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2023-03-26 13:25:19.000000 kojen-1.2.29/kojen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 13:25:18.000000 kojen-1.2.29/kojen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-26 13:25:18.000000 kojen-1.2.29/kojen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-26 13:25:18.000000 kojen-1.2.29/kojen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 13:25:19.408673 kojen-1.2.29/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-03-25 18:25:48.000000 kojen-1.2.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.068413 kojen-1.2.30/
+-rw-rw-rw-   0        0        0    20890 2023-04-09 13:23:09.068413 kojen-1.2.30/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.028377 kojen-1.2.30/kojen/
+-rw-rw-rw-   0        0        0     6200 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/Generate.py
+-rw-rw-rw-   0        0        0    14933 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/Language.py
+-rw-rw-rw-   0        0        0    44063 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguageCPP.py
+-rw-rw-rw-   0        0        0    45191 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguageCsharp.py
+-rw-rw-rw-   0        0        0    10159 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguagePython.py
+-rw-rw-rw-   0        0        0      357 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/__init__.py
+-rw-rw-rw-   0        0        0       26 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/__main__.py
+-rw-rw-rw-   0        0        0    27220 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/cgen.py
+-rw-rw-rw-   0        0        0    10071 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/coggen.py
+-rw-rw-rw-   0        0        0    17170 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/kojentypes.py
+-rw-rw-rw-   0        0        0     3169 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/plant.py
+-rw-rw-rw-   0        0        0     9902 2022-08-08 16:04:22.000000 kojen-1.2.30/kojen/preservative.py
+-rw-rw-rw-   0        0        0     7048 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/protogen.py
+-rw-rw-rw-   0        0        0    48690 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/smgen.py
+-rw-rw-rw-   0        0        0     4127 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/smvppxml.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.067413 kojen-1.2.30/kojen/test/
+-rw-rw-rw-   0        0        0        0 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/__init__.py
+-rw-rw-rw-   0        0        0    12569 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/test/cgen_test.py
+-rw-rw-rw-   0        0        0    10621 2022-08-08 16:04:22.000000 kojen-1.2.30/kojen/test/preservative_test.py
+-rw-rw-rw-   0        0        0    18069 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/test/smgen_test.py
+-rw-rw-rw-   0        0        0    15390 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/vppclassdiagram_test.py
+-rw-rw-rw-   0        0        0     3782 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/vppfs_test.py
+-rw-rw-rw-   0        0        0    24276 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/umlgen.py
+-rw-rw-rw-   0        0        0    49539 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/vppclassdiagram.py
+-rw-rw-rw-   0        0        0    35625 2022-12-09 07:45:22.000000 kojen-1.2.30/kojen/vppfs.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.050386 kojen-1.2.30/kojen.egg-info/
+-rw-rw-rw-   0        0        0    20890 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      651 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 13:23:09.069413 kojen-1.2.30/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-04-09 13:22:41.000000 kojen-1.2.30/setup.py
```

### Comparing `kojen-1.2.29/PKG-INFO` & `kojen-1.2.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kojen
-Version: 1.2.29
+Version: 1.2.30
 Summary: Code generation tools.
 Home-page: https://github.com/kohjaen/kojen
 Author: kohjaen
 Author-email: koh.jaen@yahoo.de
 License: UNKNOWN
 Description: ![CI](https://github.com/kohjaen/kojen/workflows/CI/badge.svg)
```

### Comparing `kojen-1.2.29/kojen/Generate.py` & `kojen-1.2.30/kojen/Generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 '''
 
 
 def StateMachine(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_embedded_arm")
 
-    if not os.path.isdir(templatedir):
+    if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
         print("Error : dir '" + templatedir + "' does not exist. Aborting.")
         return
 
     language = LanguageCPP.LanguageCPP()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
@@ -45,15 +45,15 @@
     return smgenerator.Generate(transition_table, namespacenname, statemachinenameprefix, dclspc, __copy_other_files)
 
 
 def StateMachine_CSHARP(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_cs_winlinmac")
 
-    if not os.path.isdir(templatedir):
+    if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
         print("Error : dir '" + templatedir + "' does not exist. Aborting.")
         return []
 
     language = LanguageCsharp.LanguageCsharp()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
@@ -62,15 +62,15 @@
     return smgenerator.Generate(transition_table, namespacenname, statemachinenameprefix, dclspc, __copy_other_files)
 
 
 def StateMachine_PYTHON(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_py")
 
-    if not os.path.isdir(templatedir):
+    if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
         print("Error : dir '" + templatedir + "' does not exist. Aborting.")
         return []
 
     language = LanguagePython.LanguagePython()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
```

### Comparing `kojen-1.2.29/kojen/Language.py` & `kojen-1.2.30/kojen/Language.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/LanguageCPP.py` & `kojen-1.2.30/kojen/LanguageCPP.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/LanguageCsharp.py` & `kojen-1.2.30/kojen/LanguageCsharp.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/LanguagePython.py` & `kojen-1.2.30/kojen/LanguagePython.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/cgen.py` & `kojen-1.2.30/kojen/cgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,20 +201,33 @@
         res = tag.replace("<<<", "").replace(">>>", "") in a
     return res
 
 
 def hasDefault(a):
     return a.find("::", a.find("<<<")) >= 0
 
-
 def extractDefaultAndTag(a):
     default = a[a.find("::", a.find("<<<")):a.rfind(">>>")].replace("::","", 1)
     tag = a[a.find("<<<"):a.rfind(">>>")+len(">>>")]
     return [tag, default]
 
+def extractDefaultAndTagNamed(a, named):
+    all = a.split(">>>")
+    for b in all:
+        if named in b:
+            return extractDefaultAndTag(b + ">>>")
+    raise Exception(named + " not found.")
+
+def extractTagAndAandB(a):
+    tag = a[a.find("<<<"):a.find(">>>") + len(">>>")]
+    r = a[a.find("<<<") + len("<<<"):a.find(">>>")].split("::")
+    A = None if len(r) < 2 else r[1]
+    B = None if len(r) < 3 else r[2]
+    return [tag, A, B]
+
 
 def removeDefault(a):
     default = a[a.find("::", a.find("<<<")):a.rfind(">>>")]
     return a.replace(default, "")
 
 
 def replaceDefault(a, b):
@@ -244,15 +257,19 @@
         self.group = group
         self.brief = brief
         self.NAMESPACE_TO_GO_TO_OWN_FOLDER = namespace_to_folders
         # Does the input exist
         if not os.path.exists(inputfiledir):
             raise Exception("Directory '" + inputfiledir + "' does not exist.")
         else:
-            files = os.listdir(inputfiledir)
+            files = None
+            if os.path.isdir(inputfiledir):
+                files = os.listdir(inputfiledir)
+            if os.path.isfile(inputfiledir):
+                files = inputfiledir
             # Is the input empty
             if not files:
                 raise Exception("Directory '" + inputfiledir + "' is empty.")
             else:
                 # Check the output dir
                 if not os.path.exists(outputfiledir):
                     os.makedirs(outputfiledir)
@@ -441,23 +458,28 @@
         @return: CCodeModel, a dictionary -> {filename,[lines]}
         """
         template_file_found = False
         result = CCodeModel()
         CWD = self.input_template_file_dir
         dict_to_replace_lines[__TAG_DATETIME__] = datetime.datetime.fromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S')
         dict_to_replace_lines[__TAG_PLATFORM__] = sys.platform + ' python ' + sys.version
-        for root, dirs, files in os.walk(CWD):
-            for file in files:
-                if (file.lower().find(filter_files_containing_in_name.lower()) > -1 or not filter_files_containing_in_name.strip()) and not file.lower().find(".removed") > -1 :
-                    template_file_found = True
-                    cm = self.loadtemplates_firstfiltering_FILE(os.path.join(root, file), dict_to_replace_lines, dict_to_replace_filenames, filter_files_containing_in_name)
-                    result.Merge(cm)
+        if os.path.isfile(self.input_template_file_dir):
+            template_file_found = True
+            cm = self.loadtemplates_firstfiltering_FILE(self.input_template_file_dir, dict_to_replace_lines, dict_to_replace_filenames, filter_files_containing_in_name)
+            result.Merge(cm)
+        else:
+            for root, dirs, files in os.walk(CWD):
+                for file in files:
+                    if (file.lower().find(filter_files_containing_in_name.lower()) > -1 or not filter_files_containing_in_name.strip()) and not file.lower().find(".removed") > -1 :
+                        template_file_found = True
+                        cm = self.loadtemplates_firstfiltering_FILE(os.path.join(root, file), dict_to_replace_lines, dict_to_replace_filenames, filter_files_containing_in_name)
+                        result.Merge(cm)
 
-        if not template_file_found:
-            raise Exception("Directory '" + self.input_template_file_dir + "' contains no templates.")
+            if not template_file_found:
+                raise Exception("Directory '" + self.input_template_file_dir + "' contains no templates.")
 
         return result
 
     def preserve_leading_tagwhitespace_in_multiline_searchandreplace(self, line, tag, desired_text):
         """
         For the case where the 'desired_text' that should replace the 'tag' in the 'line', if it is a multi-line
         replace, it will keep the leading spaces across all lines...otherwise simply returns the input desired_text
```

### Comparing `kojen-1.2.29/kojen/coggen.py` & `kojen-1.2.30/kojen/coggen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/kojentypes.py` & `kojen-1.2.30/kojen/kojentypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,15 @@
     """
     Struct.
     A struct is a collection of base types, that form part of a message, as a separate member.
     """
     def __init__(self, structName):
         super(Struct, self).__init__()
         DefaultVal.__init__(self)
+        Documentation.__init__(self)
         self.Name  = structName
 
     def AddType(self, memberName, memberType, default = None):
         self[memberName]          = memberType
         self.defaults[memberName] = str(default) if default else default
 
     def AddStruct(self, memberName, struct):
@@ -249,14 +250,15 @@
 
 class Array(OrderedDict, Query, Documentation):
 
     PREFIX = '_Cnt'
 
     def __init__(self, arrayname, arraytype):
         super(Array, self).__init__()
+        Documentation.__init__(self)
         self.Name = arrayname
         self[self.Count()] = 'uint32'
         self.type = arraytype
 
     def Count(self):
         return self.Name+Array.PREFIX
 
@@ -282,14 +284,15 @@
      - a member of Struct
      - a member of Type[]
      - a member of Struct[].
     """
     def __init__(self, messageName, messageTypeID):
         super(Message, self).__init__()
         DefaultVal.__init__(self)
+        Documentation.__init__(self)
         self.Name            = messageName
         self.MessageTypeID   = messageTypeID
         self[self.HeaderName()] = MessageHeader(0, self.MessageTypeID)
 
     # done by Interface.
     def SetPreamble(self, preamble):
         self[self.HeaderName()].OverridePreamble(preamble)
```

### Comparing `kojen-1.2.29/kojen/plant.py` & `kojen-1.2.30/kojen/plant.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/preservative.py` & `kojen-1.2.30/kojen/preservative.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/protogen.py` & `kojen-1.2.30/kojen/protogen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/smgen.py` & `kojen-1.2.30/kojen/smgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 __TAG_PROTOMSGNAME__                = '<<<PROTOMSGNAME>>>'      # As given
 __TAG_PROTOMSGNAME_SMALL_CAMEL__    = '<<<protoMsgName>>>'      # camelCaps
 __TAG_ATTRIBUTE_TYPE__              = "<<<ATTRIBUTETYPE>>>"
 __TAG_ATTRIBUTE_NAME__              = "<<<ATTRIBUTENAME>>>"
 __TAG_PAYLOAD_TYPE__                = "<<<PAYLOADTYPE>>>"
 __TAG_PAYLOAD_NAME__                = "<<<PAYLOADNAME>>>"
 __TAG_PYTHON_ATTR__                 = "<<<PyAttr>>>"
+__TAG_DOCUMENTATION__               = "<<<DOCUMENTATION>>>"
 
 __TAG_STRUCT_BEGIN__                = "<<<PER_STRUCT_BEGIN>>>"
 __TAG_STRUCT_END__                  = "<<<PER_STRUCT_END>>>"
 __TAG_MSG_BEGIN__                   = "<<<PER_MSG_BEGIN>>>"
 __TAG_MSG_END__                     = "<<<PER_MSG_END>>>"
 __TAG_PROTOMSG_BEGIN__              = "<<<PER_PROTOMSG_BEGIN>>>"
 __TAG_PROTOMSG_END__                = "<<<PER_PROTOMSG_END>>>"
@@ -365,15 +366,15 @@
                 newline = newline.replace(__TAG_ABC__, alpha)
                 newline = newline.replace(__TAG_123__, str(cnt))
                 tabcnt = newline.count('    ')
                 if hasSpecificTag(newline,__TAG_SIGNATURE__):
                     has_signature_defaults = __TAG_SIGNATURE_DEF__ in newline
                     if hasDefault(newline):
                         # Has user params
-                        user_params = extractDefaultAndTag(newline)
+                        user_params = extractDefaultAndTagNamed(newline, cleanTag(__TAG_SIGNATURE__))
                         signature = self.get_event_signature(name, False) + ", " + user_params[1]
                         signature = signature.strip(',').strip(' ')
                         newline = newline.replace(user_params[0], signature)
                     else:
                         newline = newline.replace(__TAG_SIGNATURE_DEF__ if has_signature_defaults else __TAG_SIGNATURE__, self.get_event_signature(name, has_signature_defaults))
                     # check for brackets...remove any spurious ',' and ' '
                     newline = re.sub("\([^)]*\)", lambda x:x.group(0).replace(' , )',')').replace(', )',')').replace(',)',')').replace('( , ','(').replace('( ,','(').replace('(,','('), newline)
@@ -386,31 +387,42 @@
                 # __TAG_LITE_MEMBERINST__ -> NO PTR
                 if hasSpecificTag(newline,__TAG_LITE_MEMBERINST__) and hasDefault(newline):
                     line_member = extractDefaultAndTag(newline)
                     newline = newline.replace(line_member[0],self.instantiate_event_struct_member(name, tabcnt, False, line_member[1]))
                 else:
                     newline = newline.replace(__TAG_LITE_MEMBERINST__, self.instantiate_event_struct_member(name, tabcnt, False))  # NO PTR
                 newline = newline.replace(__TAG_MEMBERDECL__, self.declare_event_struct_members(name, tabcnt))
+                # Documentation
+                if hasSpecificTag(newline, __TAG_DOCUMENTATION__):
+                    ws = getWhitespace(newline)
+                    docs = self.events_interface[name].documentation.rstrip("\n").split("\n")
+                    for d in docs:
+                        alllinesexpanded.append(ws + d + "\n")
+                    continue
                 # Aggregate initialization
                 if hasSpecificTag(newline, __TAG_AGGREGATE_INIT__):
                     newline = newline.replace(__TAG_AGGREGATE_INIT__, self.instantiate_event_aggregate_initializer(name))
                 # Member attributes ... all structs (msgs, protocols, structs)
                 if hasSpecificTag(newline, __TAG_ATTRIBUTE_TYPE__) or hasSpecificTag(newline, __TAG_ATTRIBUTE_NAME__):
                     struct_or_msg = self.events_interface[name]
                     members = struct_or_msg.Decompose(False)
                     for mem in members:
                         membername = mem[1]
                         membertype = mem[0]
                         alllinesexpanded.append(newline.replace(__TAG_ATTRIBUTE_TYPE__, membertype).replace(__TAG_ATTRIBUTE_NAME__, membername))
                     continue
                 # Python attributes ... someone piggybacks the nice interface
                 if hasSpecificTag(newline, __TAG_PYTHON_ATTR__) and hasDefault(newline):
-                    [tag, default] = extractDefaultAndTag(newline)
-                    if hasattr(self.events_interface[name], default):
-                        newline = newline.replace(tag, str(getattr(self.events_interface[name], default)))
+                    [tag, attr, useifnotexist] = extractTagAndAandB(newline)
+                    if hasattr(self.events_interface[name], attr):
+                        newline = newline.replace(tag, str(getattr(self.events_interface[name], attr)))
+                    elif useifnotexist:
+                        newline = newline.replace(tag, useifnotexist)
+                    else:
+                        continue
                 if newline.isspace():
                     continue
                 alllinesexpanded.append(newline)
             cnt = cnt + 1
             alpha = get_next_alphabet()
 
     ### CONSOLODATE ... this is essentially a copy-paste of the above ...
@@ -435,15 +447,15 @@
                 newline = newline.replace(__TAG_ABC__, alpha)
                 newline = newline.replace(__TAG_123__, str(cnt))
                 tabcnt = newline.count('    ')
                 if hasSpecificTag(newline, __TAG_SIGNATURE__):
                     has_signature_defaults = __TAG_SIGNATURE_DEF__ in newline
                     if hasDefault(newline):
                         # Has user params
-                        user_params = extractDefaultAndTag(newline)
+                        user_params = extractDefaultAndTagNamed(newline, cleanTag(__TAG_SIGNATURE__))
                         signature = self.get_event_signature(name, False) + ", " + user_params[1]
                         signature = signature.strip(',').strip(' ')
                         newline = newline.replace(user_params[0], signature)
                     else:
                         newline = newline.replace(__TAG_SIGNATURE_DEF__ if has_signature_defaults else __TAG_SIGNATURE__, self.get_event_signature(name, has_signature_defaults))
                     # check for brackets...remove any spurious ',' and ' '
                     newline = re.sub("\([^)]*\)", lambda x: x.group(0).replace(' , )', ')').replace(', )', ')').replace(',)', ')').replace('( , ', '(').replace('( ,', '(').replace('(,', '('), newline)
@@ -455,14 +467,21 @@
                     newline = newline.replace(__TAG_MEMBERINST__, self.instantiate_event_struct_member(name, tabcnt, True))  # PTR
                 # __TAG_LITE_MEMBERINST__ -> NO PTR
                 if hasSpecificTag(newline, __TAG_LITE_MEMBERINST__) and hasDefault(newline):
                     line_member = extractDefaultAndTag(newline)
                     newline = newline.replace(line_member[0], self.instantiate_event_struct_member(name, tabcnt, False, line_member[1]))
                 else:
                     newline = newline.replace(__TAG_LITE_MEMBERINST__, self.instantiate_event_struct_member(name, tabcnt, False))  # NO PTR
+                # Documentation
+                if hasSpecificTag(newline, __TAG_DOCUMENTATION__):
+                    ws = getWhitespace(newline)
+                    docs = self.events_interface[name].documentation.rstrip("\n").split("\n")
+                    for d in docs:
+                        alllinesexpanded.append(ws + d + "\n")
+                    continue
                 # Aggregate initialization
                 if hasSpecificTag(newline, __TAG_AGGREGATE_INIT__):
                     newline = newline.replace(__TAG_AGGREGATE_INIT__, self.instantiate_event_aggregate_initializer(name))
                 if hasSpecificTag(newline, __TAG_MSGID__):
                     newline = newline.replace(__TAG_MSGID__, str(self.events_interface[name].MessageTypeID))
                 newline = newline.replace(__TAG_MEMBERDECL__, self.declare_event_struct_members(name, tabcnt, True))
                 # Member attributes ... all structs (msgs, protocols, structs)
@@ -484,17 +503,21 @@
                         #isStruct = struct_or_msg.IsStruct(membername)
                         isProtocol = struct_or_msg.IsProtocolStruct(membername)
                         if not isProtocol:
                             alllinesexpanded.append(newline.replace(__TAG_PAYLOAD_TYPE__, membertype).replace(__TAG_PAYLOAD_NAME__, membername))
                     continue
                 # Python attributes ... someone piggybacks the nice interface
                 if hasSpecificTag(newline,__TAG_PYTHON_ATTR__) and hasDefault(newline):
-                    [tag, default] = extractDefaultAndTag(newline)
-                    if hasattr(self.events_interface[name], default):
-                        newline = newline.replace(tag, str(getattr(self.events_interface[name], default)))
+                    [tag, attr, useifnotexist] = extractTagAndAandB(newline)
+                    if hasattr(self.events_interface[name], attr):
+                        newline = newline.replace(tag, str(getattr(self.events_interface[name], attr)))
+                    elif useifnotexist:
+                        newline = newline.replace(tag, useifnotexist)
+                    else:
+                        continue
                 if newline.isspace():
                     continue
                 alllinesexpanded.append(newline)
             cnt = cnt + 1
             alpha = get_next_alphabet()
     ###
```

### Comparing `kojen-1.2.29/kojen/smvppxml.py` & `kojen-1.2.30/kojen/smvppxml.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/test/cgen_test.py` & `kojen-1.2.30/kojen/test/cgen_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,14 +62,45 @@
         self.assertEqual(res_b[0], "<<<something>>>", "Wrong tag")
         self.assertEqual(res_b[1], "", "Wrong default")
         self.assertEqual(res_c[0], "", "Wrong tag")
         self.assertEqual(res_c[1], "", "Wrong default")
         self.assertEqual(res_d[0], "<<<something::this::and::this>>>", "Wrong tag")
         self.assertEqual(res_d[1], "this::and::this", "Wrong default")
 
+    def test_extract_default_and_TAG_multiple(self):
+        a = "XXX::blabla<<<something::1>>> !@#!@$ <<<else::2>>>"
+        res_a = extractDefaultAndTagNamed(a, "something")
+        res_b = extractDefaultAndTagNamed(a, "else")
+        self.assertEqual(res_a[0], "<<<something::1>>>", "Wrong tag")
+        self.assertEqual(res_a[1], "1", "Wrong default")
+        self.assertEqual(res_b[0], "<<<else::2>>>", "Wrong tag")
+        self.assertEqual(res_b[1], "2", "Wrong default")
+
+    def test_extract_TAG_and_A_and_B(self):
+        a = "blab @#$KLF!WEFJ <<<some::thing::here>>>"
+        b = "blab @#$KLF!WEFJ <<<some::thing>>>"
+        res_a = extractTagAndAandB(a)
+        self.assertEqual(len(res_a), 3, "Wrong length")
+        self.assertEqual(res_a[0], "<<<some::thing::here>>>", "Wrong tag")
+        self.assertEqual(res_a[1], "thing", "Wrong A")
+        self.assertEqual(res_a[2], "here", "Wrong B")
+        res_b = extractTagAndAandB(b)
+        self.assertEqual(len(res_b), 3, "Wrong length")
+        self.assertEqual(res_b[0], "<<<some::thing>>>", "Wrong tag")
+        self.assertEqual(res_b[1], "thing", "Wrong A")
+        self.assertEqual(res_b[2], None, "Wrong B")
+
+    def test_extract_TAG_and_A_and_B_multiple(self):
+        a = "blab @#$KLF!WEFJ <<<some::thing>>> 123498123481234 <<<some::thing>>>"
+        res_a = extractTagAndAandB(a)
+        self.assertEqual(len(res_a), 3, "Wrong length")
+        self.assertEqual(res_a[0], "<<<some::thing>>>", "Wrong tag")
+        self.assertEqual(res_a[1], "thing", "Wrong A")
+        self.assertEqual(res_a[2], None, "Wrong B")
+
     def test_remove_default(self):
         a = "XXX::blabla<<<something::1>>>"
         b = "XXX::blabla<<<something>>>"
         res_a = removeDefault(a)
         res_b = removeDefault(b)
         self.assertEqual(res_a,res_b, "Failed to remove default")
         self.assertEqual(res_b,res_b, "Failed to remove default")
```

### Comparing `kojen-1.2.29/kojen/test/preservative_test.py` & `kojen-1.2.30/kojen/test/preservative_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/test/smgen_test.py` & `kojen-1.2.30/kojen/test/smgen_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -363,35 +363,103 @@
         output = TestFeatures.do_magic(input, i, [], LanguageCPP())
 
         self.assertEqual(len(output), 2)
         self.assertEqual(output[0], "{binga, bunga}\n")
         self.assertEqual(output[1], "{bla, blabla}\n")
 
     def test_pyattr(self):
+        # param, no default
         input = []
         input.append("<<<PER_STRUCT_BEGIN>>>")
-        input.append("<<<PyAttr::bla>>>")
+        input.append("<<<PyAttr::ninja>>>")
         input.append("<<<PER_STRUCT_END>>>")
         s = Struct("somestruct")
         s.AddType("binga", "bool")
         s.AddType("bunga", "size_t")
-        s.bla = "here"
+        s.ninja = "here"
         s2 = Struct("somestruct2")
         s2.AddType("bla", "bool")
         s2.AddType("blabla", "size_t")
-        s2.bla = 36
+        s2.ninja = 36
         i = Interface('')
         i.AddStruct(s)
         i.AddStruct(s2)
-
         output = TestFeatures.do_magic(input, i, [], LanguageCPP())
         self.assertEqual(len(output), 2)
         self.assertEqual(output[0], "here\n")
         self.assertEqual(output[1], "36\n")
+        # multiple param, no default
+        input = []
+        input.append("<<<PER_STRUCT_BEGIN>>>")
+        input.append("<<<PyAttr::ninja>>> is a big fat <<<PyAttr::ninja>>>")
+        input.append("<<<PER_STRUCT_END>>>")
+        output = TestFeatures.do_magic(input, i, [], LanguageCPP())
+        self.assertEqual(len(output), 2)
+        self.assertEqual(output[0], "here is a big fat here\n")
+        self.assertEqual(output[1], "36 is a big fat 36\n")
+        # no param
+        input = []
+        input.append("<<<PER_STRUCT_BEGIN>>>")
+        input.append("<<<PyAttr::ninja>>>")
+        input.append("<<<PER_STRUCT_END>>>")
+        s = Struct("somestruct")
+        s.AddType("binga", "bool")
+        s.AddType("bunga", "size_t")
+        s2 = Struct("somestruct2")
+        s2.AddType("bla", "bool")
+        s2.AddType("blabla", "size_t")
+        i = Interface('')
+        i.AddStruct(s)
+        i.AddStruct(s2)
+        output2 = TestFeatures.do_magic(input, i, [], LanguageCPP())
+        self.assertEqual(len(output2), 0)
+        # param, default
+        input = []
+        input.append("<<<PER_STRUCT_BEGIN>>>")
+        input.append("<<<PyAttr::ninja::yoyo>>>")
+        input.append("<<<PER_STRUCT_END>>>")
+        s = Struct("somestruct")
+        s.AddType("binga", "bool")
+        s.AddType("bunga", "size_t")
+        s2 = Struct("somestruct2")
+        s2.AddType("bla", "bool")
+        s2.AddType("blabla", "size_t")
+        i = Interface('')
+        i.AddStruct(s)
+        i.AddStruct(s2)
+        output3 = TestFeatures.do_magic(input, i, [], LanguageCPP())
+        self.assertEqual(len(output3), 2)
+        self.assertEqual(output3[0], "yoyo\n")
+        self.assertEqual(output3[1], "yoyo\n")
 
+    def test_Docs(self):
+        input = []
+        input.append("<<<PER_STRUCT_BEGIN>>>")
+        input.append("  *  *  <<<DOCUMENTATION>>>")
+        input.append("<<<PER_STRUCT_END>>>")
+        s = Struct("somestruct")
+        s.AddType("binga", "bool")
+        s.AddType("bunga", "size_t")
+        s.SetDocumentation("line1\nline2\nline3\n")
+        s2 = Struct("somestruct2")
+        s2.AddType("bla", "bool")
+        s2.AddType("blabla", "size_t")
+        s2.SetDocumentation("line4\nline5\nline6")
+        i = Interface('')
+        i.AddStruct(s)
+        i.AddStruct(s2)
+        # param, no default
+        output = TestFeatures.do_magic(input, i, [], LanguageCPP())
+        self.assertEqual(len(output), 6)
+        self.assertEqual(output[0], "  *  *  line1\n")
+        self.assertEqual(output[1], "  *  *  line2\n")
+        self.assertEqual(output[2], "  *  *  line3\n")
+        self.assertEqual(output[3], "  *  *  line4\n")
+        self.assertEqual(output[4], "  *  *  line5\n")
+        self.assertEqual(output[5], "  *  *  line6\n")
     '''
     def test_split(self):
         s = 'hello world'
         self.assertEqual(s.split(), ['hello', 'world'])
         # check that s.split fails when the separator is not a string
         with self.assertRaises(TypeError):
             s.split(2)
```

### Comparing `kojen-1.2.29/kojen/test/vppclassdiagram_test.py` & `kojen-1.2.30/kojen/test/vppclassdiagram_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/test/vppfs_test.py` & `kojen-1.2.30/kojen/test/vppfs_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/umlgen.py` & `kojen-1.2.30/kojen/umlgen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/vppclassdiagram.py` & `kojen-1.2.30/kojen/vppclassdiagram.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen/vppfs.py` & `kojen-1.2.30/kojen/vppfs.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/kojen.egg-info/PKG-INFO` & `kojen-1.2.30/kojen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kojen
-Version: 1.2.29
+Version: 1.2.30
 Summary: Code generation tools.
 Home-page: https://github.com/kohjaen/kojen
 Author: kohjaen
 Author-email: koh.jaen@yahoo.de
 License: UNKNOWN
 Description: ![CI](https://github.com/kohjaen/kojen/workflows/CI/badge.svg)
```

### Comparing `kojen-1.2.29/kojen.egg-info/SOURCES.txt` & `kojen-1.2.30/kojen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kojen-1.2.29/setup.py` & `kojen-1.2.30/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.MD", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kojen",
-    version="1.2.29",
+    version="1.2.30",
     author="kohjaen",
     author_email="koh.jaen@yahoo.de",
     description="Code generation tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kohjaen/kojen",
     packages=setuptools.find_packages(),
```

