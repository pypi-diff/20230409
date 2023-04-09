# Comparing `tmp/cnd_cr_obj_naming-0.1.0-py3-none-any.whl.zip` & `tmp/cnd_cr_obj_naming-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 2818 bytes, number of entries: 8
--rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-08 21:12 cr_obj_naming/VERSION
--rw-r--r--  2.0 unx      127 b- defN 23-Apr-08 21:12 cr_obj_naming/__init__.py
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-08 21:12 cr_obj_naming/__version__.py
--rw-r--r--  2.0 unx     1696 b- defN 23-Apr-08 21:12 cr_obj_naming/obj_naming.py
--rw-r--r--  2.0 unx      825 b- defN 23-Apr-08 21:13 cnd_cr_obj_naming-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 21:13 cnd_cr_obj_naming-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-08 21:13 cnd_cr_obj_naming-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      661 b- defN 23-Apr-08 21:13 cnd_cr_obj_naming-0.1.0.dist-info/RECORD
-8 files, 3542 bytes uncompressed, 1650 bytes compressed:  53.4%
+Zip file size: 3422 bytes, number of entries: 9
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-09 15:43 cr_obj_naming/VERSION
+-rw-r--r--  2.0 unx      187 b- defN 23-Apr-09 15:43 cr_obj_naming/__init__.py
+-rw-r--r--  2.0 unx      122 b- defN 23-Apr-09 15:43 cr_obj_naming/__version__.py
+-rw-r--r--  2.0 unx     1273 b- defN 23-Apr-09 15:43 cr_obj_naming/cnd_consul.py
+-rw-r--r--  2.0 unx     1433 b- defN 23-Apr-09 15:43 cr_obj_naming/obj_naming.py
+-rw-r--r--  2.0 unx      825 b- defN 23-Apr-09 15:43 cnd_cr_obj_naming-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 15:43 cnd_cr_obj_naming-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-09 15:43 cnd_cr_obj_naming-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      745 b- defN 23-Apr-09 15:43 cnd_cr_obj_naming-0.2.1.dist-info/RECORD
+9 files, 4696 bytes uncompressed, 2124 bytes compressed:  54.8%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: cr_obj_naming/__init__.py
 Comment: 
 
 Filename: cr_obj_naming/__version__.py
 Comment: 
 
+Filename: cr_obj_naming/cnd_consul.py
+Comment: 
+
 Filename: cr_obj_naming/obj_naming.py
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.1.0.dist-info/METADATA
+Filename: cnd_cr_obj_naming-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.1.0.dist-info/WHEEL
+Filename: cnd_cr_obj_naming-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.1.0.dist-info/top_level.txt
+Filename: cnd_cr_obj_naming-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_cr_obj_naming-0.1.0.dist-info/RECORD
+Filename: cnd_cr_obj_naming-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cr_obj_naming/VERSION

```diff
@@ -1 +1 @@
-0.1.0
+0.2.1
```

## cr_obj_naming/__init__.py

```diff
@@ -1,2 +1,3 @@
 from cr_obj_naming.__version__ import (__version__)  # noqa: F401
 from cr_obj_naming.obj_naming import ObjNaming  # noqa: F401
+from cr_obj_naming.cnd_consul import CndConsul  # noqa: F401
```

## cr_obj_naming/obj_naming.py

```diff
@@ -1,53 +1,51 @@
 from cnd_cr_object import CrObject
-import consul
 import hashlib
-import json
 
 
 class ObjNaming(CrObject):
     consul_creds = {}
 
-    def __init__(self, data, md5_length, _print):
+    def __init__(self, data, cnd_consul, md5_length, _print):
         super().__init__(_print)
         self._data = data
+        self._cnd_consul = cnd_consul
         self._md5_length = md5_length
 
-    def set_consul(self, host, port, token, path):
-        self.consul_creds["host"] = host
-        self.consul_creds["token"] = token
-        self.consul_creds["path"] = path
-        self.consul_creds["port"] = port
-        self.consul = consul.Consul(
-            host=self.consul_creds["host"],
-            port=self.consul_creds["port"],
-            token=self.consul_creds["token"]
-        )
-
-    def full_path(self, deployment_id):
-        return f'{self.consul_creds["path"]}/{deployment_id}'
-
     def _value(self):
         base_string = f"{self._data['vra_id']}-{self._data['service_name']}-{self._data['env']}"
         hash_val = hashlib.md5(f"{base_string}-{self._data['deployment_id']}".encode())
         return f"{base_string}-{hash_val.hexdigest()[0:self._md5_length]}"
+
+    def all(self):
+        return self._cnd_consul.all()
+
+    @property
+    def data(self):
+        return self._data
+       
+    @data.setter
+    def data(self, my_data):
+        self._data = my_data
         
     def save(self):
         self._data["name"] = self._value()
-        return self.consul.kv.put(self.full_path(self._data["deployment_id"]), json.dumps(self._data, indent=4))
+        self._print.trace_d(f'DeploymentId : {self._data["name"]}')
+        return self._cnd_consul.put(self._data["deployment_id"], self._data)
 
     def find_by_id(self, id):
-        index, my_data = self.consul.kv.get(self.full_path(id))
-        return json.loads(my_data['Value'])["name"]
+        my_data = self._cnd_consul.get(id)
+        self._print.trace_d(f'Raw data : {my_data}')
+        return my_data["name"]
         
-    def update(self, obj_naming):
-        return obj_naming.save()
+    def update(self):
+        return self.save()
         
     def destroy(self):
-        return self.consul.kv.delete(self.full_path(self._data["deployment_id"]))
+        return self._cnd_consul.destroy(self._data["deployment_id"])
         
     def has_children(self):
         return False
         
     def find_relation(self):
         return []
```

## Comparing `cnd_cr_obj_naming-0.1.0.dist-info/METADATA` & `cnd_cr_obj_naming-0.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-cr-obj-naming
-Version: 0.1.0
+Version: 0.2.1
 Summary: Base for vro Custom Resource Object Naming
 Home-page: https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
```

