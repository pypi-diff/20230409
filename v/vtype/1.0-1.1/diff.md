# Comparing `tmp/vtype-1.0.tar.gz` & `tmp/vtype-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtype-1.0.tar", last modified: Sun Mar 26 13:05:26 2023, max compression
+gzip compressed data, was "vtype-1.1.tar", last modified: Sun Apr  9 16:19:59 2023, max compression
```

## Comparing `vtype-1.0.tar` & `vtype-1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.559068 vtype-1.0/LICENSE
--rw-r--r--   0        0        0      119 2023-03-26 12:11:14.648893 vtype-1.0/README.md
--rw-r--r--   0        0        0      415 2023-03-26 12:55:40.463664 vtype-1.0/pyproject.toml
--rw-r--r--   0        0        0      142 2023-02-27 15:10:59.033303 vtype-1.0/vtype/__init__.py
--rw-r--r--   0        0        0    11959 2023-03-09 14:53:10.638668 vtype-1.0/vtype/_vtype.py
--rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 vtype-1.0/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.559068 vtype-1.1/LICENSE
+-rw-r--r--   0        0        0      119 2023-03-26 12:11:14.648893 vtype-1.1/README.md
+-rw-r--r--   0        0        0      442 2023-04-09 16:17:17.930894 vtype-1.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 vtype-1.1/vtype/__init__.py
+-rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 vtype-1.1/vtype/_cooltime.py
+-rw-r--r--   0        0        0    11905 2023-04-09 16:11:55.211629 vtype-1.1/vtype/_vtype.py
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 vtype-1.1/PKG-INFO
```

### Comparing `vtype-1.0/LICENSE` & `vtype-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vtype-1.0/vtype/_vtype.py` & `vtype-1.1/vtype/_vtype.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,14 +236,23 @@
         '''
         if not isinstance(keys, tuple):
             keys = (keys, )
         value = _XpathGet(self.core, 0, len(keys), keys)
         if value is SysEmpty:
             raise KeyError(keys)
         return value
+    
+    def deepGet(self, *keys, default=None):
+        res = self.core
+        try:
+            for k in keys:
+                res = res[k]
+            return res
+        except:
+            return default
 
 ########################################## vstr ##########################################
 
 class vstr(ztype):
 
     s_a = 'abcdefghijklmnopqrstuvwxyz'
     s_A = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
@@ -255,54 +264,47 @@
 
     def __new__(cls, obj=SysEmpty, **kvs):
         self = object.__new__(cls)
         self.selfType = cls
         self.core = str(obj)
         return self
 
-    def washParagraph(self):  # 单段清洗
+    def wash_paragraph(self):  # 单段清洗
         text = re.sub('\s+', ' ', self.core)
         text = re.sub('^ +', '', text)
         text = re.sub(' +$', '', text)
         return vstr(text)
 
     def sub(self, pattern, repl, count=0, flags=0):
         return vstr(re.sub(pattern, repl, self.core, count, flags))
 
     def visible(self):  # 是否含可视字符
         return vbool(re.search('[^\s]', self.core))
 
-    def haveSound(self):   # 是否含有有声字符(支持中文和英文)
+    def has_sound(self):   # 是否含有有声字符(支持中文和英文)
         return vbool(re.search('[\u4e00-\u9fa5\da-zA-Z]', self.core))
 
-    def haveChinese(self):
+    def has_chinese(self):
         return vbool(re.search('[\u4e00-\u9fa5]', self.core))
 
     def __bytes__(self): return self.core.encode('utf8')
 
-    def md5(self, rtype):
+    def md5(self, rtype=str):
         value = hashlib.md5(bytes(self))
-        if rtype is str: return value.hexdigest()
-        if rtype is vstr: return vstr(value.hexdigest())
-        if rtype is bytes: return value.digest()
-        raise ValueError(rtype)
-
-    def md5(self, rtype='vstr'):
-        value = hashlib.md5(bytes(self))
-        if rtype is str: return value.hexdigest()
-        if rtype in ('vstr', vstr): return vstr(value.hexdigest())
-        if rtype is bytes: return value.digest()
-        raise ValueError(rtype)
+        if rtype in (str, 'str'): return value.hexdigest()
+        if rtype in (bytes, 'bytes'): return value.digest()
+        if rtype in (vstr, 'vstr'): return vstr(value.hexdigest())
+        raise TypeError(rtype)
 
     def shake256(self, rtype='vstr', rsize=32):
         value = shake_256(bytes(self))
         if rtype is str: return value.hexdigest(ceil(rsize/2))[:rsize]
         if rtype in ('vstr', vstr): return vstr(value.hexdigest(ceil(rsize/2))[:rsize])
         if rtype is bytes: return value.digest(rsize)
-        raise ValueError(rtype)
+        raise TypeError(rtype)
 
     def __hash__(self): return hash(self.core)  # 使用内核的哈希值作为字典的键
     def __contains__(self, obj): return self._sonTypeCore(obj) in self.core
 
 
 ########################################## vbytes ##########################################
 
@@ -337,12 +339,9 @@
     
     def get(self):  # 左出
         try:
             return self.beforeGet(self.pool.popleft())
         except:
             return self.mktool()
     
-    def beforeGet(self, obj):
-        return obj
-    
-    def beforePut(self, obj):
-        return obj
+    def beforeGet(self, obj): return obj
+    def beforePut(self, obj): return obj
```

