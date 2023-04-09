# Comparing `tmp/langful-0.2-py2.py3-none-any.whl.zip` & `tmp/langful-0.21-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6384 bytes, number of entries: 9
+Zip file size: 6517 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     1476 b- defN 23-Mar-25 11:54 langful/__init__.py
--rw-rw-rw-  2.0 fat       28 b- defN 23-Apr-09 04:44 langful/define.py
+-rw-rw-rw-  2.0 fat      234 b- defN 23-Apr-09 05:45 langful/define.py
 -rw-rw-rw-  2.0 fat     1556 b- defN 23-Mar-25 12:16 langful/functions.py
--rw-rw-rw-  2.0 fat     7990 b- defN 23-Apr-09 05:15 langful/lang.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2604 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      673 b- defN 23-Apr-09 05:34 langful-0.2.dist-info/RECORD
-9 files, 15509 bytes uncompressed, 5238 bytes compressed:  66.2%
+-rw-rw-rw-  2.0 fat     8012 b- defN 23-Apr-09 06:29 langful/lang.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2605 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      679 b- defN 23-Apr-09 06:29 langful-0.21.dist-info/RECORD
+9 files, 15744 bytes uncompressed, 5361 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: langful/functions.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.2.dist-info/LICENSE
+Filename: langful-0.21.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.2.dist-info/METADATA
+Filename: langful-0.21.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.2.dist-info/WHEEL
+Filename: langful-0.21.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.2.dist-info/top_level.txt
+Filename: langful-0.21.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.2.dist-info/RECORD
+Filename: langful-0.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/define.py

```diff
@@ -1,2 +1,10 @@
 FILE = "file"
-DICT = "dict"
+DICT = "dict"
+
+def get_type( obj ) :
+    if isinstance( obj , str ) :
+        return FILE
+    elif isinstance( obj , dict ) :
+        return DICT
+    else :
+        raise TypeError(f"can't use type {type(obj)}")
```

## langful/lang.py

```diff
@@ -9,79 +9,70 @@
 
     def __init__( self , lang_dir = "lang" , default_lang : str = "en_us" , file_suffix : str = ".json" , change : str = "%" ) -> None :
         """
         # lang object
 
         ---
 
-        lang_dir: Translation file storage directory
+        lang_dir: Translation file storage directory / Translation file dictionary
 
         default_lang: Default translation
 
         file_suffix: Such as '.json' or '.lang'
 
         change: Specifies what character to use for substitution , default is '%'
 
         ---
 
-        lang_dir: 翻译文件的存放目录
+        lang_dir: 翻译文件的存放目录 / 翻译文件字典
 
         default_lang: 默认使用的翻译
 
         file_suffix: 文件后缀 例如 '.json' '.lang' '.txt' 等等
 
         change: 选择用什么符号做替换 默认为'%'
 
         """
 
         default_locale = locale.getdefaultlocale()[0].lower() # 默认语言
+        self.type = get_type( lang_dir )
 
-        if isinstance( lang_dir , str ) :
+        if self.type == FILE :
             if not os.path.exists( lang_dir ) : # 判断lang文件夹是否存在
                 raise KeyError( f"'{lang_dir}' dir not find" )
-            
             if not len( os.listdir(lang_dir) ) :
                 raise RuntimeError( f"In '{lang_dir}' dir has no lang file!" ) # lang文件夹里没有语言文件
-            
             if not os.path.exists( os.path.join( lang_dir , default_lang + file_suffix ) ) : # 判断default_lang文件是否存在
                 raise KeyError( f"'{default_lang}' not find" )
-            
-            self.type = FILE
-
             lang_file = os.path.join( lang_dir , default_locale + file_suffix )
             file_suffix_len=len(file_suffix)
             lang_file_list = []
             lang_str_list = []
             language_dict = {}
-
             use_locale = default_locale
             if not os.path.exists( lang_file ) : # 若默认语言不存在对应的本地化 那么就选用默认语言文件
                 use_locale = default_lang
                 lang_file = default_lang + file_suffix
-
             for filename in os.listdir(lang_dir): # 尝试加载所有能加载的模块
                 if len( filename ) > file_suffix_len and filename[-file_suffix_len:] == file_suffix :
                     try :
                         with open( os.path.join( lang_dir , filename ) , encoding = "utf-8" ) as file :
                             language_dict[ filename[ :-file_suffix_len ] ] = json.load( file )
                         lang_str_list.append( filename[ :-file_suffix_len ] )
                         lang_file_list.append( filename )
                     except : pass
 
-        elif isinstance( lang_dir , dict ) :
+        elif self.type == DICT :
             if default_lang not in lang_dir :
                 raise KeyError( f"'{default_lang}' not find" )
-            
-            self.type = DICT
-
             if default_locale not in lang_dir :
                 use_locale = default_lang
-
             language_dict = lang_dir
             lang_str_list = list( lang_dir.keys() )
+
         else :
             raise TypeError(f"lang_dir can't use type {type(lang_dir)}")
 
         #lang_dir: Translation file storage directory
         #lang_dir: 翻译文件的存放目录
         self.lang_dir = lang_dir
         #default_lang: Default translation
@@ -148,15 +139,15 @@
                 return self.language_dict[ lang_str ] [ key ]
             else :
                 raise KeyError( f"Key '{key}' has not in dictionary!" )
             
         else :
             raise KeyError( f"Lang '{lang_str}' has not find!" )
 
-    def set( self , key:str , value:str , lang_str:str = None ) -> None : # 设置某个键值
+    def set( self , key : str , value : str , lang_str : str = None ) -> None : # 设置某个键值
         """
 
         Set one value with one key in some one dictionary
 
         在某个字典中用一个值来设置一个键
 
         # set
@@ -186,14 +177,17 @@
 
         else :
             raise KeyError( f"Lang '{lang_str}' has not find!" )
 
         if lang_str == self.use_locale :
             self.language = self.language_dict[ lang_str ]
 
+    def add( self , lang_str : str ) -> None : #todo
+        pass
+
     def replace( self , * args : str , lang_str : str = None , change : str = None ) -> str : # 替换字符串 使用%号
         """
 
         Replace string with some one dictionary
 
         用某个字典替换字符串
```

