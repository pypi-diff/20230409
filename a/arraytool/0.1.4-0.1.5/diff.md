# Comparing `tmp/arraytool-0.1.4.tar.gz` & `tmp/arraytool-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraytool-0.1.4.tar", last modified: Fri Apr 15 17:39:52 2022, max compression
+gzip compressed data, was "arraytool-0.1.5.tar", last modified: Sat Apr  8 02:41:50 2023, max compression
```

## Comparing `arraytool-0.1.4.tar` & `arraytool-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-04-15 17:39:52.321053 arraytool-0.1.4/
--rw-rw-rw-   0        0        0     3430 2022-04-15 17:39:52.320053 arraytool-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2022-03-06 14:05:53.000000 arraytool-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2022-04-15 17:39:52.304049 arraytool-0.1.4/arraytool/
--rw-rw-rw-   0        0        0      353 2022-04-15 17:38:16.000000 arraytool-0.1.4/arraytool/__init__.py
--rw-rw-rw-   0        0        0   151366 2022-04-15 17:33:57.000000 arraytool-0.1.4/arraytool/core.py
--rw-rw-rw-   0        0        0    14220 2022-04-15 16:53:39.000000 arraytool-0.1.4/arraytool/decorator.py
--rw-rw-rw-   0        0        0    44381 2022-04-14 10:07:37.000000 arraytool-0.1.4/arraytool/pytool.py
-drwxrwxrwx   0        0        0        0 2022-04-15 17:39:52.317052 arraytool-0.1.4/arraytool.egg-info/
--rw-rw-rw-   0        0        0     3430 2022-04-15 17:39:51.000000 arraytool-0.1.4/arraytool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2022-04-15 17:39:52.000000 arraytool-0.1.4/arraytool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-15 17:39:51.000000 arraytool-0.1.4/arraytool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-04-15 17:39:51.000000 arraytool-0.1.4/arraytool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-04-15 17:39:52.321053 arraytool-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      926 2022-03-12 07:22:00.000000 arraytool-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 02:41:50.509335 arraytool-0.1.5/
+-rw-rw-rw-   0        0        0     1512 2021-10-22 06:10:12.000000 arraytool-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2332 2023-04-08 02:41:50.509335 arraytool-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2022-03-06 14:05:53.000000 arraytool-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 02:41:50.495250 arraytool-0.1.5/arraytool/
+-rw-rw-rw-   0        0        0      353 2022-04-15 17:38:16.000000 arraytool-0.1.5/arraytool/__init__.py
+-rw-rw-rw-   0        0        0   189617 2023-04-08 01:56:36.000000 arraytool-0.1.5/arraytool/core.py
+-rw-rw-rw-   0        0        0    18054 2022-11-20 04:15:58.000000 arraytool-0.1.5/arraytool/decorator.py
+-rw-rw-rw-   0        0        0    53840 2023-03-28 16:51:59.000000 arraytool-0.1.5/arraytool/pytool.py
+drwxrwxrwx   0        0        0        0 2023-04-08 02:41:50.509335 arraytool-0.1.5/arraytool.egg-info/
+-rw-rw-rw-   0        0        0     2332 2023-04-08 02:41:50.000000 arraytool-0.1.5/arraytool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-08 02:41:50.000000 arraytool-0.1.5/arraytool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 02:41:50.000000 arraytool-0.1.5/arraytool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-08 02:41:50.000000 arraytool-0.1.5/arraytool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 02:41:50.509335 arraytool-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      926 2022-04-16 10:32:43.000000 arraytool-0.1.5/setup.py
```

### Comparing `arraytool-0.1.4/README.md` & `arraytool-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `arraytool-0.1.4/arraytool/core.py` & `arraytool-0.1.5/arraytool/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 """
 Created on Fri Nov 27 20:41:00 2020
 
 @author: yonder_sky
 """
 
 # 基于ndarray的数据表类工具库，春秋迭代，yondersky@126.com，2020-11-27
-# 更新日期：2022-04-15
+# 更新日期：2023-04-08
 
-import copy
+import collections, copy
 import numpy as np
 import pandas as pd
 from bisect import bisect
 from pandas import DataFrame, Series
+from scipy.stats import pearsonr, spearmanr
 
 from arraytool.decorator import DecorateFrame, DecorateFrameGroupBy, \
     DecorateSeries, DecorateSeriesGroupBy
 from arraytool.pytool import ExpandSize, \
-    IsArray, IsBool, IsDataFrame, IsIndex, IsInteger, IsIterable, IsNA, \
-    IsMultiIndex, IsSeries, IsSimpleIndex, IsSingleType, IsSingleType2, \
-    IsSlice, NA, TupleProduct, \
-    argsort, leftex, lexsort, posdiff, rank, temap, which
+    IsArray, IsBool, IsDataFrame, IsIndex, IsInteger, IsIterable, \
+    IsMultiIndex, IsNA, IsSeries, IsSimpleIndex, \
+    IsSingleType, IsSingleType2, \
+    IsSlice, MaxRetreat, NA, ListProduct, TupleProduct, \
+    argsort, leftex, lexsort, posdiff, rank, temap, unique, which
 
 # 1. 通用模块
 
 # 1.1 通用参数
- 
+
 # ArrayFrame及其派生类、ArraySeries及其派生类、ArrayValueIndex类
 AnsiDType = object
 AnsiInitLen = 1
 AnsiAutoExpand = True
 AnsiExpandCount = 0
 AnsiExpandRatio = 1.5
 # ArraySeries及其派生类
@@ -65,16 +67,15 @@
 # 2022-03-06
 def new_index(index, new_frame = True):
     '''由现有索引创建新索引'''
     if isinstance(index,FrameAxisIndex):
         if new_frame:
             return None, index._Labels
         else:
-            if index._AssignID!=index.frame._AssignManager.AssignID:
-                index._SetIndex()
+            index.update()
             return index._Index, None
     else:
         return index, None
 
 # 2. 数据索引
 
 # 2.1 数据索引基类
@@ -147,14 +148,27 @@
     
     # 2021-12-16
     def _ArgSort(self, ascending = True, na_option = 'last', method = 'first',
         key = None):
         '''下标排序（内部使用）'''
         return None
     
+    # 2022-11-20
+    def _DropDuplicates(self, keep = 'first'):
+        '''
+        内部去重。
+        【注】
+        1. keep参数可选项：
+           first - 仅保留首项
+           last - 仅保留尾项
+           none - 不保留任何项
+        2. 返回值依次为去重后下标或切片，以及是否实际发生了去除。
+        '''
+        return slice(self._ValidLen), False
+    
     # 2021-06-25
     def _GetPrep(self, item):
         '''
         取值预处理。
         【注】函数依次返回下标、是否简单类型。
         '''
         if IsBool(item):
@@ -173,49 +187,74 @@
         赋值预处理。
         【注】本函数依次返回下标、所需最大长度。
         '''
         if IsBool(item):
             if item:
                 return 0, 1
             else:
-                return None, None
+                return None, 0
         elif IsInteger(item):
             return item, item+1
         elif IsSlice(item):
             return item, item.stop
-        elif IsIterable(item) and IsBool(item[0]):
-            item = np.where(item)[0]
         if len(item)==0:
             return item, 0
         else:
+            if IsBool(item[0]):
+                item = which(item)
+                if len(item)==0:
+                    return item, 0
             return item, max(item)+1
     
     # 2021-06-20
     def _UpdateLen(self, length):
         '''更新索引长度'''
         self._ValidLen = length
         return
     
     # 2021-09-25
     def copy(self):
         '''拷贝'''
         return ArrayIndex(self._ValidLen)
     
+    # 2022-11-20
+    def drop_duplicates(self, keep = 'first'):
+        '''
+        去重。
+        【注】
+        1. keep参数可选项：
+           first - 仅保留首项
+           last - 仅保留尾项
+           none - 不保留任何项
+        2. 返回值依次为去重后下标或切片，以及是否实际发生了去除。
+        '''
+        return self.copy()
+    
+    # 2022-04-19
+    def get_iloc(self, i):
+        '''获取指定下标上的索引'''
+        return i
+    
     # 2022-02-08
     def items(self):
         '''键值对遍历器'''
         for i in self:
             yield i, i
         return
     
     # 2022-02-08
     def keys(self):
         '''键遍历器'''
         return self.__iter__()
     
+    # 2022-06-04
+    def new_key_index(self):
+        '''根据索引键生成新的索引'''
+        return None
+    
     # 2022-03-20
     def pos(self):
         '''值下标遍历器'''
         return self.__iter__()
 
     # 2022-02-03
     def reindex(self, index, method = 'keep', dupl_method = 'all', 
@@ -246,14 +285,22 @@
         elif method=='bfill' or method=='backfill':
             index[index<0] = 0
             index[index>=vlen] = -1
         else:
             index = index[(index>=0) & (index<vlen)]
         return index, None
     
+    # 2022-04-24
+    def rename(self, mapper):
+        '''
+        重命名索引项。
+        【注】ArrayIndex不支持此操作。
+        '''
+        pass
+    
     # 2021-07-19
     def take(self, pos):
         '''切片'''
         return None
     
     # 2022-02-26
     def to_pandas(self):
@@ -280,15 +327,15 @@
     
     >>> akindex.to_pandas()
     Index(['c', 'b', 'd', 'f', 'y'], dtype='object')
     
     >>> akindex.reindex(list('abkfz'))
     (array([-1,  1, -1,  3, -1], dtype=int64), ['a', 'b', 'k', 'f', 'z'])
     >>> akindex.reindex(list('abkfz'),'ignore')
-    (array([1, 3], dtype=int64), ['a', 'b', 'k', 'f', 'z'])
+    (array([1, 3], dtype=int64), ['b', 'f'])
     >>> akindex.reindex(list('abkfz'),'ffill')
     (array([-1,  1,  3,  3,  4], dtype=int64), ['a', 'b', 'k', 'f', 'z'])
     >>> akindex.reindex(list('abkfz'),'bfill')
     (array([ 1,  1,  4,  3, -1], dtype=int64), ['a', 'b', 'k', 'f', 'z'])
     '''
     simple = False
     multi_values = False
@@ -456,25 +503,35 @@
         return
     
     # 2022-01-30
     def copy(self):
         '''拷贝（重载函数）'''
         return ArrayKeyIndex(self._KeyList)
     
+    # 2022-04-19
+    def get_iloc(self, i):
+        '''获取指定下标上的索引（重载函数）'''
+        return self._KeyList[i]
+
     # 2022-02-08
     def items(self):
         '''键值对遍历器（重载函数）'''
         yield from self._Keys.items()
         return
 
     # 2022-02-08
     def keys(self):
         '''键遍历器（重载函数）'''
         return self._Keys.keys()
     
+    # 2022-06-04
+    def new_key_index(self):
+        '''根据索引键生成新的索引（重载函数）'''
+        return ArrayKeyIndex(self._KeyList)
+
     # 2022-03-20
     def pos(self):
         '''值下标遍历器（重载函数）'''
         return self._Keys.values()
     
     # 2022-02-03
     def reindex(self, index, method = 'keep', dupl_method = 'all',
@@ -520,15 +577,41 @@
                     if sortedKeys is None:
                         self._SetSortedKeys()
                         sortedKeys = self._SortedKeys
                     p = bisect(sortedKeys,i)
                     rt.append(keys[sortedKeys[p]] if p<klen else -1)
         else:
             rt = [keys[i] for i in index if i in keys]
-        return np.array(rt,AnsiPosDtype), (None if drop_index else index)
+        if drop_index:
+            rtindex = None
+        else:
+            rtindex = self.take(rt) if method=='ignore' else index
+        return np.array(rt,AnsiPosDtype), rtindex
+    
+    # 2022-04-22
+    def rename(self, mapper):
+        '''重命名索引项（重载函数）'''
+        keys = self._Keys
+        keyList = self._KeyList
+        changed = False
+        for k, v in mapper.items():
+            if k==v:
+                continue
+            if v in keys:
+                raise ValueError(
+                    'Error(ArrayKeyIndex): Duplicated column name.')
+            keyList[keys[k]] = v
+            changed = True
+        if changed:
+            newkeys = {}
+            for i in range(len(keys)):
+                newkeys[keyList[i]] = i
+            self._Keys = newkeys
+            self._SortedKeys = None
+        return
     
     # 2021-06-09
     @temap
     def take(self, pos):
         '''切片（重载函数）'''
         return self._KeyList[pos]
     
@@ -579,17 +662,16 @@
                 init_len = values._ValidLen
             if auto_expand is None:
                 auto_expand = values._AutoExpand
             if expand_count is None:
                 expand_count = values._ExpandCount
             if expand_ratio is None:
                 expand_ratio = values._ExpandRatio
-            _assign_manager = values._AssignManager
-        
-        if isinstance(values,ArraySeries) and not copy:
+            _assign_manager = values._AssignManager        
+        elif isinstance(values,ArraySeries) and not copy:
             self._Value = values
         else:
             self._Value = ArraySeries(
                 data = values,
                 dtype = dtype,
                 copy = copy,
                 init_len = init_len,
@@ -643,14 +725,35 @@
         key = None):
         '''下标排序（内部使用，重载函数）'''
         values = self._Value._ValidData
         if not key is None:
             values = key(values)
         return argsort(values,ascending,na_option,method)
     
+    # 2022-11-20
+    def _DropDuplicates(self, keep = 'first'):
+        '''内部去重（重载函数）'''
+        if self._AssignID!=self._Value._AssignManager.AssignID:
+            self._UpdateKey()
+        if self._MultiValues:
+            rt = []
+            if keep=='first':
+                for p in self.pos():
+                    rt.append(p[0])
+            elif keep=='last':
+                for p in self.pos():
+                    rt.append(p[-1])
+            else:
+                for p in self.pos():
+                    if len(p)==1:
+                        rt += [p]
+            return rt, True
+        else:
+            return slice(len(self)), False
+    
     # 2021-07-17
     def _GetPrep(self, item):
         '''取值预处理（重载函数）'''
         if self._AssignID!=self._Value._AssignManager.AssignID:
             self._UpdateKey()
         
         keys = self._Keys
@@ -759,17 +862,33 @@
         value = self._Value
         return ArrayValueIndex(
             values = value._ValidData,
             dtype = value.dtype,
             copy = True,
             auto_expand = value._AutoExpand,
             expand_count = value._ExpandCount,
-            expand_ratio = value._ExpandRatio
+            expand_ratio = value._ExpandRatio,
         )
     
+    # 2022-11-20
+    def drop_duplicates(self, keep = 'first'):
+        '''去重（重载函数）'''
+        if self._AssignID!=self._Value._AssignManager.AssignID:
+            self._UpdateKey()
+        if self._MultiValues:
+            pos, changed = self._DropDuplicates(keep)
+            return self.take(pos) if changed else self.copy()
+        else:
+            return self.copy()
+    
+    # 2022-04-19
+    def get_iloc(self, i):
+        '''获取指定下标上的索引（重载函数）'''
+        return self._Value[i]
+    
     # 2022-02-08
     def items(self):
         '''键值对遍历器（重载函数）'''
         if self._AssignID!=self._Value._AssignManager.AssignID:
             self._UpdateKey()
         yield from self._Keys.items()
         return
@@ -777,14 +896,21 @@
     # 2022-02-08
     def keys(self):
         '''键遍历器（重载函数）'''
         if self._AssignID!=self._Value._AssignManager.AssignID:
             self._UpdateKey()
         return self._Keys.keys()
     
+    # 2022-06-04
+    def new_key_index(self):
+        '''根据索引键生成新的索引（重载函数）'''
+        if self._AssignID!=self._Value._AssignManager.AssignID:
+            self._UpdateKey()
+        return ArrayKeyIndex(self._Keys.keys())
+    
     # 2022-03-20
     def pos(self):
         '''值下标遍历器（重载函数）'''
         if self._AssignID!=self._Value._AssignManager.AssignID:
             self._UpdateKey()
         return self._Keys.values()
     
@@ -912,14 +1038,27 @@
                     rt.append(keys[sortedKeys[p]][0] if p<klen else -1)
             if drop_index:
                 rtindex = None
             else:
                 rtindex = self.take(rt) if method=='ignore' else index
         
         return np.array(rt,AnsiPosDtype), rtindex
+    
+    # 2022-04-24
+    def rename(self, mapper):
+        '''重命名索引项（重载函数）'''
+        if self._AssignID!=self._Value._AssignManager.AssignID:
+            self._UpdateKey()
+        keys = self._Keys
+        value = self._Value
+        for k, v in mapper.items():
+            if k==v:
+                continue
+            value[keys[k]] = v
+        return
 
     # 2021-05-07
     def take(self, indices, copy = False):
         '''切片（重载函数）'''
         series = self._Value
         return ArrayValueIndex(
             values = series[indices],
@@ -937,14 +1076,33 @@
         '''转为pandas索引（重载函数）'''
         values = self._Value
         return pd.Index(
             data = values._ValidData,
             dtype = values.dtype,
             name = values.name,
         )
+    
+    # 2023-03-26
+    def update(self):
+        '''更新索引'''
+        value = self._Value
+        if self._AssignID==value._AssignManager.AssignID:
+            return
+        
+        i = 0
+        for v in value._ValidData:
+            if v in self._Keys:
+                self._Keys[v].append(i)
+                self._MultiValues = True
+            else:
+                self._Keys[v] = [i]
+                self._SortedKeys = None
+            i += 1
+        self._AssignID = value._AssignManager.AssignID
+        return
 
 # 2.4 多重索引类
 
 # 2021-09-26
 class ArrayMultiIndex(ArrayIndex):
     '''
     多重索引类。
@@ -1043,23 +1201,22 @@
         
         self._LevelNames = ArrayKeyIndex(self._LevelNames)
         self._LevelCount = llen
         self._LevelShape = [len(l) for l in self._Levels]
         self._LevelBase = np.ones(llen,dtype=AnsiPosDtype)
         i = llen-2
         while i>=0:
-            self._LevelBase[i] *= self._LevelShape[i+1]
+            self._LevelBase[i] = self._LevelBase[i+1]*self._LevelShape[i+1]
             i -= 1
         
         self._MultiCodes = codes[0]
         for i in range(1,llen):
             self._MultiCodes = self._MultiCodes*self._LevelShape[i]+codes[i]
         self._ValidLen = len(self._MultiCodes)
         
-        self._MultiKeys = None
         self._GenKeys()
         return
     
     # 2021-10-06
     def __getitem__(self, item):
         return item if IsSlice(item) \
             else self._MultiKeys[self._IndexToMultiCode(item)]
@@ -1114,14 +1271,19 @@
         
         if llen==1:
             return argsort(values[level[0]],ascending,na_option,method)
         else:
             return lexsort(
                 [values[l] for l in level],ascending,na_option,method)
     
+    # 2022-11-20
+    def _DropDuplicates(self, keep = 'first'):
+        '''内部去重（重载函数）'''
+        return self._MultiKeys._DropDuplicates(keep)
+    
     # 2021-10-04
     def _GenKeys(self):
         '''生成内部索引'''
         self._Keys = []
         for l in self._Levels:
             self._Keys.append(ArrayValueIndex(l))
         self._MultiKeys = ArrayValueIndex(self._MultiCodes)
@@ -1132,31 +1294,46 @@
         '''取值预处理（重载函数）'''
         if IsSlice(item):
             return item, False
         pos = self._MultiKeys[self._IndexToMultiCode(item)]
         return pos, IsSingleType(pos)
     
     # 2021-10-05
-    def _IndexToMultiCode(self, index):
-        '''普通索引转复合代码'''
+    def _IndexToMultiCode(self, index, index_kind = 'value'):
+        '''
+        普通索引转复合代码。
+        【注】索引值indexKind类型：
+          value - 返回索引值
+          code - 返回索引编码
+        '''
         if isinstance(index,ArrayFrame):
             index = index._ValidData
         elif IsDataFrame(index):
             index = index.values
         
         if IsArray(index):
             if index.ndim==1:
                 index = index.reshape((1,len(index)))
-            rt = np.array(self._Keys[0][index[:,0]],dtype=AnsiPosDtype)
-            for i in range(1,self._LevelCount):
-                rt = rt*self._LevelShape[i]+self._Keys[i][index[:,i]]
+            if index_kind=='code':
+                rt = np.array(index[:,0],dtype=AnsiPosDtype)
+                for i in range(1,self._LevelCount):
+                    rt = rt*self._LevelShape[i]+index[:,i]
+            else:
+                rt = np.array(self._Keys[0][index[:,0]],dtype=AnsiPosDtype)
+                for i in range(1,self._LevelCount):
+                    rt = rt*self._LevelShape[i]+self._Keys[i][index[:,i]]
         else:
-            rt = np.array(self._Keys[0][index[0]],dtype=AnsiPosDtype)
-            for i in range(1,self._LevelCount):
-                rt = rt*self._LevelShape[i]+self._Keys[i][index[i]]
+            if index_kind=='code':
+                rt = np.array(index[0],dtype=AnsiPosDtype)
+                for i in range(1,self._LevelCount):
+                    rt = rt*self._LevelShape[i]+index[i]
+            else:
+                rt = np.array(self._Keys[0][index[0]],dtype=AnsiPosDtype)
+                for i in range(1,self._LevelCount):
+                    rt = rt*self._LevelShape[i]+self._Keys[i][index[i]]
         return rt
     
     # 2021-10-04
     def _MultiCodeToIndex(self, codes = None, index_kind = 'value', 
         return_kind = 'list'):
         '''
         复合代码转普通索引。
@@ -1216,14 +1393,52 @@
                 self._IndexToMultiCodes(item)])
     
     # 2022-01-30
     def copy(self):
         '''拷贝（重载函数）'''
         return copy.deepcopy(self)
     
+    # 2022-11-28
+    def drop_duplicates(self, keep = 'first'):
+        '''去重（重载函数）'''
+        keys = self._MultiKeys
+        keys.update()
+        if keys._MultiValues:
+            pos, changed = keys._DropDuplicates(keep)
+            return self.take(pos) if changed else self.copy()
+        else:
+            return self.copy()
+    
+    # 2022-04-19
+    def get_iloc(self, i):
+        '''获取指定下标上的索引（重载函数）'''
+        return self._MultiCodeToIndex(self._MultiCodes[i])
+    
+    # 2022-04-26
+    def items(self):
+        '''键值对遍历器（重载函数）'''
+        return zip(self.keys(),self.pos()).__iter__()
+    
+    # 2022-04-26
+    def keys(self):
+        '''键遍历器（重载函数）'''
+        return zip(
+            *self._MultiCodeToIndex(list(self._MultiKeys.keys()))).__iter__()
+    
+    # 2022-06-04
+    def new_key_index(self):
+        '''根据索引键生成新的索引（重载函数）'''
+        return ArrayMultiIndex(self._MultiCodeToIndex(
+            list(self._MultiKeys.keys())))
+    
+    # 2022-04-26
+    def pos(self):
+        '''值下标遍历器（重载函数）'''
+        return self._MultiKeys.pos()
+    
     # 2022-02-04
     def reindex(self, index, method = 'keep', dupl_method = 'all',
         drop_index = False):
         '''
         索引（重载函数）。
         【参数表】
         index - 索引
@@ -1299,14 +1514,24 @@
         rtpos, rtindex = self._MultiKeys.reindex(
             multiCodes,method,dupl_method,drop_index)
         if rtindex is None:
             return rtpos, None
         else:
             return rtpos, self._MultiCodeToIndex(rtindex)
     
+    # 2022-08-16
+    def set_level_names(self, names):
+        '''设置标签名称'''
+        if IsSingleType(names):
+            names = [names]
+        if len(names)!=self._LevelCount:
+            raise ValueError('Level length mismatch.')
+        self._LevelNames = ArrayKeyIndex(names)
+        return
+    
     # 2021-10-06
     def take(self, indices):
         '''切片（重载函数）'''
         if IsSingleType(indices):
             indices = [indices]
         return ArrayMultiIndex(
             levels = self._MultiCodeToIndex(self._MultiCodes[indices]),
@@ -1350,18 +1575,22 @@
                 raise KeyError('{}: Label not found.'.format(l))
         self._Labels = labels    
         self._MultiLevels = len(self._Labels)>1
         return
     
     # 2022-03-05
     def __getitem__(self, item):
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
+        self.update()
         return self._Index.__getitem__(item)
     
+    # 2022-04-27
+    def __iter__(self):
+        self.update()
+        return self._Index.__iter__()
+    
     # 2022-03-04
     def __len__(self):
         if self._AssignID!=self.frame._AssignManager.AssignID:
             self._ValidLen = self.frame._ValidShape[self.axis]
         return self._ValidLen
     
     # 2022-03-03
@@ -1369,38 +1598,176 @@
         return 'FrameAxisIndex(axis={},labels={})\n'.format(
             self.axis,self._Labels)+self.frame.__repr__()
     
     # 2022-03-05
     @property
     def values(self):
         '''索引值数组'''
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
+        self.update()
         return self._Index.values
     
+    # 2022-04-28
+    def _ArgSort(self, ascending = True, na_option = 'last', method = 'first',
+        key = None, level = None):
+        '''下标排序（内部使用，重载函数）'''
+        self.update()
+        if self._MultiLevels:
+            return self._Index._ArgSort(ascending,na_option,method,key,level)
+        else:
+            return self._Index._ArgSort(ascending,na_option,method,key)
+    
+    # 2022-11-20
+    def _DropDuplicates(self, keep = 'first'):
+        '''内部去重（重载函数）'''
+        self.update()
+        return self._Index._DropDuplicates(keep)
+    
     # 2022-03-05
     def _GetPrep(self, item):
         '''取值预处理（重载函数）'''
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
+        self.update()
         return self._Index._GetPrep(item)
     
     # 2022-03-03
-    def _SetIndex(self):
-        '''设置源索引'''
+    # def _SetIndex(self):
+    #     '''设置源索引'''
+    #     axis = self.axis
+    #     frame = self.frame
+    #     labels = self._Labels
+    #     if self._MultiLevels:
+    #         if frame.empty:
+    #             values = [[] for i in range(len(labels))]
+    #         elif axis==0:
+    #             values = [frame._ValidData[:,i] for i in frame.columns[labels]]
+    #         else:
+    #             values = [frame._ValidData[i] for i in frame.index[labels]]
+    #         self._Index = ArrayMultiIndex(
+    #             levels = values,
+    #             names = labels,
+    #             sort_codes = self._SortCodes,
+    #         )
+    #     else:
+    #         col = labels[0]
+    #         if frame.empty:
+    #             data = []
+    #         elif axis==0:
+    #             data = frame._ValidData[:,frame.columns[col]]
+    #         else:
+    #             data = frame._ValidData[frame.index[col]]
+    #         values = ArraySeries(
+    #             data = data,
+    #             dtype = frame.dtype,
+    #             name = col,
+    #             auto_expand = frame._AutoExpand[axis],
+    #             expand_count = frame._ExpandCount[axis],
+    #             expand_ratio = frame._ExpandRatio[axis],
+    #             _assign_manager = frame._AssignManager,
+    #         )
+    #         self._Index = ArrayValueIndex(values)
+    #     self._AssignID = frame._AssignManager.AssignID
+    #     self._ValidLen = frame._ValidShape[axis]
+    #     return
+    
+    # 2022-03-05
+    def _SetPrep(self, item):
+        '''赋值预处理'''
+        self.update()
+        return self._Index._SetPrep(item)
+    
+    # 2022-10-23
+    def copy(self):
+        '''拷贝（重载函数）'''
+        self.update()
+        return self._Index.copy()
+    
+    # 2022-12-03
+    def drop_duplicates(self, keep = 'first'):
+        '''去重（重载函数）'''
+        self.update()
+        return self._Index.drop_duplicates()
+    
+    # 2022-04-19
+    def get_iloc(self, i):
+        '''获取指定下标上的索引（重载函数）'''
+        self.update()
+        return self._Index.get_iloc(i)
+    
+    # 2022-04-12
+    def items(self):
+        '''键值对遍历器（重载函数）'''
+        self.update()
+        return self._Index.items()
+    
+    # 2022-04-12
+    def keys(self):
+        '''键遍历器（重载函数）'''
+        self.update()
+        return self._Index.keys()
+    
+    # 2022-06-04
+    def new_key_index(self):
+        '''根据索引键生成新的索引（重载函数）'''
+        self.update()
+        return self._Index.new_key_index()
+    
+    # 2022-04-12
+    def pos(self):
+        '''键遍历器（重载函数）'''
+        self.update()
+        return self._Index.pos()
+    
+    # 2022-04-27
+    def reindex(self, index, method = 'keep', dupl_method = 'all',
+        drop_index = False):
+        '''
+        索引（重载函数）。
+        【参数表】
+        index - 索引
+        method - 索引不存在时的处理方法（参考DataFrame.reindex同名参数）
+          ffill/pad - 后向填充（取小于其的最大值）
+          bfill/backfill - 前向填充（取大于其的最小值）
+          keep - 保持空行
+          ignore - 忽略本行
+        dupl_method - 重复值处理方式
+          all - 返回全部下标
+          first - 返回首个下标
+          last - 返回最后一个下标
+        drop_index - 返回值是否不包含索引
+        '''
+        self.update()
+        return self._Index.reindex(index,method,dupl_method,drop_index)
+    
+    # 2022-03-05
+    def take(self, indices):
+        '''切片（重载函数）'''
+        self.update()
+        return self._Index.take(indices)
+    
+    # 2022-03-05
+    def to_pandas(self):
+        '''转为pandas索引'''
+        self.update()
+        return pd.Index([]) if self._Index is None else self._Index.to_pandas()
+    
+    # 2023-02-05
+    def update(self):
+        '''更新索引'''
+        if self._AssignID==self.frame._AssignManager.AssignID:
+            return
+        
         axis = self.axis
         frame = self.frame
         labels = self._Labels
         if self._MultiLevels:
             if frame.empty:
                 values = [[] for i in range(len(labels))]
             elif axis==0:
-                values = [frame._ValidData[:,i] for i in frame.index[labels]]
+                values = [frame._ValidData[:,i] for i in frame.columns[labels]]
             else:
-                values = [frame._ValidData[i] for i in frame.columns[labels]]
+                values = [frame._ValidData[i] for i in frame.index[labels]]
             self._Index = ArrayMultiIndex(
                 levels = values,
                 names = labels,
                 sort_codes = self._SortCodes,
             )
         else:
             col = labels[0]
@@ -1419,56 +1786,14 @@
                 expand_ratio = frame._ExpandRatio[axis],
                 _assign_manager = frame._AssignManager,
             )
             self._Index = ArrayValueIndex(values)
         self._AssignID = frame._AssignManager.AssignID
         self._ValidLen = frame._ValidShape[axis]
         return
-    
-    # 2022-03-05
-    def _SetPrep(self, item):
-        '''赋值预处理'''
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
-        return self._Index._SetPrep(item)
-    
-    # 2022-04-12
-    def items(self):
-        '''键值对遍历器（重载函数）'''
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
-        return self._Index.items()
-    
-    # 2022-04-12
-    def keys(self):
-        '''键遍历器（重载函数）'''
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
-        return self._Index.keys()
-    
-    # 2022-04-12
-    def pos(self):
-        '''键遍历器（重载函数）'''
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
-        return self._Index.pos()
-    
-    # 2022-03-05
-    def take(self, indices):
-        '''切片（重载函数）'''
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
-        return self._Index.take(indices)
-    
-    # 2022-03-05
-    def to_pandas(self):
-        '''转为pandas索引'''
-        if self._AssignID!=self.frame._AssignManager.AssignID:
-            self._SetIndex()
-        return pd.Index([]) if self._Index is None else self._Index.to_pandas()
 
 # 3. 数据系列
 
 # 3.1 数据系列类
 
 # 2020-11-28
 @DecorateSeries
@@ -1751,27 +2076,31 @@
             if self._AutoExpand:
                 self._Expand(targetLen)
             else:
                 targetLen = self._Len
         self._ValidLen = targetLen
         self._ValidData = self._Data[:targetLen]
         self.iloc._UpdateLen(targetLen)
+        self._AssignManager.AssignOnce()
         return
     
     # 2021-04-07
     def append(self, data, ignore_index = False, inplace = True):
         '''追加数据'''
         rt = self if inplace else self.copy()
         dlen = 1 if IsSingleType(data) else len(data)
         vlen = rt._ValidLen
         rt[vlen:(vlen+dlen)] = data
-        if not ignore_index and not rt._NoLoc \
-            and (isinstance(data,ArraySeries) and not data._NoLoc \
-                 or IsSeries(data)):
+        
+        if not ignore_index and not rt.index.simple \
+            and isinstance(data,ArraySeries) and not data.index.simple \
+            and type(rt.index)==type(data.index):
             rt.index.append(data.index)
+        else:
+            rt.set_index(rt.iloc.index)
         return rt
     
     # 2021-12-03
     def argsort(self, ascending = True, na_option = 'last', method = 'first',
         kind = None):
         pos = argsort(self._ValidData,ascending,na_option,method,kind)
         return ArraySeries(
@@ -1803,55 +2132,156 @@
                 return rt
             else:
                 return self.new_data(self._ValidData.astype(dtype),dtype)
     
     # 2021-04-07
     def copy(self):
         '''拷贝'''
-        return copy.deepcopy(self)
+        return ArraySeries(
+            data = self._ValidData,
+            index = self.index.copy(),
+            dtype = self.dtype,
+            name = self.name,
+            copy = True,
+            auto_expand = self._AutoExpand,
+            expand_count = self._ExpandCount,
+            expand_ratio = self._ExpandRatio,
+        )
+    
+    # 2022-05-14
+    def corr(self, other = None, method = 'pearson', rt_kind = 'corr'):
+        '''
+        相关系数。
+        【注】
+        1. method参数支持项：
+          pearson - Pearson相关系数
+          spearman - Spearman相关系数
+        2. rt_kind参数支持项：
+          all - 全部参数
+          corr - 相关系数
+          pvalue - p值
+        '''
+        if self.empty:
+            return (NA,NA) if rt_kind=='all' else NA
+        method = method.lower()
+        rt_kind = rt_kind.lower()
+        if other is None:
+            other = self._ValidData
+        elif isinstance(other,ArraySeries):
+            other = other._ValidData
+        if method=='spearman':
+            rt = tuple(spearmanr(self._ValidData,other))
+        else:
+            rt = pearsonr(self._ValidData,other)
+        if rt_kind=='corr':
+            return rt[0]
+        elif rt_kind=='pvalue':
+            return rt[1]
+        else:
+            return rt
     
     # 2022-04-07
     def cummax(self, skipna = True):
         '''累计最大值'''
         if self.empty:
             return ArraySeries()
-        rtdata = self._ValidData.copy()
-        pos = which(~IsNA(rtdata)) if skipna else range(self._ValidLen)
-        plen = len(pos)
-        if plen>1:
-            m = rtdata[pos[0]]
-            for p in pos[1:]:
-                if rtdata[p]>m:
-                    m = rtdata[p]
-                else:
-                    rtdata[p] = m
-        return self.new_data(rtdata)
+        
+        rtdata = self._ValidData
+        if skipna:
+            rtdata = rtdata.copy()
+            pos = which(~IsNA(rtdata))
+            if len(pos>1):
+                rtdata[pos] = np.maximum.accumulate(rtdata[pos])
+        elif len(self)>1:
+            rtdata = np.maximum.accumulate(rtdata)
+        else:
+            rtdata = rtdata.copy()
+        return self.new_data(rtdata,self.dtype)
 
     # 2022-04-07
     def cummin(self, skipna = True):
         '''累计最小值'''
         if self.empty:
             return ArraySeries()
-        rtdata = self._ValidData.copy()
-        pos = which(~IsNA(rtdata)) if skipna else range(self._ValidLen)
-        plen = len(pos)
-        if plen>1:
-            m = rtdata[pos[0]]
-            for p in pos[1:]:
-                if rtdata[p]<m:
-                    m = rtdata[p]
-                else:
-                    rtdata[p] = m
-        return self.new_data(rtdata)
+        
+        rtdata = self._ValidData
+        if skipna:
+            rtdata = rtdata.copy()
+            pos = which(~IsNA(rtdata))
+            if len(pos>1):
+                rtdata[pos] = np.minimum.accumulate(rtdata[pos])
+        elif len(self)>1:
+            rtdata = np.minimum.accumulate(rtdata)
+        else:
+            rtdata = rtdata.copy()
+        return self.new_data(rtdata,self.dtype)
+    
+    # 2022-12-03
+    def drop_duplicates(self, keep = 'first', inplace = False):
+        '''
+        去重。
+        【注】
+        1. keep参数可选项：
+           first - 仅保留首项
+           last - 仅保留尾项
+           none - 不保留任何项
+        2. 如实际发生了去重，无论inplace取何值，都将按False处理。
+        '''
+        pos, changed = ArrayValueIndex(self._ValidData)._DropDuplicates(keep)
+        if changed:
+            return self[pos]
+        else:
+            return self if inplace else self.copy()
+    
+    # 2022-12-03
+    def drop_index_duplicates(self, keep = 'first', inplace = False):
+        '''
+        索引去重。
+        【注】
+        1. keep参数可选项：
+           first - 仅保留首项
+           last - 仅保留尾项
+           none - 不保留任何项
+        2. 如实际发生了去重，无论inplace取何值，都将按False处理。
+        '''
+        pos, changed = self.index._DropDuplicates(keep)
+        if changed:
+            return self[pos]
+        else:
+            return self if inplace else self.copy()
     
     # 2022-03-24
     def dropna(self):
         '''去除缺失值'''
         return self.iloc[~IsNA(self._ValidData)]
     
+    # 2022-08-14
+    def fillna(self, value = None, method = None, inplace = False):
+        '''
+        填充缺失值。
+        【注】method参数可选项：
+        (None) - 无特殊处理
+        ffill/pad - 后向填充（取小于其的最大值）
+        bfill/backfill - 前向填充（取大于其的最小值）
+        '''
+        rtdata = self._ValidData if inplace else self._ValidData.copy()
+        if method is None:
+            if not value is None:
+                rtdata[np.isnan(rtdata)] = value
+        else:
+            if not value is None:
+                if (method=='ffill' or method=='pad') and np.isnan(rtdata[0]):
+                    rtdata[0] = value
+                elif (method=='bfill' or method=='backfill') \
+                    and np.isnan(rtdata[-1]):
+                    rtdata[-1] = value
+            rtser = Series(rtdata)
+            rtser.fillna(method=method,inplace=True)
+        return self if inplace else self.new_data(rtdata,self.dtype)
+    
     # 2022-04-03
     def groupby(self, values = None, group_keys = True):
         '''分组（返回分组对象）'''
         return ArraySeriesGroupBy(self,values,group_keys)
     
     # 2021-09-27
     def head(self, n = 5):
@@ -1870,19 +2300,42 @@
         if dtype is None:
             dtype = data.dtype if IsArray(data) else AnsiDType
         return ArraySeries(
             data = data,
             index = self.new_index(),
             dtype = dtype,
             name = self.name,
+            init_len = self._InitLen,
             auto_expand = self._AutoExpand,
             expand_count = self._ExpandCount,
             expand_ratio = self._ExpandRatio,
         )
     
+    # 2022-04-19
+    def max_retreat(self, rtnfields = 'All'):
+        '''
+        最大回撤函数。
+        【注】rtnfields参数允许的返回字段包括：
+          All - 返回全部结果
+          MaxRetreat - 最大回撤值
+          RetreatStart - 最大回撤起始索引
+          RetreatEnd - 最大回撤结束索引
+          Recovered - 是否创新高
+          RecoverCount - 最长未创新高期数
+          RecoverStart - 最长未创新高起始索引
+          RecoverEnd - 最长未创新高结束索引
+        '''
+        rt = MaxRetreat(self,rtnfields)
+        index = self.index
+        if not index.simple:
+            for f in ['RetreatStart','RetreatEnd','RecoverStart','RecoverEnd']:
+                if f in rt:
+                    rt[f] = index.get_iloc(rt[f])
+        return rt
+    
     # 2022-03-06
     def new_index(self):
         '''创建新索引'''
         index = self.index
         return index._Index if isinstance(index,FrameAxisIndex) else index
     
     # 2022-03-30
@@ -1996,15 +2449,15 @@
     def sort_index(self, ascending = True, na_position = 'last',
         method = 'first', axis = 0, level = None, inplace = False, key = None):
         '''
         索引排序。
         【注】simple类索引不进行此类排序。
         '''
         index = self.index
-        if index.simple:
+        if self.empty or index.simple:
             return self if inplace else self.copy()
         if isinstance(index,ArrayMultiIndex):
             pos = index._ArgSort(ascending,na_position,method,key,level)
         else:
             pos = index._ArgSort(ascending,na_position,method,key)
         if inplace:
             self._ValidData[:,:] = self._ValidData[pos,:]
@@ -2013,14 +2466,17 @@
         else:
             return self.iloc[pos]
     
     # 2021-10-24
     def sort_values(self, ascending = True, na_position = 'last', 
         method = 'first', kind = None, inplace = False, key = None):
         '''值排序'''
+        if self.empty:
+            return self if inplace else self.copy()
+        
         values = self._ValidData
         if not key is None:
             values = key(values)
         pos = argsort(values,ascending,na_position,method,kind)
         
         if inplace:
             self._ValidData[:] = self._ValidData[pos]
@@ -2053,17 +2509,111 @@
             data = self._ValidData,
             index = self.index.to_pandas(),
             dtype = self.dtype,
             name = self.name,
         )
     
     # 2022-03-19
-    def unique(self):
-        '''取去重值'''
-        return np.unique(self._ValidData)
+    def unique(self, order = 'keep', rt_kind = 'array'):
+        '''
+        取去重值。
+        【注】
+        1. order参数取值：
+           keep - 保持原有顺序
+           sort - 排序
+        2. rt_kind参数取值：
+           array - np.ndarray
+           list - list
+        '''
+        rt = list(collections.OrderedDict.fromkeys(self._ValidData))
+        if order=='sort':
+            rt = sorted(rt)
+        return np.array(rt) if rt_kind=='array' else rt
+    
+    # 2022-03-19
+    def unstack(self, level = -1, fill_value = None, order = None):
+        '''逆堆叠'''
+        if self.empty:
+            return ArrayFrame()
+        index = self.index
+        if isinstance(index,FrameAxisIndex):
+            index.update()
+            index = index._Index
+        if order is None:
+            order = AnsiOrder
+        
+        if isinstance(index,ArrayMultiIndex):
+            codes = index._MultiCodeToIndex(index_kind='code')
+            
+            lcount = index._LevelCount
+            if IsInteger(level):
+                clevel = [level%lcount]
+            else:
+                clevel = [l%lcount for l in level]
+            rlevel = posdiff(lcount,clevel)
+            cllen = len(clevel)
+            rllen = len(rlevel)
+            
+            if cllen==1:
+                clist = unique(codes[clevel[0]])
+                rtcolumns = index._Levels[clevel[0]][clist]
+            else:
+                clist = ListProduct(*[unique(codes[l]) for l in clevel],
+                    order=order,rtOrder='C')
+                carr = np.array(clist,AnsiPosDtype)
+                rtcolumns = [index._Levels[clevel[i]][carr[:,i]] 
+                    for i in range(cllen)]
+            if rllen==0:
+                rlist = None
+                rtindex = None
+                fullindex = np.ndarray((len(clist),lcount),object)
+                fullindex[:,clevel] = np.array(clist)
+            else:
+                if rllen==1:
+                    rlist = unique(codes[rlevel[0]])
+                    rtindex = index._Levels[rlevel[0]][rlist]
+                else:
+                    rlist = unique(zip(*[codes[l] for l in rlevel]))
+                    rarr = np.array(rlist,AnsiPosDtype)
+                    rtindex = [index._Levels[rlevel[i]][rarr[:,i]] 
+                        for i in range(rllen)]
+                fulllist = ListProduct(rlist,clist,order=order)
+                
+                fullindex = np.ndarray((len(fulllist[0]),lcount),object)
+                if cllen==1:
+                    fullindex[:,clevel[0]] = fulllist[1]
+                else:
+                    fullindex[:,clevel] = np.array(fulllist[1])
+                if rllen==1:
+                    fullindex[:,rlevel[0]] = fulllist[0]
+                else:
+                    fullindex[:,rlevel] = np.array(fulllist[0])
+            
+            multicodes = index._IndexToMultiCode(fullindex,'code')
+            multiloc = ArraySeriesLocIndexer(self,index._MultiKeys)
+            rtseries = multiloc.reindex(
+                multicodes,'keep',fill_value,'first',True)
+            return ArrayFrame(
+                data = rtseries._ValidData.reshape(
+                    (1 if rlist is None else len(rlist),len(clist)),
+                    order = order,
+                ),
+                index = rtindex,
+                columns = rtcolumns,
+                dtype = self.dtype,
+            )
+        else:
+            return ArrayFrame(
+                data = self._ValidData.reshape((1,self._ValidLen),order=order),
+                columns = self.new_index(),
+                dtype = self.dtype,
+                auto_expand = (AnsiAutoExpand,self._AutoExpand),
+                expand_count = (AnsiExpandCount,self._ExpandCount),
+                expand_ratio = (AnsiExpandRatio,self._ExpandRatio),
+            )
 
 # 3.2 数据系列索引器类
 
 # 2021-03-28
 class ArraySeriesLocIndexer:
     '''
     数据系列Loc索引器类。
@@ -2165,21 +2715,23 @@
         pplen = len(ppos)
         if plen==0:
             rtdata = None
             rtindex = None
         elif pplen==plen:
             rtdata = series._ValidData[pos]
         else:
-            rtdata = np.repeat(fill_value,plen).astype(series.dtype)
+            rtdata = np.repeat(fill_value,plen)
+            if type(fill_value)!=series.dtype:
+                rtdata = rtdata.astype(object)
             if pplen>0:
                 rtdata[ppos] = series._ValidData[pos[ppos]]
         return ArraySeries(
             data = rtdata,
             index = rtindex,
-            dtype = series.dtype,
+            dtype = rtdata.dtype,
             name = series.name,
             auto_expand = series._AutoExpand,
             expand_count = series._ExpandCount,
             expand_ratio = series._ExpandRatio,
         )
     
     # 2021-07-19
@@ -2190,15 +2742,15 @@
             self.index = series.iloc.index if hasattr(series,'iloc') \
                 else ArrayIndex(len(series))
             return
         
         if isinstance(index,ArrayIndex):
             if len(index)!=series._ValidLen:
                 raise ValueError('Index size mismatch.')
-            self.index = copy.deepcopy(index) if copy else index
+            self.index = index.copy() if copy else index
         elif IsSingleType(index):
             if series._ValidLen!=1:
                 raise ValueError('Index size mismatch.')
             self.index = ArrayValueIndex(index)
         elif IsIndex(index):
             if len(index)!=series._ValidLen:
                 raise ValueError('Index size mismatch.')
@@ -2224,18 +2776,23 @@
                 copy = copy,
                 auto_expand = series._AutoExpand,
                 expand_count = series._ExpandCount,
                 expand_ratio = series._ExpandRatio,
                 _assign_manager = _assign_manager
             )
         else:
-            vlen = series._ValidLen
-            for i in range(len(index)):
-                if len(index[i])!=vlen:
-                    raise ValueError('Index size mismatch.')
+            if IsArray(index):
+                vlen = len(index)
+            else:
+                vlen = len(index[0])
+                for i in range(1,len(index)):
+                    if len(index[i])!=vlen:
+                        raise ValueError('Index size mismatch.')
+            if series._ValidLen!=vlen:
+                raise ValueError('Index size mismatch.')
             self.index = ArrayMultiIndex(index)
         return
 
 # 4. 数据表
 
 # 4.1 数据表类
 
@@ -2350,17 +2907,17 @@
             if expand_count is None:
                 expand_count = data._ExpandCount
             if expand_ratio is None:
                 expand_ratio = data._ExpandRatio
             if not copy:
                 _assign_manager = data._AssignManager
             if not drop_index and index is None and index_cols is None:
-                index, index_cols = self.new_index()
+                index, index_cols = data.new_index()
             if not drop_columns and columns is None and col_index is None:
-                columns, col_index = self.new_columns()
+                columns, col_index = data.new_columns()
             data = data._ValidData
         elif isinstance(data,ArraySeries):
             if dtype is None:
                 dtype = data.dtype
             if init_shape is None:
                 init_shape = (len(data),1)
             if auto_expand is None:
@@ -2424,48 +2981,57 @@
         columns = self.columns
         if name in columns:
             if len(self)==1:
                 return self._ValidData[0,columns[name]]
             else:
                 return ArraySeries(
                     data = self._ValidData[:,columns[name]],
-                    index = self.index,
+                    index = self.new_index(False)[0],
                     dtype = self.dtype,
                     name = name,
                     auto_expand = self._AutoExpand[0],
                     expand_count = self._ExpandCount[0],
                     expand_ratio = self._ExpandRatio[0],
                     _assign_manager = self._AssignManager
                 )
         else:
             return super().__getattribute__(name)
     
     # 2021-06-15
     def __getitem__(self, item):
+        if self._ValidData is None:
+            return ArraySeries(
+                dtype = self.dtype,
+                name = item,
+                auto_expand = self._AutoExpand[0],
+                expand_count = self._ExpandCount[0],
+                expand_ratio = self._ExpandRatio[0],
+            )
+        
         columns = self.columns
         simple = columns.simple
         pitem = item if simple else columns[item]
         data = self._ValidData[:,pitem]
         
         if data.ndim==1:
             return ArraySeries(
                 data = data,
-                index = self.index,
+                index = self.new_index(False)[0],
                 dtype = data.dtype,
                 name = None if simple else item,
                 auto_expand = self._AutoExpand[0],
                 expand_count = self._ExpandCount[0],
                 expand_ratio = self._ExpandRatio[0],
                 _assign_manager = None if data.flags.owndata \
                     else self._AssignManager
             )
         else:
             return ArrayFrame(
                 data = data,
-                index = self.index,
+                index = self.new_index(False)[0],
                 columns = None if simple else columns.take(pitem),
                 dtype = self.dtype,
                 auto_expand = self._AutoExpand,
                 expand_count = self._ExpandCount,
                 expand_ratio = self._ExpandRatio,
                 _assign_manager = None if data.flags.owndata \
                     else self._AssignManager
@@ -2549,18 +3115,24 @@
             return
         
         shape = self._Shape
         validShape = self._ValidShape
         expandCount = self._ExpandCount
         expandRatio = self._ExpandRatio
         
-        newx = ExpandSize(
-            shape[0],targetShape[0],expandCount[0],expandRatio[0])
-        newy = ExpandSize(
-            shape[1],targetShape[1],expandCount[1],expandRatio[1])
+        if targetShape[0]>shape[0]:
+            newx = ExpandSize(
+                shape[0],targetShape[0],expandCount[0],expandRatio[0])
+        else:
+            newx = shape[0]
+        if targetShape[1]>shape[1]:
+            newy = ExpandSize(
+                shape[1],targetShape[1],expandCount[1],expandRatio[1])
+        else:
+            newy = shape[1]
         newdata = np.ndarray((newx,newy),self.dtype,order=order)
         newdata[:validShape[0],:validShape[1]] = self._ValidData
         self._Data = newdata
         self._AssignManager = AssignManager(self._AssignManager.AssignID)
         self._ValidData = newdata[:validShape[0],:validShape[1]]
         self._Shape = (newx,newy)
         return
@@ -2621,16 +3193,15 @@
         if index is None and not index_cols is None:
             self.loc.set_axis_index(index_cols,0,copy)
             self.index = self.loc.index
         if columns is None and not col_index is None:
             self.loc.set_axis_index(col_index,1,copy)
             self.columns = self.loc.columns
         
-        self.ix = ArrayFrameLocIndexer(self,self.iloc.index,self.columns,
-            copy=copy)
+        self.ix = ArrayFrameLocIndexer(self,self.iloc.index,self.columns)
         return
     
     # 2021-12-17
     def _UpdateEmptyAxisLen(self, axis, targetLen):
         '''更新空表轴长度（不改变数组内容，内部使用）'''
         if axis==0:
             self._Shape = (targetLen,0)
@@ -2653,36 +3224,42 @@
                     targetShape = list(targetShape)
                     targetShape[i] = self._Shape[i]
         if needExpand:
             self._Expand(targetShape)
         self._ValidData = self._Data[:targetShape[0],:targetShape[1]]
         self._ValidShape = targetShape
         self.iloc._UpdateValidShape(targetShape)
+        self._AssignManager.AssignOnce()
         return
     
     # 2022-01-30
     def append(self, data, ignore_index = False, inplace = True):
         '''追加数据'''
         rt = self if inplace else self.copy()
         vlen = self._ValidShape[0]
         
         if isinstance(data,ArrayFrame):
             if data._ValidShape[1]!=self._ValidShape[1]:
                 raise ValueError('Column size mismatch.')
             rt.iloc[vlen:(vlen+data._ValidShape[0])] = data._ValidData
-            if not ignore_index and not rt.index.simple \
-                and not data.index.simple:
-                rt.index.append(data.index.values)
+            if not isinstance(rt.index,FrameAxisIndex):
+                # FrameAxisIndex不需处理
+                if not ignore_index and type(rt.index)==type(data.index) \
+                    and not rt.index.simple and not data.index.simple:
+                    rt.index.append(data.index.values)
+                else:
+                    rt.set_index(rt.iloc.index)
             return rt
         elif IsDataFrame(data):
             if data.shape[1]!=self._ValidShape[1]:
                 raise ValueError('Column size mismatch.')
             rt.iloc[vlen:(vlen+data._ValidShape[0])] = data
-            if not ignore_index and not rt.index.simple:
-                rt.index.append(data.index.values)
+            if not isinstance(rt.index,FrameAxisIndex):
+                # FrameAxisIndex不需处理
+                rt.set_index(rt.iloc.index)
             return rt
         
         if IsSingleType2(data):
             dlen = 1
         elif IsSingleType2(data[0]):
             if len(data)!=self._ValidShape[1]:
                 raise ValueError('Column size mismatch.')
@@ -2713,25 +3290,165 @@
                     rt.dtype = dtype
                 return rt
             else:
                 return self.new_data(self._ValidData.astype(dtype),dtype)
 
     # 2021-09-25
     def copy(self):
+        index, index_cols = self.new_index()
+        columns, col_index = self.new_columns()
         return ArrayFrame(
             data = self._ValidData,
-            index = self.index,
-            columns = self.columns,
+            index = index,
+            columns = columns,
+            index_cols = index_cols,
+            col_index = col_index,
             dtype = self.dtype,
             copy = True,
             auto_expand = self._AutoExpand,
             expand_count = self._ExpandCount,
             expand_ratio = self._ExpandRatio
         )
     
+    # 2022-05-22
+    def corr(self, other = None, columns = None, axis = 0, method = 'pearson',
+        rt_kind = 'corr'):
+        '''
+        相关系数。
+        【注】
+        1. method参数支持项：
+          pearson - Pearson相关系数
+          spearman - Spearman相关系数
+        2. rt_kind参数支持项：
+          all - 全部参数
+          corr - 相关系数
+          pvalue - p值
+        '''
+        if self.empty:
+            return (NA,NA) if rt_kind=='all' else NA
+        method = method.lower()
+        rt_kind = rt_kind.lower()
+        if method=='spearman':
+            func = lambda x, y: tuple(spearmanr(x,y))
+        else:
+            func = pearsonr
+        
+        if other is None:
+            other = self
+            odata = self._ValidData
+        elif isinstance(other,ArraySeries) or isinstance(other,ArrayFrame):
+            odata = other._ValidData
+        elif IsSeries(other) or IsDataFrame(other):
+            odata = other.values
+        else:
+            odata = other
+        oframe = IsArray(odata) and odata.ndim==2
+        olen = odata.shape[axis] if oframe else len(odata)
+        if self._ValidShape[axis]!=olen:
+            raise ValueError('Data size mismatch.')
+        
+        data = self._ValidData
+        if axis==0:
+            cpos = range(len(self.columns)) if columns is None \
+                else self.columns[columns]
+            if IsInteger(cpos):
+                if oframe:
+                    return other.corr(data[:,cpos],None,axis,method,rt_kind)
+                else:
+                    return self.iloc[:,cpos].corr(odata,method,rt_kind)
+            clen = len(cpos)
+            rtcolumns = self.columns.take(cpos)
+            if oframe:
+                rtindex, _ = other.new_columns(False)
+                rlen = other._ValidShape[1]
+                rtdata = ArrayFrame(
+                    index = rtindex,
+                    columns = rtcolumns,
+                    init_shape = (rlen,clen),
+                )
+                rtdata.iloc[:rlen,:clen] = NA
+                if rt_kind=='all':
+                    rtdata = (rtdata,rtdata.copy())
+                    for i in range(rlen):
+                        for j in range(clen):
+                            rt = func(odata[:,i],data[:,cpos[j]])
+                            rtdata[0].iloc[i,j] = rt[0]
+                            rtdata[1].iloc[i,j] = rt[1]
+                else:
+                    rtpos = 1 if rt_kind=='pvalue' else 0
+                    for i in range(rlen):
+                        for j in range(clen):
+                            rtdata.iloc[i,j] = func(
+                                odata[:,i],data[:,cpos[j]])[rtpos]
+            else:
+                rtdata = ArraySeries(
+                    data = np.repeat(NA,clen),
+                    index = rtcolumns,
+                )
+                if rt_kind=='all':
+                    rtdata = (rtdata,rtdata.copy())
+                    for i in range(clen):
+                        rt = func(data[:,cpos[i]],odata)
+                        rtdata[0][i] = rt[0]
+                        rtdata[1][i] = rt[1]
+                else:
+                    rtpos = 1 if rt_kind=='pvalue' else 0
+                    for i in range(clen):
+                        rtdata[i] = func(data[:,cpos[i]],odata)[rtpos]
+        else:
+            if columns is None:
+                rpos = range(len(self.index))
+            else:
+                rpos = self.index[columns]
+            if IsInteger(rpos):
+                if oframe:
+                    return other.corr(data[rpos],None,axis,method,rt_kind)
+                else:
+                    rpos = [rpos]
+            rlen = len(rpos)
+            rtindex = self.index.take(rpos)
+            if oframe:
+                rtcolumns, _ = other.new_index(False)
+                clen = other._ValidShape[0]
+                rtdata = ArrayFrame(
+                    index = rtindex,
+                    columns = rtcolumns,
+                    init_shape = (rlen,clen),
+                )
+                rtdata.iloc[:rlen,:clen] = NA
+                if rt_kind=='all':
+                    rtdata = (rtdata,rtdata.coyp())
+                    for i in range(rlen):
+                        for j in range(clen):
+                            rt = func(data[rpos[i]],odata[j])
+                            rtdata[0].iloc[i,j] = rt[0]
+                            rtdata[1].iloc[i,j] = rt[1]
+                else:
+                    rtpos = 1 if rt_kind=='pvalue' else 0
+                    for i in range(rlen):
+                        for j in range(clen):
+                            rtdata.iloc[i,j] = func(
+                                data[rpos[i]],odata[j])[rtpos]
+            else:
+                rtdata = ArraySeries(
+                    data = np.repeat(NA,rlen),
+                    index = rtindex,
+                )
+                if rt_kind=='all':
+                    rtdata = (rtdata,rtdata.copy())
+                    for i in range(rlen):
+                        rt = func(data[i],odata)
+                        rtdata[0][i] = rt[0]
+                        rtdata[1][i] = rt[1]
+                else:
+                    rtpos = 1 if rt_kind=='pvalue' else 0
+                    for i in range(rlen):
+                        rtdata[i] = func(data[i],odata)[rtpos]
+        return rtdata
+    
     # 2022-04-07
     def cummax(self, columns = None, axis = 0, skipna = True):
         '''累计最大值'''
         if self.empty:
             return self.copy()
         rtdata = self._ValidData.copy()
         if not columns is None and IsSingleType(columns):
@@ -2876,14 +3593,76 @@
                 col_index = rtcol_index,
                 dtype = self.dtype,
                 auto_expand = self._AutoExpand,
                 expand_count = self._ExpandCount,
                 expand_ratio = self._ExpandRatio,
             )
     
+    # 2022-06-21
+    def dropna(self, columns = None, axis = 0, how = 'any', thresh = None):
+        '''去除缺失值'''
+        if self.empty:
+            return self.copy()
+        if not columns is None:
+            if axis==0:
+                if IsSingleType(columns):
+                    columns = [columns]
+                return self[columns].dropna(None,0,how,thresh)
+            else:
+                return self.iloc[columns].dropna(None,1,how,thresh)
+        
+        isna = DataFrame(self._ValidData).isna().values
+        if axis==0:
+            if thresh is None:
+                if how=='any':
+                    return self.iloc[~np.any(isna,1)]
+                else:
+                    return self.iloc[~np.all(isna,1)]
+            else:
+                return self.iloc[isna.sum(1)<thresh]
+        else:
+            if thresh is None:
+                if how=='any':
+                    return self.iloc[:,~np.any(isna,0)]
+                else:
+                    return self.iloc[:,~np.all(isna,0)]
+            else:
+                return self.iloc[:,isna.sum(0)<thresh]
+    
+    # 2022-08-21
+    def fillna(self, value = None, method = None, axis = 0, inplace = False):
+        '''
+        填充缺失值。
+        【注】method参数可选项：
+        (None) - 无特殊处理
+        ffill/pad - 后向填充（取小于其的最大值）
+        bfill/backfill - 前向填充（取大于其的最小值）
+        '''
+        rtdata = self._ValidData if inplace else self._ValidData.copy()
+        if method is None:
+            if not value is None:
+                rtdata[np.isnan(rtdata)] = value
+        else:
+            if not value is None:
+                if method=='ffill' or method=='pad':
+                    cpos = 0
+                else:
+                    cpos = -1
+                if axis==0:
+                    pos = which(np.isnan(rtdata[cpos]))
+                    if len(pos)>0:
+                        rtdata[cpos,pos] = value
+                else:
+                    pos = which(np.isnan(rtdata[:,cpos]))
+                    if len(pos)>0:
+                        rtdata[pos,cpos] = value
+            rtdf = DataFrame(rtdata)
+            rtdf.fillna(method=method,axis=axis,inplace=True)
+        return self if inplace else self.new_data(rtdf.values,self.dtype)
+    
     # 2022-04-10
     def groupby(self, by = None, values = None, axis = 0, group_keys = True):
         '''分组（返回分组对象）'''
         return ArrayFrameGroupBy(self,by,values,axis,group_keys)
     
     # 2021-09-27
     def head(self, n = 5):
@@ -3097,48 +3876,55 @@
         method = 'first', axis = 0, level = None, inplace = False, key = None):
         '''
         索引排序。
         【注】simple类索引不进行此类排序。
         '''
         if axis==0:
             index = self.index
-            if index.simple:
+            if self.empty or index.simple:
                 return self if inplace else self.copy()
             if isinstance(index,ArrayMultiIndex):
                 pos = index._ArgSort(ascending,na_position,method,key,level)
             else:
                 pos = index._ArgSort(ascending,na_position,method,key)
             if inplace:
                 self._ValidData[:,:] = self._ValidData[pos,:]
-                self.set_index(index.take(pos))
+                self._AssignManager.AssignOnce()
+                if not index.simple and isinstance(index,FrameAxisIndex):
+                    self.set_index(index.take(pos))
                 return self
             else:
                 return self.iloc[pos]
         else:
             columns = self.columns
-            if columns.simple:
+            if self.empty or columns.simple:
                 return self if inplace else self.copy()
             if isinstance(columns,ArrayMultiIndex):
                 pos = columns._ArgSort(ascending,na_position,method,key,level)
             else:
                 pos = columns._ArgSort(ascending,na_position,method,key)
             if inplace:
                 self._ValidData[:,:] = self._ValidData[:,pos]
-                self.set_columns(columns.take(pos))
+                self._AssignManager.AssignOnce()
+                if not columns.simple \
+                    and not isinstance(columns,FrameAxisIndex):
+                    self.set_columns(columns.take(pos))
                 return self
             else:
                 return self.iloc[:,pos]
     
     # 2021-12-14
     def sort_values(self, by = None, ascending = True, na_position = 'last',
         method = 'first', axis = 0, inplace = False, key = None):
         '''
         值排序。
         【注】函数参数意义同DataFrame.sort_values对应参数。
         '''
+        if self.empty:
+            return self if inplace else self.copy()
         index = self.index
         columns = self.columns
         if axis==0:
             if by is None:
                 by = columns.values
             if IsSingleType(by):
                 values = self._ValidData[:,columns[by]]
@@ -3175,15 +3961,16 @@
                             v = key(v)
                     values.append(v)
                     i += 1
                 pos = lexsort(values,asc,na,method)
             
             if inplace:
                 self._ValidData[:,:] = self._ValidData[pos,:]
-                if not index.simple:
+                self._AssignManager.AssignOnce()
+                if not index.simple and not isinstance(index,FrameAxisIndex):
                     self.set_index(index.take(pos))
                 return self
             else:
                 return self.iloc[pos]
         else:
             if by is None:
                 by = index.values
@@ -3222,21 +4009,126 @@
                             v = key(v)
                     values.append(v)
                     i += 1
                 pos = lexsort(values,asc,na,method)
             
             if inplace:
                 self._ValidData[:,:] = self._ValidData[:,pos]
-                if not columns.simple:
+                self._AssignManager.AssignOnce()
+                if not columns.simple \
+                    and not isinstance(columns,FrameAxisIndex):
                     self.set_columns(columns.take(pos))
                 return self
             else:
                 return self.iloc[:,pos]
         return
     
+    # 2022-06-23
+    def stack(self, level = -1, fill_value = None, dropna = True, order = None):
+        '''堆叠'''
+        if self.empty:
+            return ArraySeries()
+        columns = self.columns
+        if isinstance(columns,FrameAxisIndex):
+            columns.update()
+            columns = columns._Index
+        if order is None:
+            order = AnsiOrder
+        
+        if isinstance(columns,ArrayMultiIndex):
+            codes = columns._MultiCodeToIndex(index_kind='code')
+            
+            lcount = columns._LevelCount
+            if IsInteger(level):
+                mlevel = [level%lcount]
+            else:
+                mlevel = [l%lcount for l in level]
+            clevel = posdiff(lcount,mlevel)
+            mllen = len(mlevel)
+            cllen = len(clevel)
+            
+            if mllen==1:
+                mlist = unique(codes[mlevel[0]])
+            else:
+                mlist = ListProduct(*[unique(codes[l]) for l in mlevel],
+                    order=order,rtOrder='C')
+            if cllen==0:
+                clist = None
+                rtcolumns = None
+                if mllen==1:
+                    fcolumns = mlist
+                else:
+                    fcolumns = np.ndarray((len(mlist),lcount),AnsiPosDtype)
+                    fcolumns[:,mlevel] = np.array(mlist)
+            else:
+                if cllen==1:
+                    clist = unique(codes[clevel[0]])
+                    rtcolumns = columns._Levels[clevel[0]][clist]
+                else:
+                    clist = unique(zip(*[codes[l] for l in clevel]))
+                    carr = np.array(clist,AnsiPosDtype)
+                    rtcolumns = [columns._Levels[clevel[i]][carr[:,i]] 
+                        for i in range(cllen)]
+                flist = ListProduct(clist,mlist,order=order)
+            
+                fcolumns = np.ndarray((len(flist[0]),lcount),object)
+                if mllen==1:
+                    fcolumns[:,mlevel[0]] = flist[1]
+                else:
+                    fcolumns[:,mlevel] = np.array(flist[1],object)
+                if cllen==1:
+                    fcolumns[:,clevel[0]] = flist[0]
+                elif cllen>1:
+                    fcolumns[:,clevel] = np.array(flist[0],object)
+            
+            multicodes = columns._IndexToMultiCode(fcolumns,'code')
+            
+            if mllen==1:
+                mcolumns = columns._Levels[mlevel[0]][mlist]
+            else:
+                mcolumns = [[columns._Levels[mlevel[i]][m[i]] 
+                    for i in range(mllen)] for m in mlist]
+            
+            multiloc = ArrayFrameLocIndexer(self,self.index,columns._MultiKeys)
+            rtdata = multiloc.reindex(
+                None,multicodes,'keep',fill_value,'first',True,1)._ValidData
+        else:
+            clist = None
+            mllen = 1
+            mcolumns = columns
+            rtdata = self._ValidData.copy()
+        
+        rlist = list(self.index.keys())
+        r0 = rlist[0]
+        rsingle = IsSingleType(r0)
+        rllen = 1 if rsingle else len(r0)
+        rorder = 'C' if order=='F' else 'F'
+        findex = ListProduct(rlist,mcolumns,order=rorder)
+        rtindex = np.ndarray((len(findex[0]),rllen+mllen),object)
+        if rllen==1:
+            rtindex[:,0] = findex[0]
+        else:
+            rtindex[:,:rllen] = np.array(findex[0],object)
+        if mllen==1:
+            rtindex[:,rllen] = findex[1]
+        else:
+            rtindex[:,rllen:(rllen+mllen)] = np.array(findex[1],object)
+        
+        if clist is None:
+            return ArraySeries(
+                data = rtdata.reshape(len(rtindex)),
+                index = rtindex,
+            )
+        else:
+            return ArrayFrame(
+                data = rtdata.reshape((len(rtindex),len(clist)),order=rorder),
+                index = rtindex,
+                columns = rtcolumns,
+            )
+    
     # 2022-04-14
     def std(self, columns = None, axis = 0, skipna = True, ddof = 1, **kwargs):
         '''统计函数，参见numpy同名函数'''
         data = self._ValidData
         if not columns is None and not axis is None:
             if IsSingleType(columns):
                 columns = [columns]
@@ -3260,14 +4152,43 @@
             return self.new_aggr_data(rt,axis,'std',columns=columns)
     
     # 2021-09-27
     def tail(self, n = 5):
         '''返回后n行'''
         return self.iloc[-n:]
     
+    # 2022-11-05
+    def to_csv(self, path_or_buf, sep = ',', na_rep = 'NA', header = True,
+        index = True, encoding = None, **kwargs):
+        '''输出为csv文件'''
+        self.to_pandas().to_csv(
+            path_or_buf = path_or_buf,
+            sep = sep,
+            na_rep = na_rep,
+            header = header,
+            index = index,
+            encoding = encoding,
+            **kwargs,
+        )
+        return
+    
+    # 2022-05-26
+    def to_excel(self, excel_writer, sheet_name = 'Sheet1', na_rep = 'NA',
+        header = True, index = False, **kwargs):
+        '''输出为Excel文件'''
+        self.to_pandas().to_excel(
+            excel_writer,
+            sheet_name,
+            na_rep,
+            header = header,
+            index = index,
+            **kwargs,
+        )
+        return
+    
     # 2022-02-26
     def to_pandas(self):
         '''转为pandas.DataFrame'''
         return DataFrame(
             data = self._ValidData,
             index = self.index.to_pandas(),
             columns = self.columns.to_pandas(),
@@ -3289,14 +4210,118 @@
             copy = copy,
             init_shape = (self._InitShape[1],self._InitShape[0]),
             auto_expand = (self._AutoExpand[1],self._AutoExpand[0]),
             expand_count = (self._ExpandCount[1],self._ExpandCount[0]),
             expand_ratio = (self._ExpandRatio[1],self._ExpandRatio[0]),
             _assign_manager = self._AssignManager
         )
+    
+    # 2022-06-08
+    def unstack(self, level = -1, fill_value = None, order = None):
+        '''逆堆叠'''
+        if self.empty:
+            return ArraySeries()
+        index = self.index
+        if isinstance(index,FrameAxisIndex):
+            index.update()
+            index = index._Index
+        if order is None:
+            order = AnsiOrder
+        
+        if isinstance(index,ArrayMultiIndex):
+            codes = index._MultiCodeToIndex(index_kind='code')
+            
+            lcount = index._LevelCount
+            if IsInteger(level):
+                mlevel = [level%lcount]
+            else:
+                mlevel = [l%lcount for l in level]
+            rlevel = posdiff(lcount,mlevel)
+            mllen = len(mlevel)
+            rllen = len(rlevel)
+            
+            if mllen==1:
+                mlist = unique(codes[mlevel[0]])
+            else:
+                mlist = ListProduct(*[unique(codes[l]) for l in mlevel],
+                    order=order,rtOrder='C')
+            if rllen==0:
+                rlist = None
+                rtindex = None
+                if mllen==1:
+                    findex = mlist
+                else:
+                    findex = np.ndarray((len(mlist),lcount),AnsiPosDtype)
+                    findex[:,mlevel] = np.array(mlist)
+            else:
+                if rllen==1:
+                    rlist = unique(codes[rlevel[0]])
+                    rtindex = index._Levels[rlevel[0]][rlist]
+                else:
+                    rlist = unique(zip(*[codes[l] for l in rlevel]))
+                    rarr = np.array(rlist,AnsiPosDtype)
+                    rtindex = [index._Levels[rlevel[i]][rarr[:,i]] 
+                        for i in range(rllen)]
+                flist = ListProduct(rlist,mlist,order=order)
+                
+                findex = np.ndarray((len(flist[0]),lcount),object)
+                if mllen==1:
+                    findex[:,mlevel[0]] = flist[1]
+                else:
+                    findex[:,mlevel] = np.array(flist[1],object)
+                if rllen==1:
+                    findex[:,rlevel[0]] = flist[0]
+                else:
+                    findex[:,rlevel] = np.array(flist[0],object)
+            
+            multicodes = index._IndexToMultiCode(findex,'code')
+            
+            if mllen==1:
+                mindex = index._Levels[mlevel[0]][mlist]
+            else:
+                mindex = [[index._Levels[mlevel[i]][m[i]] 
+                    for i in range(mllen)] for m in mlist]
+            
+            multiloc = ArrayFrameLocIndexer(self,index._MultiKeys,self.columns)
+            rtdata = multiloc.reindex(
+                multicodes,None,'keep',fill_value,'first',True)._ValidData
+        else:
+            rlist = None
+            mllen = 1
+            mindex = index
+            rtdata = self._ValidData.copy()
+            
+        clist = list(self.columns.keys())
+        c0 = clist[0]
+        csingle = IsSingleType(c0)
+        cllen = 1 if csingle else len(c0)
+        corder = 'C' if order=='F' else 'F'
+        fcolumns = ListProduct(clist,mindex,order=corder)
+        rtcolumns = np.ndarray((len(fcolumns[0]),cllen+mllen),object)
+        if cllen==1:
+            rtcolumns[:,0] = fcolumns[0]
+        else:
+            rtcolumns[:,:cllen] = np.array(fcolumns[0])
+        if mllen==1:
+            rtcolumns[:,cllen] = fcolumns[1]
+        else:
+            rtcolumns[:,cllen:(cllen+mllen)] = np.array(fcolumns[1])
+        
+        if rlist is None:
+            return ArraySeries(
+                data = rtdata.reshape(len(rtcolumns)),
+                index = rtcolumns,
+            )
+        else:
+            return ArrayFrame(
+                data = rtdata.reshape(
+                    (len(rlist),len(rtcolumns)),order=order),
+                index = rtindex,
+                columns = rtcolumns,
+            )
 
 # 4.2 数据表索引器类
 
 # 2021-05-27
 class ArrayFrameLocIndexer:
     '''
     数据表Loc索引器类。
@@ -3307,54 +4332,56 @@
         copy = False, iloc = False):
         if not isinstance(frame,ArrayFrame):
             raise TypeError('ArrayFrame required.') 
         self.frame = frame
         self._ILoc = iloc
         self.set_index(index,0,copy)
         self.set_index(columns,1,copy)
-        
-        # if index is None:
-        #     col_index = None
-        #     if columns is None:
-        #         index_cols = None
-        #     self.set_index(columns,col_index,1,copy)
-        #     self.set_index(index,index_cols,0,copy)
-        # else:
-        #     self.set_index(index,index_cols,0,copy)
-        #     self.set_index(columns,col_index,1,copy)
         return
     
     # 2021-05-29
     def __getitem__(self, item):
         if self._NeedSplit(item):
             x, xsingle = self.index._GetPrep(item[0])
             y = self.columns[item[1]]
         else:
             x, xsingle = self.index._GetPrep(item)
             y = None
         
         frame = self.frame
         if IsIterable(x) and IsIterable(y):
             data = frame._ValidData[x][:,y]
-            # data = frame._ValidData[TupleProduct(x,y,order=AnsiOrder)].reshape(
-            #     (len(x),len(y)),order=AnsiOrder)
             owndata = True
         else:
             data = frame._ValidData[x] if y is None else frame._ValidData[x,y]
             if not IsArray(data):
                 return data
             owndata = data.flags.owndata
         
         if data.ndim==1:
             if xsingle:
+                if y is None and isinstance(frame.index,FrameAxisIndex):
+                    index = None
+                    index_cols = frame.index._Labels
+                else:
+                    index = frame.index.take(x)
+                    index_cols = None
+                if y is None:
+                    columns, col_index = frame.new_columns(True)
+                    if not columns is None:
+                        columns = columns.copy()
+                else:
+                    columns = frame.columns.take(y)
+                    col_index = None
                 return ArrayFrame(
                     data = data.reshape((1,len(data)),order=AnsiOrder),
-                    index = frame.index.take(x),
-                    columns = frame.columns if y is None 
-                        else frame.columns.take(y),
+                    index = index,
+                    index_cols = index_cols,
+                    columns = columns,
+                    col_index = col_index,
                     dtype = frame.dtype,
                     auto_expand = frame._AutoExpand,
                     expand_count = frame._ExpandCount,
                     expand_ratio = frame._ExpandRatio,
                     _assign_manager = None if owndata else frame._AssignManager
                 )
             else:
@@ -3365,18 +4392,33 @@
                     name = item[1],
                     auto_expand = frame._AutoExpand[0],
                     expand_count = frame._ExpandCount[0],
                     expand_ratio = frame._ExpandRatio[0],
                     _assign_manager = None if owndata else frame._AssignManager
                 )
         else:
+            if y is None and isinstance(frame.index,FrameAxisIndex):
+                index = None
+                index_cols = frame.index._Labels
+            else:
+                index = frame.index.take(x)
+                index_cols = None
+            if y is None:
+                columns, col_index = frame.new_columns(True)
+                if not columns is None:
+                    columns = columns.copy()
+            else:
+                columns = frame.columns.take(y)
+                col_index = None
             return ArrayFrame(
                 data = data,
-                index = frame.index.take(x),
-                columns = frame.columns if y is None else frame.columns.take(y),
+                index = index,
+                index_cols = index_cols,
+                columns = columns,
+                col_index = col_index,
                 dtype = frame.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
                 expand_ratio = frame._ExpandRatio,
                 _assign_manager = None if owndata else frame._AssignManager
             )
     
@@ -3422,23 +4464,30 @@
                 vshape = value.shape[:2]
                 if vshape[0]==0 or vshape[1]==0:
                     return
         
         # 空数据框处理
         if not self._ILoc and frame.shape==(0,0):
             frame._SetData(value)
+            frame.iloc._UpdateValidShape(frame._ValidShape)
+            frame.ix.index = frame.iloc.index
             if not IsSlice(x):
                 self.set_index(x)
                 frame.index = self.index
                 frame._NoLoc = False
+            else:
+                frame.index = frame.iloc.index
             if not y is None and not IsSlice(y):
                 self.set_index(y,axis=1)
                 frame.columns = self.columns
                 frame.ix.columns = self.columns
                 frame._NoLoc = False
+            else:
+                frame.columns = frame.iloc.columns
+                frame.ix.columns = frame.columns
             return
         
         # 下标处理
         x, maxxlen = self.index._SetPrep(x)
         if maxxlen==0:
             return
         if maxxlen is None:
@@ -3535,15 +4584,16 @@
             else:
                 if IsSingleType2(cpos):
                     clen = frame.shape[1] if IsSlice(cpos) else 1
                 else:
                     clen = len(cpos)
                 rtdata = np.ndarray(
                     shape = (plen,clen),
-                    dtype = frame.dtype,
+                    dtype = frame.dtype if type(fill_value)==frame.dtype 
+                        else object,
                     order = AnsiOrder
                 )
                 rtdata[:,:] = fill_value
                 if pplen>0:
                     if columns is None:
                         v = values[pos[ppos]]
                     elif values.flags.c_contiguous:
@@ -3585,20 +4635,21 @@
                     rtdata = values[:,pos]
                 elif values.flags.c_contiguous:
                     rtdata = values[:,pos][rpos]
                 else:
                     rtdata = values[rpos][:,pos]
             else:
                 if IsSingleType2(rpos):
-                    rlen = frame.shape[1] if IsSlice(rpos) else 1
+                    rlen = frame.shape[0] if IsSlice(rpos) else 1
                 else:
                     rlen = len(rpos)
                 rtdata = np.ndarray(
                     shape = (rlen,plen),
-                    dtype = frame.dtype,
+                    dtype = frame.dtype if type(fill_value)==frame.dtype 
+                        else object,
                     order = AnsiOrder
                 )
                 rtdata[:,:] = fill_value
                 if pplen>0:
                     if index is None:
                         v = values[:,pos[ppos]]
                     elif values.flags.c_contiguous:
@@ -3653,38 +4704,26 @@
                 if values.flags.c_contiguous:
                     rtdata = values[:,cpos][rpos]
                 else:
                     rtdata = values[rpos][:,cpos]
             else:
                 rtdata = np.ndarray(
                     shape = (rlen,clen),
-                    dtype = frame.dtype,
+                    dtype = frame.dtype if type(fill_value)==frame.dtype 
+                        else object,
                     order = AnsiOrder
                 )
                 rtdata[:,:] = fill_value
                 if rplen>0 and cplen>0:
                     if rplen<cplen:
                         for r in rppos:
                             rtdata[r,cppos] = values[rpos[r],cppos]
                     else:
                         for c in cppos:
                             rtdata[rppos,c] = values[rppos,cpos[c]]
-                    
-                    # if values.flags.c_contiguous:
-                    #     v = values[:,cpos[cppos]][rpos[rppos]]
-                    # else:
-                    #     v = values[rpos[rppos]][:,cpos[cppos]]
-                    # if IsSingleType2(v):
-                    #     rtdata[rppos,cppos] = v
-                    # elif rplen==1:
-                    #     rtdata[rppos,cppos] = v.reshape((1,cplen))
-                    # elif cplen==1:
-                    #     rtdata[rppos,cppos] = v.reshape((rplen,1))
-                    # else:
-                    #     rtdata[rppos,cppos] = v
             return ArrayFrame(
                 data = rtdata,
                 index = rtindex,
                 columns = rtcols,
                 dtype = frame.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
@@ -3719,22 +4758,14 @@
                 self.index = frame.iloc.index if hasattr(frame,'iloc') \
                     else ArrayIndex(frame._ValidShape[0])
             else:
                 self.columns = frame.iloc.columns if hasattr(frame,'iloc') \
                     else ArrayIndex(frame._ValidShape[1])
             return
         
-        # if index is None and not index_cols is None:
-        #     index = FrameAxisIndex(frame,index_cols,axis,copy)
-        #     if axis==0:
-        #         self.index = index
-        #     else:
-        #         self.columns = index
-        #     return
-        
         if isinstance(index,ArrayIndex):
             if frame._ValidShape[axis]==0:
                 frame._UpdateEmptyAxisLen(axis,len(index))
             elif frame._ValidShape[axis]!=len(index):
                 raise ValueError('Index size mismatch.')
             if copy:
                 index = index.copy()
@@ -3746,15 +4777,15 @@
             index = ArrayValueIndex(index)
         elif IsIndex(index):
             if frame._ValidShape[axis]==0:
                 frame._UpdateEmptyAxisLen(axis,len(index))
             elif frame._ValidShape[axis]!=len(index):
                 raise ValueError('Index size mismatch.')
             if IsMultiIndex(index):
-                index = ArrayMultiIndex(np.array(tuple(index.values)))
+                index = ArrayMultiIndex(list(zip(*index.values)))
             else:
                 index = ArrayValueIndex(
                     values = index.values,
                     copy = copy,
                     _assign_manager = _assign_manager
                 )
         elif IsSingleType(index[0]):
@@ -3764,18 +4795,21 @@
                 raise ValueError('Index size mismatch.')
             index = ArrayValueIndex(
                 values = index,
                 copy = copy,
                 _assign_manager = _assign_manager
             )
         else:
-            vlen = len(index[0])
-            for i in range(1,len(index)):
-                if len(index[i])!=vlen:
-                    raise ValueError('Index size mismatch.')
+            if IsArray(index):
+                vlen = len(index)
+            else:
+                vlen = len(index[0])
+                for i in range(1,len(index)):
+                    if len(index[i])!=vlen:
+                        raise ValueError('Index size mismatch.')
             if frame._ValidShape[axis]==0:
                 frame._UpdateEmptyAxisLen(axis,vlen)
             elif frame._ValidShape[axis]!=vlen:
                 raise ValueError('Index size mismatch.')
             index = ArrayMultiIndex(index)
         
         if axis==0:
@@ -3847,19 +4881,19 @@
                 rtdata = np.concatenate([d._ValidData for d in details])
             dlens = [len(d) for d in details]
             multi_values = max(dlens)>1
         
         if group_keys is None:
             group_keys = self.group_keys
         if group_keys:
-            keys = list(index.keys())
+            keys = index.new_key_index()
             if multi_values:
                 rtindex = []
                 for i in range(len(keys)):
-                    rtindex += [keys[i]]*dlens[i]
+                    rtindex += [keys.get_iloc(i)]*dlens[i]
             else:
                 rtindex = keys
         elif not dsingle and not darray and not d0.index.simple:
             rtindex = np.concatenate([d.index.values for d in details])
         else:
             rtindex = None
         
@@ -3973,25 +5007,26 @@
                 else:
                     rtdata = np.concatenate(values)
                     dlens = [v.shape[0] for v in values]
                     multi_values = max(dlens)>1
                 rtcolumns, rtcol_index = d0.new_columns(False)
             
             if group_keys:
-                keys = list(locIndex.keys())
+                keys = locIndex.new_key_index()
                 if multi_values:
                     rtindex = []
                     for i in range(len(keys)):
-                        rtindex += [keys[i]]*dlens[i]
+                        rtindex += [keys.get_iloc(i)]*dlens[i]
                 else:
                     rtindex = keys
             elif not dsingle and not darray and not d0.index.simple:
                 rtindex = np.concatenate([d.index.values for d in details])
             else:
                 rtindex = None
+            rtindex_cols = None
         else:
             if not columns is None:
                 data = data[locIndex[columns]]
             
             if locColumns.multi_values:
                 details = [func(data[:,p],*args,**kwargs) 
                     for p in locColumns.pos()]
@@ -4024,25 +5059,26 @@
                 else:
                     rtdata = np.concatenate(values,1)
                     dlens = [v.shape[1] for v in values]
                     multi_values = max(dlens)>1
                 rtindex, rtindex_cols = d0.new_index(False)
             
             if group_keys:
-                keys = list(locColumns.keys())
+                keys = locColumns.new_key_index()
                 if multi_values:
                     rtcolumns = []
                     for i in range(len(keys)):
-                        rtcolumns += [keys[i]]*dlens[i]
+                        rtcolumns += [keys.get_iloc(i)]*dlens[i]
                 else:
                     rtcolumns = keys
             elif not dsingle and not darray and not d0.index.simple:
                 rtcolumns = np.concatenate([d.columns.values for d in details])
             else:
                 rtcolumns = None
+            rtcol_index = None
         
         if rtdata.ndim==1:
             return ArraySeries(
                 data = rtdata,
                 index = rtindex if axis==0 else rtcolumns,
                 dtype = rtdata.dtype,
                 auto_expand = frame._AutoExpand[axis],
@@ -4051,14 +5087,15 @@
             )
         else:
             return ArrayFrame(
                 data = rtdata,
                 index = rtindex,
                 index_cols = rtindex_cols,
                 columns = rtcolumns,
+                col_index = rtcol_index,
                 dtype = rtdata.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
                 expand_ratio = frame._ExpandRatio,
             )
     
     # 2022-04-05
@@ -4092,15 +5129,15 @@
                 cplen = len(cpos)
                 for p in locIndex.pos():
                     rtdata.append(np.repeat(len(p),cplen))
             rtdata = np.array(rtdata)
             
             return ArrayFrame(
                 data = rtdata,
-                index = list(locIndex.keys()) if self.group_keys else None,
+                index = locIndex.new_key_index() if self.group_keys else None,
                 columns = rtcolumns,
                 col_index = rtcol_index,
                 dtype = rtdata.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
                 expand_ratio = frame._ExpandRatio,
             )
@@ -4125,15 +5162,16 @@
                 for p in locColumns.pos():
                     rtdata.append(np.repeat(len(p),iplen))
             rtdata = np.array(rtdata).T
             
             return ArrayFrame(
                 data = rtdata,
                 index = rtindex,
-                columns = list(locColumns.keys()) if self.group_keys else None,
+                columns = locColumns.new_key_index() if self.group_keys 
+                    else None,
                 index_cols = rtindex_cols,
                 dtype = rtdata.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
                 expand_ratio = frame._ExpandRatio,
             )
     
@@ -4155,15 +5193,15 @@
                 cpos = locColumns[columns]
                 data = data[:,cpos]
                 rtcolumns = locColumns.take(cpos)
                 rtcol_index = None
             rtdata = data[[p[0] for p in locIndex.pos()]]
             return ArrayFrame(
                 data = rtdata,
-                index = list(locIndex.keys()) if self.group_keys else None,
+                index = locIndex.new_key_index() if self.group_keys else None,
                 columns = rtcolumns,
                 col_index = rtcol_index,
                 dtype = rtdata.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
                 expand_ratio = frame._ExpandRatio,
             )
@@ -4177,15 +5215,16 @@
                 rtindex = locIndex.take(ipos)
                 rtindex_cols = None
             rtdata = data[:,[p[0] for p in locColumns.pos()]]
             return ArrayFrame(
                 data = rtdata,
                 index = rtindex,
                 index_cols = rtindex_cols,
-                columns = list(locColumns.keys()) if self.group_keys else None,
+                columns = locColumns.new_key_index() if self.group_keys
+                    else None,
                 dtype = rtdata.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
                 expand_ratio = frame._ExpandRatio,
             )
 
     # 2022-04-05
@@ -4206,15 +5245,15 @@
                 cpos = locColumns[columns]
                 data = data[:,cpos]
                 rtcolumns = locColumns.take(cpos)
                 rtcol_index = None
             rtdata = data[[p[-1] for p in locIndex.pos()]]
             return ArrayFrame(
                 data = rtdata,
-                index = list(locIndex.keys()) if self.group_keys else None,
+                index = locIndex.new_key_index() if self.group_keys else None,
                 columns = rtcolumns,
                 col_index = rtcol_index,
                 dtype = rtdata.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
                 expand_ratio = frame._ExpandRatio,
             )
@@ -4228,15 +5267,16 @@
                 rtindex = locIndex.take(ipos)
                 rtindex_cols = None
             rtdata = data[:,[p[-1] for p in locColumns.pos()]]
             return ArrayFrame(
                 data = rtdata,
                 index = rtindex,
                 index_cols = rtindex_cols,
-                columns = list(locColumns.keys()) if self.group_keys else None,
+                columns = locColumns.new_key_index() if self.group_keys 
+                    else None,
                 dtype = rtdata.dtype,
                 auto_expand = frame._AutoExpand,
                 expand_count = frame._ExpandCount,
                 expand_ratio = frame._ExpandRatio,
             )
 
 # 6. 后序函数
@@ -4245,15 +5285,22 @@
 
 # 2022-03-08
 def concat(objs, axis = 0, concat_index = False):
     '''
     数据表拼接。
     【注】本函数默认要求objs所有成员及其索引（如有）的类型均相同。
     '''
+    objs = [o for o in objs if not o is None and np.product(o.shape)>0]
+    olen = len(objs)
+    if olen==0:
+        return None
+    
     obj0 = objs[0]
+    if olen==1:
+        return obj0.copy()
     if IsArray(obj0):
         rtdata = np.concatenate(objs,axis)
         if rtdata.ndim==1:
             return ArraySeries(rtdata,dtype=rtdata.dtype)
         else:
             return ArrayFrame(rtdata,dtype=rtdata.dtype)
     else:
```

