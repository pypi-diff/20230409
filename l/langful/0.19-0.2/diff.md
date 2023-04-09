# Comparing `tmp/langful-0.19-py2.py3-none-any.whl.zip` & `tmp/langful-0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 6075 bytes, number of entries: 8
+Zip file size: 6384 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     1476 b- defN 23-Mar-25 11:54 langful/__init__.py
--rw-rw-rw-  2.0 fat     1549 b- defN 23-Mar-25 12:06 langful/functions.py
--rw-rw-rw-  2.0 fat     7219 b- defN 23-Mar-25 11:52 langful/lang.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Mar-25 12:07 langful-0.19.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2605 b- defN 23-Mar-25 12:07 langful-0.19.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Mar-25 12:07 langful-0.19.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-25 12:07 langful-0.19.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      606 b- defN 23-Mar-25 12:07 langful-0.19.dist-info/RECORD
-8 files, 14637 bytes uncompressed, 5029 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat       28 b- defN 23-Apr-09 04:44 langful/define.py
+-rw-rw-rw-  2.0 fat     1556 b- defN 23-Mar-25 12:16 langful/functions.py
+-rw-rw-rw-  2.0 fat     7990 b- defN 23-Apr-09 05:15 langful/lang.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2604 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      673 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/RECORD
+9 files, 15509 bytes uncompressed, 5238 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: langful/__init__.py
 Comment: 
 
+Filename: langful/define.py
+Comment: 
+
 Filename: langful/functions.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.19.dist-info/LICENSE
+Filename: langful-0.2.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.19.dist-info/METADATA
+Filename: langful-0.2.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.19.dist-info/WHEEL
+Filename: langful-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.19.dist-info/top_level.txt
+Filename: langful-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.19.dist-info/RECORD
+Filename: langful-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/functions.py

```diff
@@ -1,8 +1,8 @@
-import langful.__init__
+from langful.__init__ import *
 
 def if_then( args : str = "" , replace_list : list or str = "" , change : str = "%" , else_replace : str = "" ) -> str :
     """
     # 'if_then' function
     ---
     If the Boolean value of a particular item is true or false , then replace it for the str or list
     ---
```

## langful/lang.py