## Comparing `langful-0.2.dist-info/LICENSE` & `langful-0.21.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.2.dist-info/METADATA` & `langful-0.21.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.2
+Version: 0.21
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
-Metadata-Version: 2.1 Name: langful Version: 0.2 Home-page: https://github.com/
-cueavyqwp/langful Author: cueavyqwp Author-email: cueavyqwp@outlook.com
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: > 3.6 Description-Content-Type: text/markdown License-File:
-LICENSE # langful
+Metadata-Version: 2.1 Name: langful Version: 0.21 Home-page: https://
+github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
+cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
+markdown License-File: LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
 # example - test.py - lang - zh_cn.json - en_us.json ## zh_cn.json ```json
 { "hi" : "ä½ å¥½" , "welcome" : "æ¬¢è¿" } ``` ## en_us.json ```json { "hi" :
 "Hi" , "welcome" : "Welcome" } ``` ## tset.py ```python import langful Text =
 langful.lang() print( Text.language_dict ) print( Text.replace( "%hi%" ,
 lang_str = "zh_cn" ) ) print( Text.replace( "!hi!" , lang_str = "zh_cn" ,
```

## Comparing `langful-0.2.dist-info/RECORD` & `langful-0.21.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 langful/__init__.py,sha256=SUFPXKHNiA0PO02bImWsDuDqEKIO-PIQJB0U6ccQYFg,1476
-langful/define.py,sha256=tv0iWs4cvq3i8g9lz7xaUxoseuHm7T0vYGn8dvID8Hw,28
+langful/define.py,sha256=7O52lYGt1ayQsptk5O9STlIuQggSjy2-deVOnaD0m4s,234
 langful/functions.py,sha256=duvxnPbVpwVtuV5QVhjuXMdQ0_nstiQD6oNNh5a3HP8,1556
-langful/lang.py,sha256=_57FmAG67Q74ThhyKleUH_YIjNnMTz0-efn-p_dliz8,7990
-langful-0.2.dist-info/LICENSE,sha256=wtOXhcoLntZcyZBfSBI51OyCoeuHjed_JMZTnGOL3IY,1064
-langful-0.2.dist-info/METADATA,sha256=Pg3LrDIzgwhohWBx9psxdeQ_Y94amuIn_tq4tm-oHSs,2604
-langful-0.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-langful-0.2.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
-langful-0.2.dist-info/RECORD,,
+langful/lang.py,sha256=i2IpVhn3NI9_wIxnjBfAZR3aLxnRQbQ1ST0P6Mbsp4c,8012
+langful-0.21.dist-info/LICENSE,sha256=wtOXhcoLntZcyZBfSBI51OyCoeuHjed_JMZTnGOL3IY,1064
+langful-0.21.dist-info/METADATA,sha256=Ej_s0_c8hCExaJzTeBhjbYMoKLVASrk-iidobdu_GUY,2605
+langful-0.21.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+langful-0.21.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
+langful-0.21.dist-info/RECORD,,
```