### Comparing `arraytool-0.1.4/arraytool/decorator.py` & `arraytool-0.1.5/arraytool/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Created on Fri Feb 25 20:47:35 2022
 
 @author: chenyc
 """
 
 # arraytool包专用装饰器，春秋迭代，yondersky@126.com，2022-02-25
-# 更新日期：2022-04-16
+# 更新日期：2022-11-20
 
 # 【注】通用装饰器位于pytool.py文件中。
 
 import bisect
 import numpy as np
 from pandas import Series, DataFrame
 
@@ -50,14 +50,25 @@
     def operfunc(self):
         datafunc = getattr(getattr(self,attr),operator)
         return self.new_data(datafunc(),dtype)
     
     return operfunc
 
 # 2022-02-25
+def UnaryFuncBool(operator, attr = '_ValidData'):
+    '''数据序列一元运算符'''
+    
+    # 2022-02-25
+    def operfunc(self):
+        datafunc = getattr(getattr(self,attr).astype(bool),operator)
+        return self.new_data(datafunc(),bool)
+    
+    return operfunc
+
+# 2022-02-25
 def BinaryFunc(operator, attr = '_ValidData', dtype = None):
     '''数据序列二元运算符'''
     
     # 2022-02-25
     def operfunc(self, other):
         try:
             datafunc = getattr(getattr(self,attr),operator)
@@ -79,15 +90,15 @@
     '''
     运算符转移装饰器。
     【注】运算符转移装饰器将ArraySeries或ArrayFrame的运算符操作转移至_ValidData成员。
     '''
     for op in UnaryOperators:
         setattr(cls,op,UnaryFunc(op,attr))
     for op in UnaryBoolOperators:
-        setattr(cls,op,UnaryFunc(op,attr,bool))
+        setattr(cls,op,UnaryFuncBool(op,attr))
     for op in BinaryOperators:
         setattr(cls,op,BinaryFunc(op,attr))
     for op in BinaryBoolOperators:
         setattr(cls,op,BinaryFunc(op,attr,bool))
     return cls
 
 # 2. 统计函数装饰器
@@ -151,14 +162,43 @@
         else:
             return getattr(np,operator)(data,**kwargs)
     
     return operfunc
 
 # 2.2.3 数据系列分组
 
+# 2022-11-13
+def CumNAStatFuncSeriesGroupBy(operator):
+    '''数据系统分组累计统计函数（含NA相关参数）'''
+    
+    # 2022-11-13
+    def operfunc(self, skipna = True, **kwargs):
+        '''累计统计函数，参见numpy同名函数'''
+        series = self.series
+        data = series._ValidData
+        if skipna:
+            data = data.astype(float) if data.dtype==object else data.copy()
+            statfunc = getattr(np,'nan'+operator)
+        else:
+            data = data.copy()
+            statfunc = getattr(np,operator)
+        for p in self.index.pos():
+            data[p] = statfunc(data[p])
+        return series.__class__(
+            data = data,
+            index = series.new_index() if self.group_keys else None,
+            dtype = data.dtype,
+            name = operator,
+            auto_expand = series._AutoExpand,
+            expand_count = series._ExpandCount,
+            expand_ratio = series._ExpandRatio,
+        )
+    
+    return operfunc
+
 # 2022-03-19
 def NAStatFuncSeriesGroupBy(operator):
     '''数据系列分组统计函数（含NA相关参数）'''
     
     # 2022-03-19
     def operfunc(self, skipna = True, **kwargs):
         '''统计函数，参见numpy同名函数'''
@@ -169,15 +209,15 @@
             if data.dtype==object:
                 data = data.astype(float)
             statfunc = getattr(np,'nan'+operator)
         else:
             statfunc = getattr(np,operator)
         return series.__class__(
             data = [statfunc(data[index[k]]) for k in index.keys()],
-            index = list(index.keys()) if self.group_keys else None,
+            index = index.new_key_index() if self.group_keys else None,
             dtype = data.dtype,
             name = operator,
             auto_expand = series._AutoExpand,
             expand_count = series._ExpandCount,
             expand_ratio = series._ExpandRatio,
         )
     
@@ -266,14 +306,81 @@
         else:
             return self.new_aggr_data(rt,axis,operator,columns=columns)
     
     return operfunc
 
 # 2.2.5 数据表分组
 
+# 2022-11-20
+def CumNAStatFuncFrameGroupBy(operator):
+    '''数据表分组累计统计函数'''
+    
+    # 2022-11-20
+    def operfunc(self, columns = None, skipna = True, **kwargs):
+        '''累计统计函数，参见numpy同名函数'''
+        axis = self.axis
+        group_keys = self.group_keys
+        frame = self.frame
+        data = frame._ValidData
+        locIndex = self.index
+        locColumns = self.columns
+        
+        if skipna:
+            data = data.astype(float) if data.dtype==object else data.copy()
+            statfunc = getattr(np,'nan'+operator)
+        else:
+            data = data.copy()
+            statfunc = getattr(np,operator)
+        
+        if columns is None:
+            if axis==0:
+                rtcolumns, rtcol_index = frame.new_columns(False,locColumns)
+            else:
+                rtindex, rtindex_cols = frame.new_index(False,locIndex)
+        else:
+            if IsSingleType(columns):
+                columns = [columns]
+            if axis==0:
+                cpos = locColumns[columns]
+                data = data[:,cpos]
+                rtcolumns = locColumns.take(cpos)
+                rtcol_index = None
+            else:
+                ipos = locIndex[columns]
+                data = data[ipos]
+                rtindex = locIndex.take(ipos)
+                rtindex_cols = None
+        
+        if axis==0:
+            for p in locIndex.pos():
+                data[p] = statfunc(data[p],axis=0)
+            rtindex = locIndex.copy() if group_keys else None
+            rtindex_cols = None
+        else:
+            for p in locColumns.pos():
+                data[:,p] = statfunc(data[:,p],axis=1)
+            if group_keys:
+                rtcolumns, rtcol_index = frame.new
+            rtcolumns = locColumns.copy() if group_keys else None
+            rtcol_index = None
+        
+        return frame.__class__(
+            data = data,
+            index = rtindex,
+            columns = rtcolumns,
+            index_cols = rtindex_cols,
+            col_index = rtcol_index,
+            dtype = data.dtype,
+            auto_expand = frame._AutoExpand,
+            expand_count = frame._ExpandCount,
+            expand_ratio = frame._ExpandRatio,
+        )
+    
+    return operfunc
+
 # 2022-04-03
 def NAStatFuncFrameGroupBy(operator):
     '''数据表分组统计函数'''
     
     # 2022-04-03
     def operfunc(self, columns = None, skipna = True, **kwargs):
         '''统计函数，参见numpy同名函数'''
@@ -311,24 +418,24 @@
         
         if axis==0:
             if locIndex.multi_values:
                 rtdata = np.array([statfunc(data[p],0) for p in locIndex.pos()])
             else:
                 rtdata = np.array(
                     [statfunc(data[[p]],0) for p in locIndex.pos()])
-            rtindex = list(locIndex.keys()) if self.group_keys else None
+            rtindex = locIndex.new_key_index() if self.group_keys else None
             rtindex_cols = None
         else:
             if locColumns.multi_values:
                 rtdata = np.array(
                     [statfunc(data[:,p],1) for p in locColumns.pos()]).T
             else:
                 rtdata = np.array(
                     [statfunc(data[:,[p]],1) for p in locColumns.pos()]).T
-            rtcolumns = list(locColumns.keys()) if self.group_keys else None
+            rtcolumns = locColumns.new_key_index() if self.group_keys else None
             rtcol_index = None
         return frame.__class__(
             data = rtdata,
             index = rtindex,
             columns = rtcolumns,
             index_cols = rtindex_cols,
             col_index = rtcol_index,
@@ -428,14 +535,16 @@
 # 4.1.2 数据系列分组
 
 # 2022-03-20
 def DecorateSeriesGroupBy(cls):
     '''数据系列分组类装饰器'''
     for op in NAStatOperators:
         setattr(cls,op,NAStatFuncSeriesGroupBy(op))
+    for op in CumNAStatOperators:
+        setattr(cls,op,CumNAStatFuncSeriesGroupBy(op))
     for op in AggrOperators:
         setattr(cls,op,AggrFuncSeriesGroupBy(op))
     return cls
 
 # 4.2 数据表
 
 # 4.2.1 数据表
@@ -455,8 +564,10 @@
 # 4.2.2 数据表分组
 
 # 2022-04-03
 def DecorateFrameGroupBy(cls):
     '''数据表分组类装饰器'''
     for op in NAStatOperators:
         setattr(cls,op,NAStatFuncFrameGroupBy(op))
+    for op in CumNAStatOperators:
+        setattr(cls,op,CumNAStatFuncFrameGroupBy(op))
     return cls
```

### Comparing `arraytool-0.1.4/arraytool/pytool.py` & `arraytool-0.1.5/arraytool/pytool.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 """
 Created on Fri Nov 20 20:22:44 2020
 
 @author: yonder_sky
 """
 
 # Python通用工具库，春秋迭代，yondersky@126.com，2020-11-20
-# 更新日期：2022-04-14
+# 更新日期：2023-03-28
 
 import collections, functools, itertools, math, numbers, time
 import datetime as dt
 import numpy as np
 import pandas as pd
+from calendar import monthrange
 from pandas import DataFrame, Series
 from scipy.stats import rankdata
 
 # 0. 全局变量
 
 ConsoleInitStamp = time.strftime('%Y%m%d%H%M%S')
 # LogDir = os.getcwd()+'\\Log'
@@ -269,19 +270,21 @@
             if rttype is range or rttype is set:
                 rttype = list
             if rttype is list:
                 return result
             elif rttype is np.ndarray:
                 return np.array(result)
             elif hasattr(rttype,'values') and hasattr(iterables[0],'values'):
-                return rttype(result,iterable[0].index)
+                return rttype(result,iterables[0].index)
             else:
                 return rttype(result)
         else:
             return func(self,*iterables,**kwargs)
+    
+    return applied
 
 # 3. 格式转换
 
 # 3.1 字符串相关
 
 # 3.1.1 子字符串
 
@@ -384,93 +387,159 @@
     '''
     rq = rquotes[quote] if quote in rquotes else quote
     return quote+refStr+rq
 
 # 3.1.4 整数转字符串
 
 # 2022-01-11
-@sapply
+@emap
 def DateIntToStr(dateInt):
     '''
     数字日期转字符串。
     【示例】
     >>> DateIntToStr([20090101,20121031,0])
     ['2009-01-01', '2012-10-31', '0-00-00']
     '''
     s = '{:05d}'.format(dateInt)
     return s[:-4]+'-'+s[-4:-2]+'-'+s[-2:]
 
-# 3.1.5 当前时间
+# 3.1.5 字符串转日期
+
+# 2022-07-05
+@emap
+def DateStrToDate(dstr):
+    '''
+    日期字符转日期。
+    【示例】
+    >>> DateStrToDate(['2022-06-05','2022/7/1'])
+    [datetime.datetime(2022, 6, 5, 0, 0), datetime.datetime(2022, 7, 1, 0, 0)]
+    '''
+    return pd.Timestamp(dstr).to_pydatetime()
+
+# 2022-07-06
+@emap
+def DateStrToInt(dstr):
+    '''
+    日期字符串转数字日期。
+    【示例】
+    >>> DateStrToInt(['2022-06-05','2022/7/1'])
+    [20220605, 20220701]
+    '''
+    return DateToInt(pd.Timestamp(dstr))
+
+# 2022-07-05
+@emap
+def DateStrToTimestamp(dstr):
+    '''
+    日期字符转时间戳。
+    【示例】
+    >>> DateStrToTimestamp(['2022-06-05','2022/7/1'])
+    [Timestamp('2022-06-05 00:00:00'), Timestamp('2022-07-01 00:00:00')]
+    '''
+    return pd.Timestamp(dstr)
+
+# 3.1.6 当前时间
 
 # 2022-01-24
 def CurrentTimeStr():
     '''当前时间戳'''
     return time.strftime('%Y-%m-%d %H:%M:%S')
 
-# 3.1.6 可迭代对象转字符串
+# 3.1.7 可迭代对象转字符串
 
 # 2022-04-14
-def ListToStr(iterables, sep = ',', unique = False, NAIgnored = False):
+def ListToStr(iterables, sep = ',', unique = False, NAIgnored = False,
+    NAStr = 'NA'):
     '''
     可迭代对象转字符串。
-
-    示例：
+    【示例】
     >>> ListToStr([1,2,3],';')
     '1;2;3'
     >>> ListToStr(Series([1,3,2,3,2,1]),unique=True)
     '1,3,2'
     >>> ListToStr('abc')
     'abc'
     >>> ListToStr(['a','b',NA,'c'])
     'a,b,NA,c'
     >>> ListToStr(['a','b',NA,'c'],NAIgnored=True)
     'a,b,c'
-    >>> ListToStr({'a':'aa','b':'bb'})
-    'aa,bb'
     '''
-    values = Series(iterables)
-    if unique:
-        values = values.drop_duplicates()
+    if isinstance(iterables,str):
+        iterables = [iterables]
+    elif unique:
+        iterables = collections.OrderedDict.fromkeys(iterables)
+    strs = [format(i) for i in iterables]
     if NAIgnored:
-        values = values.dropna()
+        strs = [s for s in strs if s!='nan']
     else:
-        values = values.replace(np.nan,'NA')
-    return sep.join(values.astype(str))
+        strs = [NAStr if s=='nan' else s for s in strs]
+    return sep.join(strs)
 
 # 3.2 数字相关
 
 # 3.2.1 舍入
 
 # 2021-10-17
 @emap
 def ExactInt(x):
     '''
     舍入取整。
 
     示例：
-    >>> ExactInt([0, 1, 0.5])
-    [0, 1, 1]
+    >>> ExactInt([0, 1, 0.5, -5.05])
+    [0, 1, 1, -5]
     '''
-    return int(x+0.5)
+    return int(x+0.5) if x>=0 else -int(-x+0.5)
 
 # 2021-09-14
 @sapply
 def ExactRound(number, ndigits = 0):
     '''
     自定义舍入函数。
     【示例】
-    >>> ExactRound([0, 0.05, 0.0499], 1)
-    [0.0, 0.1, 0.0]
+    >>> ExactRound([0, 0.05, 0.0499, -5.005], 1)
+    [0.0, 0.1, 0.0, -5.0]
     >>> ExactRound(12345.6789,3)
     12345.679
     >>> ExactRound(12345.6789,-3)
     12000.0
     '''
     base = 10**ndigits
-    return int(number*base+0.5)/base
+    return int(number*base+0.5)/base if number>=0 \
+        else -int(0.5-number*base)/base
+
+# 2022-04-21
+@sapply
+def eceiling(x, n = 0):
+    '''
+    扩展math.ceiling函数。
+
+    示例：
+    >>> eceiling([0, 1, 0.5])
+    [0.0, 1.0, 1.0]
+    >>> eceiling(111,-2)
+    200.0
+    '''
+    base = 10**n
+    return math.ceil(x*base)/base
+
+# 2022-04-21
+@sapply
+def efloor(x, n = 0):
+    '''
+    扩展math.floor函数。
+
+    示例：
+    >>> efloor([0, 1, 0.5])
+    [0.0, 1.0, 0.0]
+    >>> efloor(111,-2)
+    100.0
+    '''
+    base = 10**n
+    return math.floor(x*base)/base
 
 # 3.3 切片相关
 
 # 格式化切片
 # 2020-11-28
 def FormatSlice(s, maxlen):
     '''
@@ -494,31 +563,40 @@
         stop %= maxlen
     return slice(start,stop,step)
 
 # 3.4 列表相关
 
 # 多维笛卡尔积
 # 2021-06-03
-def ListProduct(*iterables, order = 'C'):
+def ListProduct(*iterables, order = 'C', rtOrder = 'F'):
     '''
     多维笛卡尔积。
     【注】
     关于order参数：
       C - 以行主序进行遍历（C风格）
       F - 以列主序进行遍历（F风格）
     【示例】
     >>> ListProduct(list('abc'),[1,0])
     [['a', 'a', 'b', 'b', 'c', 'c'], [1, 0, 1, 0, 1, 0]]
+    >>> ListProduct(list('abc'),[1,0],rtOrder='C')
+    [('a', 1), ('a', 0), ('b', 1), ('b', 0), ('c', 1), ('c', 0)]
     >>> ListProduct(list('abc'),[1,0],order='F')
     [['a', 'b', 'c', 'a', 'b', 'c'], [1, 1, 1, 0, 0, 0]]
+    >>> ListProduct(list('abc'),[1,0],order='F',rtOrder='C')
+    [('a', 1), ('b', 1), ('c', 1), ('a', 0), ('b', 0), ('c', 0)]
     '''
     if order=='F':
-        return [list(z) for z in zip(*itertools.product(*iterables[::-1]))][::-1]
+        rt = itertools.product(*iterables[::-1])
+        if rtOrder=='F':
+            return [list(z) for z in zip(*rt)][::-1]
+        else:
+            return [z[::-1] for z in rt]
     else:
-        return [list(z) for z in zip(*itertools.product(*iterables))]
+        rt = itertools.product(*iterables)
+        return [list(z) for z in zip(*rt)] if rtOrder=='F' else list(rt)
 
 # 3.5 元组相关
 
 # 多维笛卡尔积
 # 2021-06-03
 def TupleProduct(*iterables, order = 'C'):
     '''
@@ -635,14 +713,16 @@
     [20211231, 20201130]
     >>> edate([dt.date(2022,1,31),dt.date(2022,2,28)])
     [datetime.date(2022, 2, 28), datetime.date(2022, 3, 28)]
     >>> edate([dt.date(2022,3,31),dt.date(2021,12,30)])
     [datetime.date(2022, 4, 30), datetime.date(2022, 1, 30)]
     >>> edate(pd.Timestamp('2022-01-01 19:31:31'))
     Timestamp('2022-02-01 19:31:31')
+    >>> edate(20141204,36)
+    20171204
     '''
     if IsNA(date):
         return NA
     elif isinstance(date,numbers.Real):
         return edateIntSingle(int(date),count)
     else:
         return edateDateSingle(date,count)
@@ -675,24 +755,52 @@
     返回指定日前推/后推一定月份的日期。
     '''
     year = dateInt//10000
     month = dateInt%10000//100
     day = dateInt%100
     
     month += count
-    if month>12:
-        year += month//12
-        month %= 12
-    elif month<1:
+    if month<1 or month>12:
         year += (month-1)//12
         month = (month-1)%12+1
     day = min(day,monthdaysSingle(year,month))
     return year*10000+month*100+day
 
-# 3.6.3.4 区间起止日
+# 3.6.3.4 报告期偏移
+
+ReportDateEnd = [331,630,930,1231]
+
+# 报告期偏移
+# 2022-09-07
+@sapply
+def eReportPeriod(date, count = 1):
+    '''
+    返回指定日期前推/后推一定季度的季末。
+    【示例】
+    >>> eReportPeriod([20211231,20220501,20210630])
+    [20220331, 20220930, 20210930]
+    >>> eReportPeriod([dt.date(2022,12,31),dt.date(2022,5,30)],-1)
+    [datetime.date(2022, 9, 30), datetime.date(2022, 3, 31)]
+    '''
+    if IsNASingle(date):
+        return NA
+    if isinstance(date,numbers.Real):
+        date = int(date)
+        doff = edateIntSingle(date,count*3)
+        year = doff//10000
+        month = doff%10000//100
+        return year*10000+ReportDateEnd[(month-1)//3]
+    else:
+        doff = edateDateSingle(date,count*3)
+        year = doff.year
+        month = doff.month
+        month += (12-month)%3
+        return dt.date(year,month,31 if month==3 or month==12 else 30)
+
+# 3.6.3.5 区间起止日
 
 # 年起始日
 # 2022-01-17
 @emap
 def StartOfTheYear(date):
     '''
     返回指定日所在年起始日。
@@ -850,30 +958,112 @@
         dateInt = True
         date = IntToDate(int(date))
     else:
         dateInt = False
     end = date+dt.timedelta((-date.weekday()+weekStart-2)%7)
     return DateToInt(end) if dateInt else end
 
-# 3.6.3.5 日期间隔
+# 3.6.3.6 间隔统计
+
+# 数字日所在月天数
+# 2023-03-28
+@emap
+def DatesOfTheMonth(date):
+    '''
+    返回对应日所在月天数。
+
+    【示例】
+    >>> DatesOfTheMonth([20200221,20210221])
+    [29, 28]
+    >>> DatesOfTheMonth([dt.date(2020,2,21),dt.date(2021,2,21)])
+    [29, 28]
+    '''
+    if IsNASingle(date):
+        return NA
+    if isinstance(date,numbers.Real):
+        if not isinstance(date,numbers.Integral):
+            date = int(date)
+        return monthrange(date//10000,date%10000//100)[1]
+    else:
+        return monthrange(date.year,date.month)[1]
+
+# 数字日所在年天数
+# 2023-03-28
+@emap
+def DatesOfTheYear(date):
+    '''
+    返回对应日所在年天数。
 
+    【示例】
+    >>> DatesOfTheYear([20200701,20210701])
+    [366, 365]
+    >>> DatesOfTheYear([dt.date(2020,7,1),dt.date(2021,7,1)])
+    [366, 365]
+    '''
+    if IsNASingle(date):
+        return NA
+    if isinstance(date,numbers.Real):
+        if not isinstance(date,numbers.Integral):
+            date = int(date)
+        return 366 if IsLeapYear(date//10000) else 365
+    else:
+        return 366 if IsLeapYear(date.year) else 365
+
+# 日期间隔
 # 2022-04-02
 def DateDiff(startDate, endDate):
     '''
     日期间隔。
     【示例】
     >>> DateDiff(20220101,20220331)
     89
     '''
     if IsInteger(startDate):
         startDate = IntToDate(startDate)
     if IsInteger(endDate):
         endDate = IntToDate(endDate)
     return (endDate-startDate).days
 
+# 时间间隔
+# 2023-03-28
+@fapply
+def TimeDiff(start, end, kind = 'Day'):
+    '''
+    返回起始与结束日期之间的时间间隔。
+    【注】kind支持类型：Day、Month、Year。
+    【示例】
+    >>> TimeDiff(20190701,20200701)
+    366
+    >>> TimeDiff(20190701,20200701,'Month')
+    12.0
+    >>> TimeDiff(20190701,20200701,'Year')
+    1.0
+    '''
+    if IsNASingle(start) or IsNASingle(end):
+        return NA
+    if isinstance(start,numbers.Real):
+        start = IntToDate(start)
+    if isinstance(end,numbers.Real):
+        end = IntToDate(end)
+    if kind=='Day':
+        return (end-start).days
+    elif kind=='Month':
+        return (end.year-start.year)*12+end.month-start.month \
+            +(end.day-start.day)/DatesOfTheMonth(end)
+    elif kind=='Year':
+        sm = start.month
+        sd = start.day
+        ey = end.year
+        if not IsLeapYear(ey) and sm==2 and sd==29:
+            sd = 28
+        newstart = dt.date(ey,sm,sd)
+        return end.year-start.year+(end-newstart).days/DatesOfTheYear(end)
+    else:
+        return NA
+
 # 4. 类型判断
 
 # 4.1 变量类型判断
 
 # 2021-02-16
 def IsArray(var):
     '''
@@ -1511,16 +1701,145 @@
         endValue = endValue._ValidData
     elif hasattr(endValue,'values'):
         endValue = endValue.values
     elif not IsArray(endValue):
         endValue = np.array(endValue,np.float64)
     return (endValue-startValue)/np.abs(startValue)
 
+# 5.5 最大回撤
+
+# 2022-04-19
+def MaxRetreat(values, rtnfields = 'MaxRetreat'):
+    '''
+    最大回撤函数。
+    【注】rtnfields参数允许的返回字段包括：
+      All - 返回全部结果
+      MaxRetreat - 最大回撤值
+      RetreatStart - 最大回撤起始索引
+      RetreatEnd - 最大回撤结束索引
+      Recovered - 是否创新高
+      RecoverCount - 最长未创新高期数
+      RecoverStart - 最长未创新高起始索引
+      RecoverEnd - 最长未创新高结束索引
+    '''
+    if hasattr(values,'_ValidData'):
+        values = values._ValidData
+    elif hasattr(values,'values'):
+        values = values.values
+    elif not isinstance(values,np.ndarray):
+        values = np.array(values)
+    if isinstance(rtnfields,str):
+        rtnfields = [rtnfields] if rtnfields!='All' else \
+            ['MaxRetreat','RetreatStart','Recovered','RecoverStart','RecoverEnd']
+    rt = {}
+    
+    retreats = values/np.maximum.accumulate(values)-1
+    retreatEnd = retreats.argmin()
+    rt['RetreatEnd'] = retreatEnd
+    rt['MaxRetreat'] = -retreats[retreatEnd]
+    
+    if 'RetreatStart' in rtnfields or 'RetreatCount' in rtnfields:
+        retreatCount = retreats[retreatEnd::-1].argmax()
+        rt['RetreatCount'] = retreatCount
+        if 'RetreatStart' in rtnfields:
+            rt['RetreatStart'] = retreatEnd-retreatCount
+    
+    if 'Recovered' in rtnfields or 'RecoverCount' in rtnfields \
+        or 'RecoverStart' in rtnfields or 'RecoverEnd' in rtnfields:
+        countfunc = np.frompyfunc(lambda x, y: 0 if y==0 else int(x)+1,2,1)
+        retreatCounts = countfunc.accumulate(retreats,dtype=object)
+        rpos = retreatCounts.argmax()
+        recoverCount = int(retreatCounts[0]) if rpos==0 else retreatCounts[rpos]
+        if 'Recovered' in rtnfields:
+            rt['Recovered'] = not rpos==len(retreats)-1
+        if 'RecoverCount' in rtnfields or 'RecoverStart' in rtnfields:
+            rt['RecoverCount'] = recoverCount
+        if 'RecoverStart' in rtnfields:
+            rt['RecoverStart'] = rpos-recoverCount
+        if 'RecoverEnd' in rtnfields:
+            rt['RecoverEnd'] = rpos
+    return rt
+
+# 5.6 去重
+
+# 2022-06-05
+def unique(values, order = 'keep', rt_kind = 'list'):
+    '''
+    取去重值。
+    【注】
+    1. order参数取值：
+       keep - 保持原有顺序
+       sort - 排序
+    2. rt_kind参数取值：
+       array - np.ndarray
+       list - list
+    【示例】
+    >>> unique([2,1,1,2,3,2])
+    [2, 1, 3]
+    >>> unique([2,1,1,2,3,2],'sort')
+    [1, 2, 3]
+    '''
+    rt = list(collections.OrderedDict.fromkeys(values))
+    if order=='sort':
+        rt = sorted(rt)
+    return np.array(rt) if rt_kind=='array' else rt
+
 # 6. 逻辑扩展
 
+# 2022-09-07
+def ifelse(condition, x, y):
+    '''
+    类R语言ifelse函数。
+    【示例】
+    >>> c1 = [True,True,True,False,False]
+    >>> l1 = [1,2,3,4,5]
+    >>> l2 = list('abcde')
+    >>> a1 = np.array(l1)
+    >>> a2 = np.array(l2)
+    >>> ifelse(c1,1,-1)
+    array([ 1,  1,  1, -1, -1])
+    >>> ifelse(c1,a1,-1)
+    array([1, 2, 3, -1, -1], dtype=object)
+    >>> ifelse(c1,-1,a2)
+    array([-1, -1, -1, 'd', 'e'], dtype=object)
+    >>> ifelse(c1,l1,l2)
+    array([1, 2, 3, 'd', 'e'], dtype=object)
+    >>> ifelse(c1,a2,a1)
+    array(['a', 'b', 'c', 4, 5], dtype=object)
+    '''
+    clen = len(condition)
+    if IsSingleType(x):
+        xsingle = True
+        xtype = type(x)
+    else:
+        xsingle = False
+        if isinstance(x,list):
+            x = np.array(x,dtype=object)
+            xtype = object
+        else:
+            xtype = type(x[0])
+    if IsSingleType(y):
+        ysingle = True
+        ytype = type(y)
+    else:
+        ysingle = False
+        if isinstance(y,list):
+            y = np.array(y,dtype=object)
+            ytype = object
+        else:
+            ytype = type(y[0])
+    xpos = which(condition)
+    ypos = posdiff(clen,xpos)
+    rt = np.ndarray(clen,dtype=xtype if xtype==ytype else object)
+    if len(xpos)>0:
+        rt[xpos] = x if xsingle else x[xpos]
+    if len(ypos)>0:
+        rt[ypos] = y if ysingle else y[ypos]
+    return rt
+
 # 2021-12-02
 def which(expression):
     '''
     下标筛选函数（同R语言which）。
     【示例】
     >>> which(np.arange(5)==4)
     array([4], dtype=int64)
```

### Comparing `arraytool-0.1.4/setup.py` & `arraytool-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open('README.md','r',encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name = 'arraytool',
-    version = '0.1.4',
+    version = '0.1.5',
     author = '春秋迭代',
     author_email = 'yondersky@126.com',
     description = '基于numpy的Series及DataFrame数据结构',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://gitee.com/yonder_sky/arraytool',
     packages = setuptools.find_packages(),
```

