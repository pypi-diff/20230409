# Comparing `tmp/mongopersistence-0.1.3.tar.gz` & `tmp/mongopersistence-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongopersistence-0.1.3.tar", max compression
+gzip compressed data, was "mongopersistence-0.2.0.tar", max compression
```

## Comparing `mongopersistence-0.1.3.tar` & `mongopersistence-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-02-15 22:24:10.106716 mongopersistence-0.1.3/LICENSE
--rw-r--r--   0        0        0       94 2023-02-22 21:51:25.863470 mongopersistence-0.1.3/README.md
--rw-r--r--   0        0        0      112 2023-02-23 21:02:46.777735 mongopersistence-0.1.3/mongopersistence/__init__.py
--rw-r--r--   0        0        0     1691 2023-02-24 22:06:51.891364 mongopersistence-0.1.3/mongopersistence/dbhelper.py
--rw-r--r--   0        0        0     8680 2023-02-26 17:44:58.335454 mongopersistence-0.1.3/mongopersistence/persistence.py
--rw-r--r--   0        0        0      406 2023-02-26 17:10:37.445548 mongopersistence-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 mongopersistence-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-08 15:03:17.174512 mongopersistence-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2219 2023-04-08 15:03:17.174657 mongopersistence-0.2.0/README.md
+-rw-r--r--   0        0        0       57 2023-04-08 15:15:28.419882 mongopersistence-0.2.0/mongopersistence/__init__.py
+-rw-r--r--   0        0        0     9918 2023-04-09 19:21:09.184267 mongopersistence-0.2.0/mongopersistence/persistence.py
+-rw-r--r--   0        0        0      406 2023-04-09 20:27:18.310535 mongopersistence-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 mongopersistence-0.2.0/PKG-INFO
```

### Comparing `mongopersistence-0.1.3/LICENSE` & `mongopersistence-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongopersistence-0.1.3/mongopersistence/persistence.py` & `mongopersistence-0.2.0/mongopersistence/persistence.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,88 @@
-from mongopersistence.dbhelper import *
-
+from dataclasses import dataclass,field
 from copy import deepcopy
 from typing import Dict, Optional
 
-from telegram.ext import BasePersistence
+from telegram.ext import BasePersistence,PersistenceInput
 from telegram.ext._utils.types import BD, CD, UD, CDCData, ConversationDict, ConversationKey 
 
+from pymongo import MongoClient
+from pymongo.collection import Collection
+from pymongo.database import Database
+
 BOT_DATA_KEY = 0
 
+@dataclass()
+class TypeData:
+
+    collection_name : str
+    db  : Database
+
+    col  : Collection = None
+    data : dict = field(default_factory=dict)
+    
+    def exists(self) -> bool:
+        return not self.collection_name is None
+
+    def __post_init__(self) -> None:
+        if self.exists():
+            self.col = self.db[self.collection_name]
+
 class MongoPersistence(BasePersistence[BD,CD,UD]):
 
     def __init__(
-            self,helper: DBMongoHelper,
+            self,
+            mongo_key: str,
+            db_name: str,
+            name_col_bot_data: str = None,
+            name_col_chat_data:str = None,
+            name_col_user_data:str = None,
+            #name_col_callback_data:str = None,
+            name_col_conversations:str = None,
             update_interval: float = 60,
-            load_on_flush = True
+            load_on_flush = False
         ):
-        super().__init__(helper.store_data, update_interval)
+        
+        #TODO: add support for callback_data
+        #TODO: add a feature that allows you to ignore dictionary elements using string lists so they don't become persistent
+        
+        self.client = MongoClient(mongo_key)
+        self.db     = self.client[db_name]
 
-        self.helper = helper
+        self.bot_data = TypeData(name_col_bot_data,self.db)
+        self.chat_data = TypeData(name_col_chat_data,self.db)
+        self.user_data = TypeData(name_col_user_data,self.db)
+        #self.callback_data = TypeData(name_col_callback_data,self.db)
+        self.conversations_data = TypeData(name_col_conversations,self.db)
+
+        self.store_data = PersistenceInput(
+            self.bot_data.exists(),
+            self.chat_data.exists(),
+            self.user_data.exists(),
+            False #self.callback_data.exists()
+        )
+                
+        super().__init__(self.store_data, update_interval)
 
         self.load_on_flush = load_on_flush
 
-        self.user_data : typedata = helper.user_data
-        self.chat_data : typedata = helper.chat_data
-        self.bot_data  : typedata = helper.bot_data
-
-        #self.callback_data      : typedata = helper.callback_data
-        self.conversations_data : typedata = helper.conversations_data
-
 # [================================================ GENERAL FUNCTIONS ==================================================]
 
-    def get_data(self,type_data: typedata) -> dict:       
+    def get_data(self,type_data: TypeData) -> dict:       
         if not type_data.exists():
             return
         if type_data.data == {}:
             data = type_data.data
             post : dict
             for post in type_data.col.find():
                 id = post.pop('_id')
                 data[id] = post
         return deepcopy(data)
 
-    def update_data(self,type_data: typedata,id,new_data) -> None:
+    def update_data(self,type_data: TypeData,id,new_data) -> None:
         if not type_data.exists() or self.load_on_flush or new_data == {}:
             return
         data = type_data.data
         if data.get(id) == new_data:
             return
         new_post = {'_id':id}
         new_post.update(new_data)
@@ -53,35 +90,35 @@
         if not old_post:
             type_data.col.insert_one(new_post)
             return
         if old_post != new_post:
             type_data.col.replace_one({'_id':id},new_post)
         data[id] = new_data
     
-    def refresh_data(self,type_data: typedata,id,local_data: dict) -> None:
+    def refresh_data(self,type_data: TypeData,id,local_data: dict) -> None:
         if not type_data.exists() or self.load_on_flush:
             return
         data = type_data.data
         post : dict = type_data.col.find_one({"_id":id})
         if not post:
             return
         post.pop('_id')
         if post != local_data:
             local_data.update(post)
             data[id] = deepcopy(local_data)
 
-    def drop_data(self,type_data: typedata,id) -> None:
+    def drop_data(self,type_data: TypeData,id) -> None:
         if not type_data.exists():
             return
         data = type_data.data
         if data.get(id):
             data.pop(id)
             type_data.col.delete_one({'_id':id})
 
-    def load_all_type_data(self,type_data: typedata) -> None:
+    def load_all_type_data(self,type_data: TypeData) -> None:
         if not type_data.exists():
             return
         data = type_data.data
         for key,item in data.items():
             new_post = {'_id':key}
             new_post.update(item)
             old_post = type_data.col.find_one({'_id':key})
@@ -221,8 +258,8 @@
                 new_post = {'_id':BOT_DATA_KEY,'content':self.bot_data.data}
                 old_post = self.bot_data.col.find_one({'_id':BOT_DATA_KEY})
                 if old_post:
                     if old_post!=new_post:
                         self.bot_data.col.update_one({'_id':BOT_DATA_KEY},{'$set':{'content':self.bot_data}})
                 else:
                     self.bot_data.col.insert_one(new_post)
-        self.helper.client.close()
+        self.client.close()
```