```diff
@@ -1,21 +1,22 @@
 import locale
 import json
 import os
 
 from langful.__init__ import *
+from langful.define import *
 
 class lang :
 
-    def __init__( self , lang_dir : str = "lang" , default_lang : str = "en_us" , file_suffix : str = ".json" , change : str = "%" ) -> None :
+    def __init__( self , lang_dir = "lang" , default_lang : str = "en_us" , file_suffix : str = ".json" , change : str = "%" ) -> None :
         """
         # lang object
 
         ---
-        
+
         lang_dir: Translation file storage directory
 
         default_lang: Default translation
 
         file_suffix: Such as '.json' or '.lang'
 
         change: Specifies what character to use for substitution , default is '%'
@@ -27,58 +28,81 @@
         default_lang: 默认使用的翻译
 
         file_suffix: 文件后缀 例如 '.json' '.lang' '.txt' 等等
 
         change: 选择用什么符号做替换 默认为'%'
 
         """
-        if not os.path.exists( lang_dir ) : # 判断lang文件夹是否存在
-            raise KeyError( f"'{lang_dir}' dir not find" )
-        
-        if not len( os.listdir(lang_dir) ) : raise RuntimeError( f"In '{lang_dir}' dir has no lang file!" ) # lang文件夹里没有语言文件
-
-        if not os.path.exists( os.path.join( lang_dir , default_lang + file_suffix ) ) : # 判断default_lang文件是否存在
-            raise KeyError( f"'{default_lang}' not find" )
-        
+
         default_locale = locale.getdefaultlocale()[0].lower() # 默认语言
-        lang_file = os.path.join( lang_dir , default_locale + file_suffix )
-        file_suffix_len=len(file_suffix)
-        lang_file_list = []
-        lang_str_list = []
-        language_dict = {}
-
-        use_locale = default_locale
-        if not os.path.exists( lang_file ) : # 若默认语言不存在对应的本地化 那么就选用默认语言文件
-            use_locale = default_lang
-            lang_file = default_lang + file_suffix
-
-        for filename in os.listdir(lang_dir): # 尝试加载所有能加载的模块
-            if len( filename ) > file_suffix_len and filename[-file_suffix_len:] == file_suffix :
-                try :
-                    with open( os.path.join( lang_dir , filename ) , encoding = "utf-8" ) as file :
-                        language_dict[ filename[ :-file_suffix_len ] ] = json.load( file )
-                    lang_str_list.append( filename[ :-file_suffix_len ] )
-                    lang_file_list.append( filename )
-                except : pass
+
+        if isinstance( lang_dir , str ) :
+            if not os.path.exists( lang_dir ) : # 判断lang文件夹是否存在
+                raise KeyError( f"'{lang_dir}' dir not find" )
+            
+            if not len( os.listdir(lang_dir) ) :
+                raise RuntimeError( f"In '{lang_dir}' dir has no lang file!" ) # lang文件夹里没有语言文件
+            
+            if not os.path.exists( os.path.join( lang_dir , default_lang + file_suffix ) ) : # 判断default_lang文件是否存在
+                raise KeyError( f"'{default_lang}' not find" )
+            
+            self.type = FILE
+
+            lang_file = os.path.join( lang_dir , default_locale + file_suffix )
+            file_suffix_len=len(file_suffix)
+            lang_file_list = []
+            lang_str_list = []
+            language_dict = {}
+
+            use_locale = default_locale
+            if not os.path.exists( lang_file ) : # 若默认语言不存在对应的本地化 那么就选用默认语言文件
+                use_locale = default_lang
+                lang_file = default_lang + file_suffix
+
+            for filename in os.listdir(lang_dir): # 尝试加载所有能加载的模块
+                if len( filename ) > file_suffix_len and filename[-file_suffix_len:] == file_suffix :
+                    try :
+                        with open( os.path.join( lang_dir , filename ) , encoding = "utf-8" ) as file :
+                            language_dict[ filename[ :-file_suffix_len ] ] = json.load( file )
+                        lang_str_list.append( filename[ :-file_suffix_len ] )
+                        lang_file_list.append( filename )
+                    except : pass
+
+        elif isinstance( lang_dir , dict ) :
+            if default_lang not in lang_dir :
+                raise KeyError( f"'{default_lang}' not find" )
+            
+            self.type = DICT
+
+            if default_locale not in lang_dir :
+                use_locale = default_lang
+
+            language_dict = lang_dir
+            lang_str_list = list( lang_dir.keys() )
+        else :
+            raise TypeError(f"lang_dir can't use type {type(lang_dir)}")
 
         #lang_dir: Translation file storage directory
         #lang_dir: 翻译文件的存放目录
         self.lang_dir = lang_dir
         #default_lang: Default translation
         #default_lang: 默认使用的翻译
         self.default_lang = default_lang
         #file_suffix: Such as '.json' '.lang' '.txt' and more
         #file_suffix: 文件后缀 例如 '.json' '.lang' '.txt' 等等
-        self.file_suffix = file_suffix
+        if self.type == FILE :
+            self.file_suffix = file_suffix
         # lang_file: Choose to use's language file
         # lang_file: 选择使用的语言文件
-        self.lang_file = lang_file
+        if self.type == FILE :
+            self.lang_file = lang_file
         # lang_file_list: All can find's language file
         # lang_file_list: 所有能找到的语言文件
-        self.lang_file_list = lang_file_list
+        if self.type == FILE :
+            self.lang_file_list = lang_file_list
         # lang_str_list: All can find's language file's name
         # lang_str_list: 所有能找到的语言文件的名字
         self.lang_str_list = lang_str_list
         # language_dict: Load all can read's language file
         # language_dict: 加载所有可以读取的语言文件
         self.language_dict = language_dict
         # language: Load need's language file
@@ -148,28 +172,28 @@
         ---
 
         key: 键值
 
         value: 需要更改的值
 
         lang_str: 例如 'zh_cn' 或 'en_us' 等等
-        
+
         """
         if not lang_str :
             lang_str = self.use_locale
 
         if lang_str in self.lang_str_list :
-            self.language_dict[ lang_str ] [ key ] =  value
+            self.language_dict[ lang_str ] [ key ] = value
 
         else :
             raise KeyError( f"Lang '{lang_str}' has not find!" )
 
         if lang_str == self.use_locale :
             self.language = self.language_dict[ lang_str ]
-            
+
     def replace( self , * args : str , lang_str : str = None , change : str = None ) -> str : # 替换字符串 使用%号
         """
 
         Replace string with some one dictionary
 
         用某个字典替换字符串
 
@@ -178,15 +202,15 @@
         ---
 
         key: The dictionary's key
 
         args: Strings
 
         lang_str: Such as 'zh_cn' or 'en_us' and more
-    
+
         change: Specifies what character to use for substitution , default is '%'
 
         ---
 
         key: 键值
 
         args: Strings
@@ -217,9 +241,9 @@
 
                 elif not I : Ret += change
 
                 else : raise KeyError( f"Key '{I}' has not find!" )
             else : Ret += I
 
             i += 1
-            
+
         return Ret
```

## Comparing `langful-0.19.dist-info/LICENSE` & `langful-0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.19.dist-info/METADATA` & `langful-0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.19
+Version: 0.2
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
```

### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: langful Version: 0.19 Home-page: https://
-github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
-cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
-markdown License-File: LICENSE # langful
+Metadata-Version: 2.1 Name: langful Version: 0.2 Home-page: https://github.com/
+cueavyqwp/langful Author: cueavyqwp Author-email: cueavyqwp@outlook.com
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: > 3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
 # example - test.py - lang - zh_cn.json - en_us.json ## zh_cn.json ```json
 { "hi" : "ä½ å¥½" , "welcome" : "æ¬¢è¿" } ``` ## en_us.json ```json { "hi" :
 "Hi" , "welcome" : "Welcome" } ``` ## tset.py ```python import langful Text =
 langful.lang() print( Text.language_dict ) print( Text.replace( "%hi%" ,
 lang_str = "zh_cn" ) ) print( Text.replace( "!hi!" , lang_str = "zh_cn" ,
```

